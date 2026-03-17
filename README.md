# API de Produtos

## Descrição

API REST desenvolvida em Node.js com Express para gerenciamento de produtos.
Permite criar, listar, filtrar, ordenar e paginar produtos.

---

## Tecnologias utilizadas

* Node.js
* Express
* Postman

---

## Endpoints

---

### POST /api/produtos

Cria um novo produto.

#### Body (JSON):

```json
{
  "nome": "Teclado",
  "preco": 200,
  "categoria": "Informática"
}
```

#### Resposta:

```json
{
  "id": 3,
  "nome": "Teclado",
  "preco": 200,
  "categoria": "Informática"
}
```

#### Validações:

* Nome obrigatório
* Preço deve ser um número maior que 0
* Categoria obrigatória

---

### GET /api/produtos

Lista produtos com filtros, ordenação e paginação.

#### Parâmetros:

* categoria
* preco_min
* preco_max
* ordem (preco ou nome)
* direcao (asc ou desc)
* pagina
* limite

---

### GET /api/produtos/:id

Busca produto por ID.

---

## Testes no Postman

### Criando produtos (POST)

prints/post-criar-produto.png
prints/post-criar-produto2.png
prints/post-criar-produto3.png
prints/post-criar-produto4.png
prints/post-criar-produto5.png

---

### Listar produtos

prints/get-listar-produtos.png

---

### Buscar produto por ID

prints/get-produto-id.png

---

### Filtro por categoria

prints/get-produto-categoria.png

---

### Ordenação

prints/get-produto-ordenacao.png

---

### Paginação

prints/get-produto-paginacao.png

---

## Collection do Postman

A collection utilizada está disponível no arquivo:

```
postman_collection.json
```
