![futuristic_robot_200x200](https://github.com/user-attachments/assets/041f001c-9917-46e1-a682-06448c6ae6de)

```md
# Megaman API

Bem-vindo ao **Megaman API**, um backend desenvolvido em **.NET Core 3.1** que fornece informações sobre os bosses da franquia **Megaman**. A API retorna dados no formato JSON, permitindo fácil integração com outras aplicações.

## 📌 Exemplo de Resposta

```json
{
  "Id": 1,
  "Code": "DLN/DRN-003",
  "Name": "Cutman",
  "HP": 150,
  "Picture": "https://vignette.wikia.nocookie.net/megaman/images/2/22/Cutman.png"
}
```

---

## 📦 Tecnologias Utilizadas

Esta API foi desenvolvida utilizando as seguintes tecnologias e práticas:

- **.NET Core 3.1** - Framework principal para desenvolvimento da API.
- **Entity Framework Core** - ORM para manipulação do banco de dados.
- **SQL Server** - Banco de dados utilizado na aplicação.
- **Newtonsoft.Json** - Biblioteca para manipulação de JSON.
- Arquitetura baseada em **Controller-Service-Repository**.
- Uso de **Middlewares** para controle de requisições.
- Princípios de **RESTful APIs**.

---

## 🔧 Estrutura do Projeto

```bash
MegamanApi/
│── .vs/                         # Configurações do Visual Studio
│── .vscode/                     # Configurações do VS Code
│── bin/                         # Arquivos binários gerados pelo build
│── Controllers/                  # Contém os controllers da API
│── Database/                     # Scripts e configurações do banco de dados
│── middlewares/                   # Middlewares customizados da API
│── Models/                        # Modelos de entidades do banco de dados
│── obj/                           # Arquivos temporários gerados pelo .NET
│── Properties/                    # Configurações adicionais
│── Services/                      # Camada de serviços para regras de negócio
│── appsettings.Development.json    # Configurações para ambiente de desenvolvimento
│── appsettings.json                # Configurações principais da aplicação
│── global.json                     # Arquivo de configuração global
│── MegamanApi.csproj                # Arquivo do projeto
│── MegamanApi.sln                   # Solution do projeto
│── Program.cs                       # Arquivo principal da aplicação
│── Startup.cs                        # Configuração de serviços e middlewares
```

---

## 📜 Normas Técnicas Utilizadas

O projeto segue algumas normas técnicas e boas práticas no desenvolvimento:

- **RESTful API**: Estruturação seguindo os princípios REST.
- **SOLID**: Princípios para um código modular e de fácil manutenção.
- **Clean Code**: Código legível e organizado.
- **Entity Framework Code-First**: Uso do EF Core para modelagem do banco de dados.
- **Dependency Injection**: Injeção de dependências para melhor escalabilidade.
- **Swagger** (futuramente) para documentação interativa da API.

---

## 📌 Endpoints

| Método | Rota                     | Descrição |
|--------|--------------------------|------------|
| `GET`  | `/api/v1/robots`         | Retorna a lista de todos os robots. |
| `GET`  | `/api/v1/robots/{id}`    | Retorna um robot específico pelo ID. |
| `POST` | `/api/v1/robots`         | Cria um novo robot (em construção). |

---

## 📦 Dependências

| Dependência | Descrição |
|------------|-------------|
| [.NET Core 3.1](https://dotnet.microsoft.com/en-us/download/dotnet/3.1) | Framework utilizado para desenvolvimento da API |
| [Entity Framework Core](https://learn.microsoft.com/pt-br/ef/core/) | ORM para comunicação com banco de dados |
| [Entity Framework Core Design](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.Design/3.1.8) | Ferramentas para design e migração do EF Core |
| [Entity Framework Core SQL Server](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.SqlServer/3.1.8) | Provider do SQL Server para o EF Core |
| [Newtonsoft.Json](https://www.newtonsoft.com/json) | Biblioteca para manipulação de JSON |

---

## 🏁 Como Rodar o Projeto

1. Clone este repositório:
   ```bash
   git clone https://github.com/seuusuario/megaman-api.git
   ```
2. Acesse a pasta do projeto:
   ```bash
   cd megaman-api
   ```
3. Instale as dependências do projeto:
   ```bash
   dotnet restore
   ```
4. Configure o banco de dados no `appsettings.json`.
5. Execute a API:
   ```bash
   dotnet run
   ```

---

## 📄 Licença

Este projeto está sob a licença **MIT**. Sinta-se livre para usá-lo e modificá-lo.

---

🚀 **Megaman API** - Desenvolvido com 💙 para os fãs de Megaman!
```
