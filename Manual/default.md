# 📘 Manual do Usuário - GC Driver

Bem-vindo ao guia detalhado por módulos do **GC Driver**. Escolha o módulo abaixo para aprender a utilizar todas as funcionalidades.

---

## 📚 Índice de Módulos

| # | Módulo | Descrição |
|---|--------|-----------|
| 1 | [💰 Gestão Financeira](GestaoFinanceira.md) | Livro caixa, lançamentos, receitas e despesas |
| 2 | [🚗 Gestão de Veículos](GestaoVeiculos.md) | Cadastro e gerenciamento da sua frota |
| 3 | [⛽ Controle de Abastecimento](ControleAbastecimento.md) | Registro de combustível e cálculo de consumo |
| 4 | [📝 Diário de Bordo](DiarioBordo.md) | Jornadas de trabalho e cálculo de eficiência |
| 5 | [🔧 Manutenção Preventiva](ManutencaoPreventiva.md) | Lembretes de manutenção baseados em KM |
| 6 | [⚙️ Configurações e Backup](ConfiguracoesBackup.md) | Categorias, backup local e sincronização na nuvem |

---

## 💰 1. Gestão Financeira (Livro Caixa)

*O coração do seu controle financeiro diário.*

### 🔹 O que é?

Aqui você registra todo o dinheiro que entra (corridas, gorjetas) e sai (alimentação, manutenção, combustível). O objetivo é saber o seu **Lucro Líquido** real.

### 🔹 Como usar:

1. **Novo Lançamento:**
   * Toque no botão **`+`** no Dashboard.
   * Escolha **Receita** (Verde) ou **Despesa** (Vermelho).
   * Digite o valor.
   * Escolha uma Categoria (ex: Uber, Gasolina).
   * Toque em Salvar.

2. **Editar/Excluir:**
   * Toque em um item da lista para editar.
   * Deslize o item para a esquerda para ver o botão "Excluir".

3. **Saldo do Dia:**
   * No topo do Dashboard, veja o quadro "Hoje". Se estiver vermelho, significa que gastou mais do que ganhou hoje.

📖 [Ver guia completo de Gestão Financeira](GestaoFinanceira.md)

---

## 🚗 2. Gestão de Veículos

*Cadastre sua frota para cálculos precisos.*

### 🔹 O que é?

Permite registrar um ou mais carros. O sistema precisa saber qual carro você está usando para calcular a média de consumo e alertar sobre a manutenção correta.

### 🔹 Como usar:

1. Acesse o menu **Configurações** (Engrenagem) > **Meus Veículos** (ou ícone de Carro no topo).
2. Toque em **Novo**.
3. Informe o Modelo (ex: Onix) e Placa.
4. Informe o **KM Atual** do odômetro (olhe no painel).
5. **Ativar Veículo:** Ao salvar, marque a opção "Veículo Principal (Ativo)". O sistema usará este carro para todos os cálculos a partir de agora.

📖 [Ver guia completo de Gestão de Veículos](GestaoVeiculos.md)

---

## ⛽ 3. Controle de Abastecimento

*Controle cada gota de combustível.*

### 🔹 O que é?

Registra quando você para no posto. O sistema usa isso para calcular a média (KM/L) e o custo por quilômetro rodado.

### 🔹 Como usar:

1. Toque no ícone de **Bomba de Combustível** no Dashboard.
2. Verifique se o veículo exibido no topo é o que está abastecendo.
3. Informe:
   * **Odômetro:** O KM total do carro no momento do abastecimento.
   * **Valor Total (R$):** Quanto pagou.
   * **Litros:** Quantidade exata (olhe na bomba).
4. **Integração Financeira:** Mantenha a opção "Lançar no Financeiro" marcada para criar automaticamente uma despesa no seu caixa.

> **Dica:** Tente encher o tanque ou abastecer sempre da mesma forma para que o cálculo de média (KM/L) seja mais preciso.

📖 [Ver guia completo de Controle de Abastecimento](ControleAbastecimento.md)

---

## 📝 4. Diário de Bordo (Jornadas)

*Sua folha de ponto inteligente.*

### 🔹 O que é?

Registra o início e fim do seu trabalho. É aqui que descobrimos sua eficiência real (Lucro vs KM Rodado).

### 🔹 Passo a Passo de um Dia:

1. **Iniciar o Dia:** Ao entrar no carro, toque no ícone de **Prancheta** e depois no **Play (Iniciar)**.
   * *Dica:* Zere o **Trip A** do painel do carro neste momento.

2. **Trabalhar:** Faça suas corridas normalmente.

3. **Fechar o Dia:** Quando chegar em casa:
   * Volte à lista de Diários.
   * Toque no registro que está "EM ANDAMENTO".
   * Informe o **KM do Trip** (o que você zerou de manhã).
   * Informe o **KM dos Apps** (some o total rodado na Uber + 99).
   * Se abasteceu hoje, selecione o abastecimento na lista para calcular o custo exato do dia.
   * Toque em Salvar.

### 🔹 Entendendo os Resultados:

* **KM Real:** Quanto o carro andou de verdade.
* **KM App:** Quanto as plataformas pagaram para você andar.
* **KM Morta (Ocioso):** A diferença. Se for alta, você está andando muito vazio.
* **Custo por KM:** Quanto custou cada KM rodado hoje em combustível.

📖 [Ver guia completo de Diário de Bordo](DiarioBordo.md)

---

## 🔧 5. Manutenção Preventiva

*Nunca mais esqueça de trocar o óleo.*

### 🔹 O que é?

Um sistema de lembretes que monitora o odômetro do carro automaticamente.

### 🔹 Como usar:

1. Toque no ícone de **Chave Inglesa** (Manutenção).
2. Toque em **Novo**.
3. Escolha o serviço (ex: Troca de Óleo).
4. Defina o intervalo (ex: a cada 10.000 km).
5. Informe qual foi a KM da última troca.
6. O sistema mostrará uma barra de progresso. Quando estiver perto de vencer, ficará amarela/vermelha.

📖 [Ver guia completo de Manutenção Preventiva](ManutencaoPreventiva.md)

---

## ⚙️ 6. Configurações e Backup

*Segurança dos seus dados.*

### 🔹 Categorias Personalizadas:

* Vá em Configurações > **Gerenciar Categorias**.
* Crie novas categorias (ex: "Multa", "Lanche", "Gorjeta") escolhendo ícones e cores.

### 🔹 Backup na Nuvem (Automático):

* O GC Driver agora sincroniza seus dados automaticamente na nuvem (Azure CosmosDB).
* Trocou de celular? Instale o app e seus dados serão baixados automaticamente.
* Funciona offline - os dados são sincronizados quando você conectar à internet.

### 🔹 Backup Local (Manual):

* Para segurança extra, vá em Configurações > **Backup de Dados**.
* Toque em **Exportar** regularmente e guarde o arquivo no seu Google Drive ou envie para si mesmo no WhatsApp.
* Se trocar de celular, instale o app e use a opção **Restaurar** com esse arquivo.

📖 [Ver guia completo de Configurações e Backup](ConfiguracoesBackup.md)

---

## 🔗 Links Úteis

- [📋 Histórico de Versões (CHANGELOG)](../CHANGELOG.md)
- [🔌 Documentação da API](../API.md)
- [📖 Manual do Usuário (Resumo)](../Manual_do_Usuario.md)
- [💻 Manual Técnico](../Manual_Tecnico.md)