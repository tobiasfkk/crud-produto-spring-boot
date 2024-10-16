# Spring Boot Produto Teste

Esta é uma aplicação Spring Boot para gerenciamento de produtos. Inclui operações básicas de CRUD e usa Maven para gerenciamento de dependências.

### Clone o repositório:
  
    git clone https://github.com/tobiasfkk/crud-produto-spring-boot.git
  
Ao executar, a aplicação será iniciada em `http://localhost:8080`.

Edite o arquivo application.properties com URL, USUÁRIO e SENHA da sua base de dados `src/main/resources/application.properties`.

## Endpoints da API

### Criar um novo produto
- **URL:** `/api/produtos`
- **Método:** `POST`
- **Corpo da Requisição:**
    ```json
    {
        "nome": "Nome do Produto",
        "preco": 100.0
    }
    ```

### Obter um produto pelo ID
- **URL:** `/api/produtos/{id}`
- **Método:** `GET`

### Atualizar um produto pelo ID
- **URL:** `/api/produtos/updateProdutoById`
- **Método:** `POST`
- **Corpo da Requisição:**
    ```json
    {
        "id": 1,
        "nome": "Nome do Produto Atualizado",
        "preco": 150.0
    }
    ```

## Construído com

- [Spring Boot](https://spring.io/projects/spring-boot) - O framework web utilizado
- [Maven](https://maven.apache.org/) - Gerenciamento de dependências
