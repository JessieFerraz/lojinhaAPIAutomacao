# Lojinha API Automação

Esse é um repositório que contém a automação de alguns testes de API Rest de um software denominado Lojinha. Os subtópicos abaixo descrevem algumas decisões tomadas na estruturação do projeto.

## Tecnologias Utilizadas
- Java
  [Java Downloads | Oracle](https://www.oracle.com/java/technologies/downloads/#jdk21-windows)
- JUnit
  [Maven Repository: org.junit.jupiter » junit-jupiter-api » 5.8.0-M1 (mvnrepository.com)](https://mvnrepository.com/artifact/org.junit.jupiter/junit-jupiter-api/5.8.0-M1)
- RestAssured
  [Maven Repository: io.rest-assured » rest-assured » 4.4.0 (mvnrepository.com)](https://mvnrepository.com/artifact/io.rest-assured/rest-assured/4.4.0)
- Maven
  [Maven – Welcome to Apache Maven](https://maven.apache.org/)

## Testes Automatizados
Testes para validar as Partições de Equivalência relacionadas ao valor do produto na Lojinha, que estão diretamente vinculados à Regra de Negócio que diz que o valor do produto deve estar entre R$ 0,01 e R$ 7.000,00.

## Notas Gerais
- Utilização da anotação Before Each para capturar o token que será utilizado posteriormente nos métodos de teste.
- Armazenamento dos dados que são enviados para a API através do uso de classes POJO.
-  Criação de dados iniciais através do uso de classes Data Factory, para facilitar a criação e controle dos mesmos.
- Utilização do JUnit5, o que dá a possibilidade de usar a anotação DisplayName para dar descrições em português para o teste.