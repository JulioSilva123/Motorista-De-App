# 🔌 Documentação da API REST

Documentação dos endpoints da Web API do GC Driver para sincronização de dados.

---

## Visão Geral

**Base URL:** `https://api.gcdriver.com/v1` (exemplo)

**Autenticação:** Bearer Token (JWT)

**Content-Type:** `application/json`

---

## Endpoints

### 👤 Usuários

#### POST /usuarios/login
Autentica um usuário e retorna token de acesso.

**Request:**
```json
{
  "email": "motorista@email.com",
  "senha": "senha123"
}
```

**Response (200):**
```json
{
  "token": "eyJhbGciOiJIUzI1NiIs...",
  "usuario": {
    "id": 1,
    "nome": "João Silva",
    "email": "motorista@email.com"
  }
}
```

#### POST /usuarios/registro
Registra um novo usuário.

#### GET /usuarios/{id}
Retorna dados do usuário.

---

### 🚗 Veículos

#### GET /veiculos
Lista todos os veículos do usuário.

#### GET /veiculos/{id}
Retorna um veículo específico.

#### POST /veiculos
Cria um novo veículo.

**Request:**
```json
{
  "modelo": "Onix",
  "placa": "ABC-1234",
  "ano": 2022,
  "km_atual": 45000
}
```

#### PUT /veiculos/{id}
Atualiza um veículo existente.

#### DELETE /veiculos/{id}
Remove um veículo.

---

### 💰 Lançamentos

#### GET /lancamentos
Lista lançamentos com filtro por período.

**Query Params:**
- `mes` (int): Mês de referência
- `ano` (int): Ano de referência

#### GET /lancamentos/{id}
Retorna um lançamento específico.

#### POST /lancamentos
Cria um novo lançamento.

**Request:**
```json
{
  "vl_lancamento": 150.00,
  "dt_lancamento": "2025-01-15",
  "id_categoria": 1,
  "ds_observacao": "Corrida Uber"
}
```

#### PUT /lancamentos/{id}
Atualiza um lançamento.

#### DELETE /lancamentos/{id}
Remove um lançamento.

---

### 🏷️ Categorias

#### GET /categorias
Lista todas as categorias.

#### POST /categorias
Cria nova categoria personalizada.

#### PUT /categorias/{id}
Atualiza uma categoria.

#### DELETE /categorias/{id}
Remove categoria (se não for protegida).

---

### ⛽ Abastecimentos

#### GET /abastecimentos
Lista abastecimentos do usuário.

#### GET /abastecimentos/{id}
Retorna um abastecimento específico.

#### POST /abastecimentos
Registra novo abastecimento.

**Request:**
```json
{
  "id_veiculo": 1,
  "nr_odometro": 46500,
  "vl_total": 280.00,
  "qt_litros": 45.5,
  "dt_abastecimento": "2025-01-15",
  "lancar_financeiro": true
}
```

#### DELETE /abastecimentos/{id}
Remove um abastecimento.

---

### 📝 Diários

#### GET /diarios
Lista diários de bordo.

#### GET /diarios/{id}
Retorna um diário específico.

#### POST /diarios
Inicia um novo diário.

#### PUT /diarios/{id}
Fecha/atualiza um diário.

**Request (fechamento):**
```json
{
  "hr_fim": "2025-01-15T18:30:00",
  "nr_km_trip": 150,
  "nr_km_app": 100,
  "id_abastecimento": 5
}
```

---

### 🔧 Manutenção

#### GET /lembretes-manutencao
Lista lembretes de manutenção ativos.

#### POST /lembretes-manutencao
Cria novo lembrete.

#### GET /historico-manutencao
Lista histórico de manutenções realizadas.

#### POST /historico-manutencao
Registra manutenção realizada.

---

### 📊 Saldos Mensais

#### GET /saldos-mensais
Lista checkpoints de saldo por mês.

#### GET /saldos-mensais/{mes}/{ano}
Retorna saldo de um mês específico.

---

### 🎯 Metas

#### GET /metas
Lista metas do usuário.

#### POST /metas
Cria nova meta.

#### PUT /metas/{id}
Atualiza uma meta.

---

## Códigos de Resposta

| Código | Descrição |
|--------|-----------|
| 200 | Sucesso |
| 201 | Criado com sucesso |
| 400 | Requisição inválida |
| 401 | Não autorizado |
| 404 | Recurso não encontrado |
| 500 | Erro interno do servidor |

---

## Exemplo de Erro

```json
{
  "error": true,
  "message": "Categoria não encontrada",
  "code": "CATEGORY_NOT_FOUND"
}
```
