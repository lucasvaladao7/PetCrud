# 🐾 PetCrud - Cadastro de Animais

Sistema desenvolvido em **ASP.NET Core MVC** para realizar o cadastro e gerenciamento de animais domésticos. O projeto permite cadastrar, visualizar, editar e excluir registros de animais contendo **Nome, Idade e Raça**, utilizando uma arquitetura MVC e banco de dados SQL Server.

## 📸 Demonstração

### Tela Principal

![Lista de Animais](PetCrud/Imagens/lista.png)

### Tela de Cadastro

![Cadastro de Animal](PetCrud/Imagens/cadastro.png)

> **Obs.:** Coloque as capturas de tela na pasta `imagens` do projeto e renomeie para `lista.png` e `cadastro.png`.

---

# ✨ Funcionalidades

- ✅ Cadastro de animais
- ✅ Listagem de animais
- ✅ Visualização das informações
- ✅ Edição de registros
- ✅ Exclusão de animais
- ✅ Interface responsiva com Bootstrap
- ✅ Pesquisa, ordenação e paginação utilizando DataTables

---

# 🛠 Tecnologias Utilizadas

| Tecnologia | Descrição |
|------------|-----------|
| ASP.NET Core MVC | Arquitetura da aplicação |
| C# | Linguagem principal |
| Entity Framework Core | ORM para acesso ao banco de dados |
| SQL Server | Banco de dados |
| Bootstrap | Interface responsiva |
| jQuery | Manipulação da interface |
| DataTables | Pesquisa, paginação e ordenação |

---

# 📁 Estrutura do Projeto

```
PetCrud
│
├── Controllers
├── Models
├── Views
├── Data
├── wwwroot
│   ├── css
│   ├── js
│   └── lib
├── appsettings.json
└── Program.cs
```

---

# 📌 Modelo da Entidade

```csharp
public class Animal
{
    public int Id { get; set; }

    public string Nome { get; set; }

    public int Idade { get; set; }

    public string Raca { get; set; }
}
```

---

# 🚀 Como executar o projeto

### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/PetCrud.git
```

### 2. Abra o projeto

Abra a solução utilizando o **Visual Studio 2022**.

### 3. Configure a conexão com o banco

No arquivo:

```json
appsettings.json
```

Configure sua string de conexão com o SQL Server.

Exemplo:

```json
"ConnectionStrings": {
  "DefaultConnection": "Server=SEU_SERVIDOR;Database=PetCrud;Trusted_Connection=True;TrustServerCertificate=True;"
}
```

### 4. Execute as migrations

```bash
Update-Database
```

ou

```bash
dotnet ef database update
```

### 5. Execute a aplicação

Pressione **F5** ou execute:

```bash
dotnet run
```

---

# 📚 Operações CRUD

O sistema possui todas as operações básicas de CRUD:

- ➕ Create (Cadastrar)
- 📄 Read (Listar e Visualizar)
- ✏️ Update (Editar)
- 🗑 Delete (Excluir)

---

# 🎯 Objetivo

Este projeto foi desenvolvido com fins acadêmicos para praticar os conceitos de:

- ASP.NET Core MVC
- Entity Framework Core
- CRUD
- SQL Server
- Bootstrap
- Organização em camadas
- Padrão MVC
- Boas práticas de desenvolvimento

---

# 👨‍💻 Autor

**David Oliveira da Silva**

Estudante do curso Técnico em Desenvolvimento de Sistemas - SENAI/SE

GitHub:
https://github.com/davidosilva9-hub/HospitalCrud.git

---

## 📄 Licença

Este projeto foi desenvolvido para fins de estudo e aprendizado.
