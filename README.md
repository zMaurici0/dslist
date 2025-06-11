 ## DSList - Catálogo de Jogos com Spring Boot

Projeto backend desenvolvido com **Java + Spring Boot**, que oferece uma API REST para listar jogos organizados por categorias (listas). É possível consultar todos os jogos, buscar por ID, visualizar todas as listas e os jogos dentro de uma lista específica.
Feito durante o evento Intensivão Java spring organizado pelo [devsuperior](https://devsuperior.com.br)

## Tecnologias

- Java 17+
- Spring Boot
- Spring Web
- Spring Data JPA
- H2 Database (em memória)
- Maven

## Como Executar

1. Clone o repositório:

```
git clone https://github.com/zMaurici0/dslist.git
cd dslist
```

2. Execute o projeto em sua IDE:
```
mvnw spring-boot:run
```

3. Acesse o H2 Console (opcional):

- URL: http://localhost:8080/h2-console
- JDBC URL: jdbc:h2:mem:testdb
- Usuário: sa
- Senha: (deixe em branco)

## Endpoints

| Método | URL                     | Descrição                             |
| ------ | ----------------------- | ------------------------------------- |
| GET    | `/games`                | Retorna todos os jogos (resumo)       |
| GET    | `/games/{id}`           | Retorna os dados completos de um jogo |
| GET    | `/lists`                | Retorna todas as listas de jogos      |
| GET    | `/lists/{listId}/games` | Retorna os jogos de uma lista         |


