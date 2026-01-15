# 📖 Manual do Usuário - GC Driver

Bem-vindo ao **GC Driver**, o seu parceiro definitivo para gestão inteligente de transportes. Este manual foi criado para ajudar você a explorar ao máximo todas as funcionalidades do aplicativo.

---

## 🚀 Primeiros Passos

### O que é o GC Driver?
O GC Driver não é apenas um livro caixa. Ele é uma ferramenta completa que cruza dados de abastecimento, quilometragem e faturamento para lhe entregar o **Custo Real por KM** e o seu **Lucro Líquido Real**.

Ao abrir o aplicativo pela primeira vez, recomendamos que você:
1.  **Cadastre seu Veículo**: Insira os dados do carro que você utiliza. Se você aluga, pode cadastrar vários.
2.  **Configure suas Categorias**: O app já vem com categorias padrão (Combustível, Alimentação, Manutenção), mas você pode personalizá-las.

---

## 📱 Guia de Uso Diário

A rotina no GC Driver é pensada para ser rápida e não atrapalhar suas corridas.

### 1. Iniciando o Dia (Diário de Bordo)
O **Diário de Bordo** é o coração do cálculo de eficiência.
1.  No Dashboard (tela inicial), toque no ícone de **Prancheta**.
2.  Toque no botão **Play (Iniciar)**.
3.  **IMPORTANTE:** Zere o hodômetro parcial (Trip A/B) do painel do seu carro neste momento. O app registrará a hora de início automaticamente.

### 2. Durante o Dia (Lançamentos Financeiros)
Fez uma corrida por fora? Gastou com um lanche? Pagou uma lavagem?
1.  Toque no botão **+** no Dashboard.
2.  Selecione **Receita** (dinheiro entrando) ou **Despesa** (dinheiro saindo).
3.  Digite o valor, selecione uma categoria e salve.
    *   *Dica: Você pode adicionar uma observação para lembrar do detalhe depois.*

### 3. Abastecendo
Para ter o cálculo exato de consumo e custo:
1.  Toque no ícone de **Bomba de Combustível**.
2.  Informe três dados essenciais:
    *   **Valor Total** (em R$).
    *   **Litros** abastecidos.
    *   **Odômetro Total** do carro (KM atual).
3.  Marque a opção **"Lançar no Financeiro"**. Isso cria automaticamente uma despesa no seu caixa, poupando trabalho.

### 4. Fechando o Dia
Ao encerrar seu turno:
1.  Volte na lista de Diários (ícone de Prancheta).
2.  Toque no registro que está "EM ANDAMENTO".
3.  Preencha os dados finais:
    *   **KM do Trip**: Quanto você rodou no painel do carro desde que iniciou.
    *   **KM dos Apps**: Some o que a Uber/99 dizem que você rodou em corrida.
4.  O app calculará imediatamente:
    *   Sua **KM Morta** (quanto rodou vazio).
    *   Seu **Lucro Líquido** (descontando combustível e depreciação).

---

## 🛠️ Funcionalidades Detalhadas

### 💰 Gestão Financeira
*   **Saldo em Tempo Real:** No topo da tela, você vê o caixa acumulado e o resultado específico do dia ("Hoje").
*   **Histórico:** Veja todos os lançamentos passados, filtre por data ou categoria.

### 🚗 Gestão de Frota
*   **Múltiplos Veículos:** Ideal para quem tem mais de um carro ou troca de carro alugado com frequência.
*   **Veículo Ativo:** O app sempre considera o veículo marcado como "Ativo" para os cálculos de média de consumo.

### 🔧 Manutenção Preventiva
Não deixe passar a hora da troca de óleo!
*   **Cadastre Lembretes:** Informe com qual KM deve ser feita a próxima manutenção (ex: Troca de Óleo aos 100.000 km).
*   **Monitoramento Automático:** Conforme você lança abastecimentos e diários, o app monitora o odômetro e avisa quando a manutenção estiver próxima.

### 🛡️ Segurança e Backup
*   **Offline First:** O GC Driver funciona 100% sem internet. Seus dados estão salvos no seu celular.
*   **Backup:** Vá em Configurações > Backup para exportar seus dados. O arquivo gerado (`.db3`) pode ser salvo no Google Drive ou enviado por e-mail. Use a função "Restaurar" se trocar de celular.

---

## ❓ Perguntas Frequentes (FAQ)

**P: O aplicativo precisa de internet?**
R: Não! O GC Driver funciona totalmente offline.

**P: Como ele calcula o custo da gasolina se eu não abasteci hoje?**
R: O app usa a **média de consumo** do seu histórico e o **preço do último abastecimento** para calcular quanto você gastou exatamente nos KMs que rodou hoje.

**P: Posso usar em dois celulares ao mesmo tempo?**
R: Atualmente não. O banco de dados é local para garantir privacidade e velocidade.

---

## 📄 Suporte e Contato
Encontrou um bug ou tem uma sugestão? Entre em contato com o desenvolvedor através da loja de aplicativos.

*© 2025 GC Driver. Todos os direitos reservados.*
