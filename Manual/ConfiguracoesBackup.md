# ⚙️ Configurações e Backup

*Segurança dos seus dados.*

---

## 🔹 Categorias Personalizadas

### O que são?
As categorias organizam seus lançamentos financeiros. Você pode personalizar para refletir melhor sua rotina.

### Como gerenciar

1. Vá em **Configurações** (ícone de engrenagem).
2. Toque em **Gerenciar Categorias**.
3. Você pode:
   - **Criar** novas categorias
   - **Editar** categorias existentes
   - **Excluir** categorias (exceto as protegidas)

### Criando uma Categoria

1. Toque em **Nova**.
2. Preencha:
   - **Nome**: Ex: "Multa", "Lanche", "Gorjeta"
   - **Tipo**: Receita ou Despesa
   - **Ícone**: Escolha um ícone da lista
   - **Cor**: Escolha uma cor para identificar

> ⚠️ **Categorias protegidas** (Combustível, Uber, 99) não podem ser excluídas pois são usadas internamente pelo sistema.

---

## 🔹 Backup de Dados

### Backup Automático na Nuvem ☁️

O GC Driver agora salva seus dados automaticamente na nuvem segura (Azure CosmosDB).

**Vantagens:**
- ✅ Seus dados estão protegidos mesmo se perder o celular
- ✅ Troque de aparelho sem perder nada
- ✅ Sincronização automática quando conectado à internet

**Como funciona:**
- O app prioriza o funcionamento **offline** (sempre funciona sem internet)
- Quando você conecta à internet, os dados são sincronizados automaticamente
- Ao instalar em um novo celular, seus dados são baixados automaticamente

### Backup Local (Manual)

Para segurança extra, você pode fazer backup manual:

1. Vá em **Configurações > Backup de Dados**.
2. Toque em **Exportar**.
3. Um arquivo `.db3` será gerado.
4. **Salve esse arquivo em local seguro:**
   - Envie para seu e-mail
   - Salve no Google Drive
   - Envie para si mesmo no WhatsApp

### Restaurando um Backup Local

1. Instale o app no novo celular.
2. Vá em **Configurações > Backup de Dados**.
3. Toque em **Restaurar**.
4. Selecione o arquivo `.db3` que você salvou.

> ⚠️ **Atenção:** A restauração local **substitui** todos os dados atuais do app.

---

## 🔹 Outras Configurações

### Veículo Ativo
Defina qual carro você está usando atualmente para cálculos corretos.

### Metas Financeiras
Configure metas diárias ou mensais de faturamento.

### Tipos de Serviço
Gerencie os tipos de manutenção preventiva.

---

## 🔹 Perguntas Frequentes

**P: Troquei de celular. O que fazer?**
R: Se você tem backup na nuvem, basta instalar o app que os dados são baixados automaticamente. Se preferir backup local, restaure o arquivo `.db3`.

**P: O app funciona sem internet?**
R: Sim! O GC Driver funciona 100% offline. A internet é usada apenas para sincronização de backup.

**P: Posso usar o app em dois celulares?**
R: Sim, os dados são sincronizados entre os dispositivos através da nuvem.

---

[⬅ Voltar ao Manual Principal](Default.md)
