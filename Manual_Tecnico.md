# 💻 Manual Técnico - GC Driver

> Informações detalhadas sobre a arquitetura e desenvolvimento do projeto.

---

## 🛠️ Stack Tecnológica

O **GC Driver** utiliza uma arquitetura híbrida e robusta, focada em performance para dispositivos móveis Android.

*   **Front-end:** Xamarin.Forms (XAML/C#)
*   **Core/Backend Logic:** .NET Standard 2.0 (VB.NET)
*   **Banco de Dados:** SQLite (via biblioteca `sqlite-net-pcl`)
*   **Arquitetura:** MVVM (Model-View-ViewModel) com padrão Repository e Unit of Work.

---

## 🏗️ Estrutura da Solução

A solução segue os princípios **SOLID** e é dividida em camadas lógicas:

### 1. `GCDriver` (Projeto Principal - C#)
Este projeto contém a camada de apresentação e inicialização.
*   **Views:** Pages em XAML que compõem a interface do usuário.
*   **Responsabilidade:** UI, Navegação entre telas e Injeção de Dependência (`App.Repo`).

### 2. `GCDriver.Core` (Biblioteca de Classes - VB.NET)
O coração da lógica do aplicativo.
*   **Models:** Entidades que mapeiam as tabelas do banco de dados (ex: `Lancamentos`, `Veiculos`).
*   **Interfaces:** Contratos para desacoplamento (ex: `IRepositoryManager`).
*   **Repositories:** Contém as regras de negócio, cálculos financeiros complexos e acesso a dados.
*   **ViewModels:** Faz a ponte entre os dados e a View, gerenciando o estado da tela (ex: `DashboardPageViewModel`).
*   **Behaviors/Converters:** Lógicas auxiliares de conversão (ex: formatação de moeda) e validação.

---

## 📐 Decisões de Arquitetura

*   **Inversão de Dependência:** As ViewModels nunca instanciam repositórios diretamente; elas dependem de Interfaces (`IRepositoryManager`), facilitando testes e manutenção.
*   **Code-First:** O banco de dados SQLite é gerado e migrado automaticamente com base nas definições das classes Model na inicialização do app.
*   **Hydration:** Para otimizar a performance, o carregamento de dados relacionados (como a Categoria de um Lançamento) é feito sob demanda (Lazy Loading ou Hydration explícito) nos repositórios.
*   **Performance de UI:** Uso extensivo de `CollectionView` para listas longas e compilação de XAML (XAMLC) habilitada. Queries de banco de dados são otimizadas com filtros por período.

---

## 🚀 Compilação e Deploy

Os pacotes APK localizados na pasta `versoes` são gerados através do build de Release do Visual Studio com assinatura digital (Keystore) para permitir a instalação e atualização segura no Android.
