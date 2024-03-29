# Projeto de Teste Prático - Golang/Flutter

Este projeto é um teste prático para avaliar as habilidades de programação em Golang e Flutter. O backend foi desenvolvido utilizando o framework Gin para o servidor, Swaggo para a documentação e PostgreSQL como banco de dados. Já o frontend foi implementado em Flutter, utilizando MobX para gerenciamento de estado, Dio para consumo de API, e Clean Architecture em ambas as partes.

## Estrutura do Projeto

## Backend

### Requisitos

Na pasta `backend`, encontra-se toda a implementação da API desenvolvida em Golang. Abaixo estão as principais características da implementação:

- **Clean Architecture:** A estrutura do projeto segue os princípios da Clean Architecture, dividindo a aplicação em camadas independentes.

- **PostgreSQL:** O banco de dados utilizado é o PostgreSQL para armazenamento de dados relacionais.

- **Gin:** O framework Gin foi utilizado para roteamento HTTP.

#### Rotas

- `course/list`: Lista todos os cursos disponíveis.
- `course/create`: Cria um novo curso.
- `course/add-student`: Adiciona um aluno a um curso.
- `course/update`: Atualiza informações de um curso.
- `course/list-student`: Lista todos os alunos de um curso.
- `student/list`: Lista todos os alunos cadastrados.
- `student/create`: Cria um novo aluno.
- `student/update`: Atualiza informações de um aluno.
### Instruções para execução

1. Navegue até o diretório `backend`.

```bash cd backend```

Execute o seguinte comando para construir e iniciar o servidor utilizando o Docker Compose.

```bash docker-compose up --build```

Isso iniciará o backend, configurando o banco de dados PostgreSQL e expondo os endpoints através do framework Gin.

Documentação da API
A documentação da API pode ser acessada através do Swagger. Após iniciar o servidor, acesse:

http://localhost:8080/swagger/index.html

### Depois de rodar o backend e ja estiver configurado 

    - Entre na pasta workspace
```bash cd backend```

    - Inicie o frontend em modo release para melhor experiencia
```bash flutter run --release```


### Frontend

### Requisitos
 - Flutter
 - Visual Studio Code (ou IDE de sua escolha)

### Instruções para execução
 - Navegue até o diretório frontend/workspace.
 ```bash cd frontend/workspace```

    - Inicie o frontend em modo release para melhor experiencia
```bash flutter run --release```

Isso iniciará o frontend, onde você poderá interagir com a aplicação desenvolvida. O MobX será responsável pelo gerenciamento de estado, e o Dio será utilizado para consumir a API do backend.

### Clean Architecture

O projeto foi estruturado seguindo os princípios da Clean Architecture tanto no backend quanto no frontend. Isso proporciona uma separação clara de responsabilidades, facilitando a manutenção e testabilidade do código.

 - Observação: Certifique-se de que todos os requisitos estão instalados corretamente antes de executar o projeto. Boa sorte no teste prático!