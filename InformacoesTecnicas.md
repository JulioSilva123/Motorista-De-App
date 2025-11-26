# 🚗 GC Driver - Gestão Inteligente para Motoristas

> **O parceiro definitivo para quem vive do volante.**
> Controle financeiro, gestão de frota, cálculo de eficiência e diário de bordo em um único aplicativo.
 
---

## 💻 Informações Técnicas (Para Desenvolvedores)

Este projeto utiliza uma arquitetura híbrida e robusta, focada em performance e manutenibilidade.

### Stack Tecnológica
- **Front-end:** Xamarin.Forms (XAML/C#)
- **Core/Backend Logic:** .NET Standard 2.0 (VB.NET)
- **Banco de Dados:** SQLite (sqlite-net-pcl)
- **Arquitetura:** MVVM (Model-View-ViewModel) com Repository Pattern e Unit of Work.

### Estrutura da Solução
A solução é dividida em camadas seguindo os princípios **SOLID**:

1.  **`GCDriver` (Projeto Principal - C#):**
    * Contém as **Views** (Pages XAML).
    * Responsável pela UI, Navegação e Injeção de Dependência (`App.Repo`).
    
2.  **`GCDriver.Core` (Biblioteca de Classes - VB.NET):**
    * **Models:** Entidades do banco de dados (`Lancamentos`, `Veiculos`, etc).
    * **Interfaces:** Contratos dos repositórios (`IRepositoryManager`).
    * **Repositories:** Regras de negócio, cálculos complexos e acesso a dados.
    * **ViewModels:** Lógica de apresentação e estado (`DashboardPageViewModel`).
    * **Behaviors/Converters:** Lógicas auxiliares de UI (Validação monetária, cores).

### Decisões de Arquitetura
* **Inversão de Dependência:** As ViewModels dependem de Interfaces (`IRepositoryManager`), não de classes concretas.
* **Code-First:** O banco de dados é gerado e migrado automaticamente baseado nas classes Model.
* **Hydration:** O carregamento de dados relacionados (ex: Categoria de um Lançamento) é feito sob demanda nos repositórios para otimizar performance.
* **Performance:** Uso de `CollectionView`, compilação de XAML e queries otimizadas com Paginação/Filtro por período.

---

## 📄 Licença e Direitos

Este projeto é um software proprietário desenvolvido para auxiliar a comunidade de motoristas.
*© 2025 GC Driver. Todos os direitos reservados.*