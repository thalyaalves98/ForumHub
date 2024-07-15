# ForumHub - Challenge ONE (Back End)

## 📋 Descrição do Projeto

Este projeto é uma API REST desenvolvida com Spring Boot, que permite o gerenciamento de tópicos, incluindo funcionalidades de autenticação de usuários. Utiliza JWT para autenticação e segue as melhores práticas de segurança.

## ➕ Tecnologias Utilizadas

- **Java 17**
- **Spring Boot**
- **Spring Security**
- **JPA / Hibernate**
- **Banco de Dados**: MySQL
- **Lombok**

## ➕ Funcionalidades

- Registro e autenticação de usuários.
- Criação, listagem, atualização e exclusão de tópicos.
- Validação de dados de entrada.
- Retorno de informações detalhadas sobre os tópicos.

## 🛠 Instalação

1. **Clone o repositório**

   ```bash
   git clone https://github.com/thalyaalves98/ForumHub.git
   cd ForumHub

2. **Configure o Banco de Dados**

No arquivo src/main/resources/application.properties, adicione as configurações necessárias para o banco de dados. 

3. **Execute o Projeto**

   ```bash
   ./mvnw spring-boot:run

Utilize o comando acima para executar a aplicação.

## Gerando o Token JWT

Para gerar um token JWT, você deve primeiro autenticar um usuário. Siga os passos abaixo:

1. **Faça uma requisição POST para o endpoint `/login` com as credenciais do usuário:**

   - **URL**: `http://localhost:8080/login`
   - **Body**:
     ```json
     {
       "login": "seu_login",
       "senha": "sua_senha"
     }
     ```

2. **Resposta esperada:**
   Se a autenticação for bem-sucedida, você receberá um token JWT no formato:

   ```json
   {
     "token": "seu_token_jwt"
   }

## Testando a API

Utilize ferramentas como **Insomnia** ou **Postman** para testar a API de forma prática e intuitiva.

## Endpoints Principais

- **POST /login**: 
  - Autentica o usuário e retorna um token JWT.

- **POST /topicos**: 
  - Cria um novo tópico com os dados fornecidos.

- **GET /topicos**: 
  - Lista todos os tópicos disponíveis.

- **GET /topicos/{id}**: 
  - Retorna detalhes de um tópico específico, onde `{id}` é o identificador do tópico.

- **PUT /topicos/{id}**: 
  - Atualiza informações de um tópico existente, onde `{id}` é o identificador do tópico.

- **DELETE /topicos/{id}**: 
  - Deleta um tópico específico, onde `{id}` é o identificador do tópico.

## Licença

Este projeto está sob a **Licença MIT**. Veja o arquivo **LICENSE** para mais detalhes.

### Autor:
---

<a>
 <img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/u/145573026?v=4" width="100px;" alt=""/>
 <br />
 <sub><b>Thalya Alves</b></sub></a>


Desafio ☑️ por Thalya Alves 👋🏽 

[![Twitter Badge](https://img.shields.io/badge/-@talyalvs-1ca0f1?style=flat-square&labelColor=1ca0f1&logo=twitter&logoColor=white&link=https://twitter.com/talyalvs)](https://twitter.com/talyalvs) [![Linkedin Badge](https://img.shields.io/badge/-Thalya-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/thalya-alves/)](https://www.linkedin.com/in/thalya-alves/) 
[![Gmail Badge](https://img.shields.io/badge/-thalya.alvesg7@gmail.com-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:thalya.alvesg7@gmail.com)](mailto:thalya.alvesg7@gmail.com)
