# MoneyMinder

## Requisitos 

- [ ] CRUD Movimentações 
- [ ] CRUD Categorias 
- [ ] Dashboard
- [ ] Autenticação

## Endpoints 

## Categorias 

GET /categoria/

Lista todas as categorias cadastradas no sistema.

*Códigos de status*
200 sucesso

---
GET /categoria/{id}

Retorna os detalhes de uma categoria com o 'id' informado.

*Códigos de status*
200 sucesso
404 id não encontrado

---
POST/categoria

Cadastrar uma nova categoria.

| campo | tipo | obrigatório | descrição 
|-------|------|-------------|-----------
| nome  |string|    sim      | um nome curto para identificar a categoria 
| icone |string|    nao      | o nome do icone conforme biblioteca material design 

*Códigos de status*
201 criado com sucesso
400 validação falhou

---
DELETE /categoria/{id}

Apaga a categoria com o 'id' informado.

*Códigos de status*
204 apagado com sucesso
404 id não encontrado

---
PUT /categoria/{id}

Altera a categoria com o 'id' informado.

| campo | tipo | obrigatório | descrição 
|-------|------|-------------|-----------
| nome  |string|    sim      | novo nome curto para identificar a categoria 
| icone |string|    nao      | novo nome do icone conforme biblioteca material design

*Códigos de status*
200 sucesso
404 id não encontrado
400 validação falhou 

*Scheme*

js
{
    "id": 1,
    "nome": "Alimentação",
    "icone": "fast-food"
}
