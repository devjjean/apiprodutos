# 🛒 API de Produtos

Uma API REST feita com **Java + Spring Boot**, que permite **cadastrar, listar, buscar por ID, atualizar e deletar produtos**. Esse projeto foi feito com foco em aprendizado e prática com desenvolvimento de APIs RESTful.

---

## 🚀 Tecnologias utilizadas

- Java 17  
- Spring Boot  
- Spring Web  
- Spring Data JPA  
- H2 Database (banco de dados em memória)  
- Postman (para testar os endpoints)

---

## 📦 Endpoints da API

| Método | Rota              | Ação                          |
|--------|-------------------|-------------------------------|
| GET    | `/produtos`       | Listar todos os produtos      |
| GET    | `/produtos/{id}`  | Buscar produto por ID         |
| POST   | `/produtos`       | Criar um novo produto         |
| PUT    | `/produtos/{id}`  | Atualizar produto existente   |
| DELETE | `/produtos/{id}`  | Deletar produto por ID        |

---

## 🧪 Testando com Postman

### 🔹 Criar produto (`POST /produtos`)
**Body (raw / JSON):**
```json
{
  "nome": "Smartphone Samsung",
  "descricao": "Galaxy S21 com 128GB de memória",
  "preco": 2599.99
}

```
🔹 Listar produtos (GET /produtos)
Sem body.

🔹 Buscar produto por ID (GET /produtos/{id})
Exemplo: GET /produtos/1

🔹 Atualizar produto (PUT /produtos/{id})
Body (raw / JSON):
```json
{
  "nome": "Smartphone Samsung Atualizado",
  "descricao": "Galaxy S21 Ultra",
  "preco": 3199.99
}
```
🔹 Deletar produto (DELETE /produtos/{id})
Exemplo: DELETE /produtos/1

🛠️ Como rodar o projeto
Clone o repositório:
```json
git clone https://github.com/seu-usuario/apiprodutos.git
```
Abra no IntelliJ ou VSCode com suporte a Java.

Rode a aplicação pela classe:

ApiprodutosApplication.java
Acesse:
http://localhost:8080/produtos
