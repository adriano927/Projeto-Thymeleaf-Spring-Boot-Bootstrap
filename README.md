# Projeto-Thymeleaf-Spring-Boot-Bootstrap
O Sistema de Cadastro de Alunos é uma aplicação web desenvolvida com Spring Boot, Thymeleaf e Bootstrap, seguindo o padrão MVC (Model–View–Controller).

Descrição do Projeto – Sistema de Cadastro de Alunos

O Sistema de Cadastro de Alunos é uma aplicação web desenvolvida com Spring Boot, Thymeleaf e Bootstrap, seguindo o padrão MVC (Model–View–Controller).
O objetivo é demonstrar na prática como criar um sistema completo de cadastro (CRUD) com validação, interface responsiva e persistência de dados em um banco relacional.

A aplicação permite:

 Listar todos os alunos cadastrados;

 Cadastrar novos alunos, com campos obrigatórios e validação de formulário;

 Editar informações já registradas;

 Excluir alunos do banco de dados.

Os dados são armazenados em um banco H2 (em memória) — ou seja, não é preciso instalar banco nenhum, e o projeto roda imediatamente após ser executado.
O layout foi desenvolvido com Bootstrap 5, garantindo uma interface simples, elegante e totalmente responsiva.

Tecnologias Utilizadas

Spring Boot 3.2

Spring Data JPA

Spring Web

Thymeleaf

Bootstrap 5

H2 Database

Validação com Jakarta Validation (Bean Validation)

Passos para Executar a Aplicação
 1. Pré-requisitos

Certifique-se de ter instalado:

Java 17 ou superior

Maven (ou use o Maven embutido do IntelliJ / VS Code)

 2. Importar o projeto

Extraia o arquivo aluno-project.zip.

Abra o IntelliJ IDEA ou VS Code.

Escolha “Open” ou “Import Project” e selecione a pasta aluno-project.

Aguarde o Maven baixar as dependências automaticamente.

3. Executar o projeto

Você tem duas opções:

Pelo terminal:

Na raiz do projeto, execute:
mvn spring-boot:run

Pelo IntelliJ / VS Code:

Abra o arquivo:
src/main/java/com/example/alunoapp/DemoApplication.java
e clique em Run

4. Acessar o sistema

Após a execução, abra o navegador e vá para:
http://localhost:8080/alunos
Lá você verá a lista de alunos e poderá:

Criar novos registros clicando em “Novo Aluno”;

Editar ou excluir registros existentes.

Banco de Dados

O sistema usa o H2 Database em memória, então os dados são apagados ao encerrar a aplicação.
Para visualizar as tabelas:
Acesse:
http://localhost:8080/h2-console

Use essas credenciais:

JDBC URL: jdbc:h2:mem:db

User: sa

Password: (deixe em branco)

Clique em Connect e veja as tabelas e dados.
Validação

Os formulários possuem validações automáticas:

Nome, e-mail, curso, matrícula e data de nascimento são obrigatórios.

E-mail deve ser válido.

Matrícula não pode ser duplicada.
