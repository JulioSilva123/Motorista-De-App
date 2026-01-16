# 🚗 GC Driver - Gestão Inteligente para Motoristas

> **O parceiro definitivo para quem vive do volante.**
> Controle financeiro, gestão de frota, cálculo de eficiência e diário de bordo em um único aplicativo.

---

## 📖 Sobre o Projeto

O **GC Driver** é um aplicativo móvel focado em resolver a maior dor dos motoristas de aplicativo: **saber o lucro real**.

Diferente dos apps das plataformas (Uber/99) que mostram apenas o faturamento bruto, o GC Driver calcula o custo por KM, a depreciação, o consumo de combustível e a "KM Morta" (rodagem sem passageiro), entregando a verdade sobre o rendimento do dia.

---

## ✨ Principais Funcionalidades

| Funcionalidade | Descrição |
|----------------|-----------|
| 💰 Gestão Financeira | Livro caixa com receitas, despesas e saldo em tempo real |
| 📝 Diário de Bordo | Registro de jornadas com cálculo de KM Morta |
| ⛽ Controle de Abastecimento | Registro de combustível e média de consumo (KM/L) |
| 🚗 Gestão de Veículos | Suporte a múltiplos veículos |
| 🔧 Manutenção Preventiva | Lembretes baseados em quilometragem |
| ☁️ Backup na Nuvem | Sincronização automática com Azure CosmosDB |

---

## 📚 Documentação

Acesse a documentação completa para aprender a usar ou modificar o sistema:

### Para Motoristas
- 📖 **[Manual do Usuário](Manual_do_Usuario.md)** - Guia completo de uso do aplicativo
- 📘 **[Manual por Módulos](Manual/Default.md)** - Guias detalhados de cada funcionalidade

### Para Desenvolvedores
- 💻 **[Manual Técnico](Manual_Tecnico.md)** - Arquitetura, banco de dados e stack tecnológica
- 🔌 **[Documentação da API](API.md)** - Endpoints da Web API REST
- 📋 **[Changelog](CHANGELOG.md)** - Histórico de versões

---

## 📥 Instalação

As versões compiladas do aplicativo (APK para Android) estão disponíveis no diretório `versoes`.

1. Navegue até a pasta `versoes`.
2. Entre na pasta da versão mais recente (ex: `0.1.5`).
3. Copie o arquivo `.apk` para o seu dispositivo Android.
4. Instale habilitando "Fontes Desconhecidas" se necessário.

---

## 🛠️ Stack Tecnológica

| Camada | Tecnologia |
|--------|------------|
| Front-end Mobile | Xamarin.Forms (XAML/C#) |
| Lógica de Negócio | .NET Standard 2.0 (VB.NET) |
| Banco Local | SQLite |
| Nuvem | Azure CosmosDB |
| Web API | ASP.NET Core |

---

## 📄 Licença

Este projeto é distribuído sob a licença **GPL v3**. Veja o arquivo [LICENSE.txt](LICENSE.txt) para mais detalhes.

*© 2025 GC Driver. Todos os direitos reservados.*