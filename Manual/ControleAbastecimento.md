# ⛽ Controle de Abastecimento

*Controle cada gota de combustível.*

---

## 🔹 O que é?

Registra quando você para no posto. O sistema usa isso para calcular a **média de consumo (KM/L)** e o **custo por quilômetro rodado**.

---

## 🔹 Como usar

### Registrando um Abastecimento

1. Toque no ícone de **Bomba de Combustível** no Dashboard.
2. Verifique se o veículo exibido no topo é o que está abastecendo.
3. Preencha os dados:
   - **Odômetro**: O KM total do carro no momento do abastecimento.
   - **Valor Total (R$)**: Quanto você pagou.
   - **Litros**: Quantidade exata abastecida (olhe na bomba).
4. **Integração Financeira**: Mantenha a opção **"Lançar no Financeiro"** marcada para criar automaticamente uma despesa no seu caixa.
5. Toque em **Salvar**.

### Visualizando o Histórico

1. Toque no ícone de **Bomba de Combustível**.
2. Acesse a **Lista de Abastecimentos**.
3. Veja todos os registros ordenados por data.

---

## 🔹 Cálculos Automáticos

### Média de Consumo (KM/L)
O sistema calcula automaticamente quantos quilômetros você roda por litro de combustível.

**Fórmula:**
```
Média = (Odômetro Atual - Odômetro Anterior) / Litros Abastecidos
```

### Custo por KM
Quanto custa cada quilômetro rodado em combustível.

**Fórmula:**
```
Custo/KM = Valor do Abastecimento / KM Rodados
```

---

## 🔹 Dicas para Cálculos Precisos

> 💡 **Encha o tanque sempre!** Abastecimentos parciais prejudicam o cálculo de média.

> 💡 **Abasteça sempre da mesma forma** (tanque cheio → tanque cheio) para resultados mais precisos.

> 💡 **Anote o odômetro corretamente.** Um erro de 100 km pode distorcer bastante a média.

---

## 🔹 Vinculando ao Diário de Bordo

Ao fechar um Diário de Bordo, você pode selecionar um abastecimento do dia para vincular. Isso permite que o sistema calcule o **custo exato de combustível daquele turno**.

---

## 🔹 Perguntas Frequentes

**P: Preciso anotar o odômetro a cada abastecimento?**
R: Sim! É fundamental para o cálculo de consumo funcionar.

**P: Posso editar um abastecimento depois?**
R: Sim. Toque no item da lista e faça as correções.

**P: O que acontece se eu não marcar "Lançar no Financeiro"?**
R: O abastecimento é registrado para cálculo de consumo, mas NÃO aparece como despesa no seu caixa. Você precisaria lançar manualmente depois.

---

[⬅ Voltar ao Manual Principal](Default.md)
