# 📋 Sistema de Tarefas API

<p align="center">
  <img src="https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white" />
  <img src="https://img.shields.io/badge/.NET%206-512BD4?style=for-the-badge&logo=dotnet&logoColor=white" />
  <img src="https://img.shields.io/badge/SQL%20Server-CC2927?style=for-the-badge&logo=microsoft-sql-server&logoColor=white" />
  <img src="https://img.shields.io/badge/Entity%20Framework-512BD4?style=for-the-badge&logo=dotnet&logoColor=white" />
</p>

> **API RESTful para gerenciamento de tarefas e usuários**, desenvolvida com foco em arquitetura limpa e padrões de projeto essenciais para escalabilidade.

---

## 🚀 Sobre o Projeto

Este projeto é uma Web API completa construída com **ASP.NET Core**. Ele permite o gerenciamento de um fluxo de trabalho, onde é possível cadastrar usuários e atribuir tarefas a eles, controlando o status de cada atividade.

### Principais Funcionalidades:
- **Gestão de Usuários:** CRUD completo de usuários do sistema.
- **Gestão de Tarefas:** Criação, edição, consulta e exclusão de tarefas.
- **Vínculo Dinâmico:** Atribuição de tarefas a usuários específicos.
- **Persistência de Dados:** Uso de Migrations para versionamento do banco de dados SQL Server.
- **Documentação:** Interface interativa via Swagger para testes de endpoints.

---

## 🛠️ Tecnologias e Padrões

- **Backend:** C# com ASP.NET Core 6.0
- **ORM:** Entity Framework Core (Code First)
- **Banco de Dados:** Microsoft SQL Server
- **Padrões de Projeto:** - **Repository Pattern:** Para abstração da camada de dados e facilitar testes unitários.
  - **Dependency Injection:** Nativa do .NET para desacoplamento de classes.
  - **Fluent API:** Utilizada na pasta `Maps` para configurações refinadas do banco de dados.

---

## 📂 Estrutura do Projeto

- `Controllers/`: Endpoints da API e controle de fluxo.
- `Models/`: Classes de entidade que representam as tabelas do banco.
- `Repositorios/`: Implementação da lógica de acesso a dados (Interfaces e Classes).
- `Data/`: Contexto do banco de dados e configuração das Migrations.
- `Maps/`: Configurações de mapeamento objeto-relacional (Entity Configuration).

---

## ✨ Como Executar o Projeto

### 1. Clone o repositório

```bash
git clone https://github.com/Maruka13/SistemaDeTarefas.git
```

---

### 2. Configure o Banco de Dados

No arquivo `appsettings.json`, ajuste a `ConnectionStrings` para o seu SQL Server local.

Exemplo:

```json
"ConnectionStrings": {
"DefaultConnection": "Server=.;Database=DB_SistemaTarefas;User Id=sa;Password=SuaSenhaAqui;"
}
```

---

### 3. Execute as Migrations

No Console do Gerenciador de Pacotes ou via CLI:

```bash
dotnet ef database update
```

---

### 4. Inicie a aplicação

```bash
dotnet run
```

---

### 📄 Documentação

Acesse no navegador:

```
[https://localhost:7xxx/swagger](https://localhost:7xxx/swagger)
```

---

## 🤝 Contato

Desenvolvido por **Emanuelle Gomes**
*Aplicando engenharia de software e persistência em cada linha de código.*

<div align="center">
  <a href="https://www.linkedin.com/in/manugomesdev/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
</div>
