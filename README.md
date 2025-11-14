🚀 Global Solution 2025 - API "Projetos com Propósito"
📝 Descrição do Projeto
Esta é uma API RESTful desenvolvida em .NET 9 como solução para o desafio da Global Solution (FIAP), com o tema "O Futuro do Trabalho".

A solução simula o backend de uma plataforma tecnológica que visa conectar talentos (usuários) a projetos com propósito (alinhados a causas sociais ou ambientais).

O projeto ataca diretamente os desafios do briefing, conectando o valor humano à tecnologia e alinhando-se diretamente às ODS (Objetivos de Desenvolvimento Sustentável) da ONU:

ODS 8 (Trabalho Decente e Crescimento Econômico): Foco em criar oportunidades de trabalho com mais significado.

ODS 9 (Indústria, Inovação e Infraestrutura): Uso de uma API .NET como infraestrutura inovadora para o mercado de trabalho.

ODS 10 (Redução das Desigualdades): Democratização do acesso a projetos de impacto.

-----

🛠️ Tecnologias Utilizadas
.NET 9 (Framework para a API RESTful)

Entity Framework Core 9 (ORM para comunicação com o banco)

Oracle Database (Banco de dados relacional)

Swagger (OpenAPI) (Documentação interativa da API)

-----

✅ Checklist de Requisitos
Este projeto cumpre todos os requisitos técnicos da avaliação:

[x] API RESTful .NET 9 (Tema: Futuro do Trabalho)

[x] Status Codes HTTP adequados (200, 201, 204, 400, 404, etc.)

[x] Uso correto dos Verbos HTTP (GET, POST, PUT, DELETE)

[x] Versionamento da API (Todos os endpoints estão em /api/v1)

[x] Integração com Banco de Dados Oracle

[x] Uso de Entity Framework Core com Migrations

[x] Documentação interativa com Swagger

[x] Diagrama de Arquitetura (abaixo)

-----

🏛️ Diagrama de Arquitetura
O fluxo da solução segue uma arquitetura de 3 camadas simples e robusta:


<img width="1145" height="135" alt="diagrama_csharp" src="https://github.com/user-attachments/assets/6a68a53b-ce71-479c-b0b0-831ce132372c" />


(Para colar no GitHub, suba o PNG para o repositório e arraste-o para o README.md)

-----

⚙️ Como Executar (Instruções para Acesso e Testes)
Este projeto foi desenvolvido para ser executado localmente. Não há deploy público (Cloud) nesta versão.

1. Pré-requisitos
.NET 9 SDK

Um servidor de Banco de Dados Oracle (Ex: Oracle XE) acessível.

Visual Studio 2022 (ou VS Code).

2. Configuração do Banco de Dados
Clone este repositório:

Bash

git clone gs_csharp
Abra o arquivo appsettings.json.

Localize a ConnectionStrings e altere os valores (User Id, Password, Data Source) para os do seu banco Oracle.

JSON

"ConnectionStrings": {
  "DefaultConnection": "User Id=SEU_USUARIO;Password=SUA_SENHA;Data Source=SEU_DATA_SOURCE;"
}
3. Executando as Migrations
Com o banco configurado, aplique as migrations para criar as tabelas:

Abra o "Console do Gerenciador de Pacotes" no Visual Studio.

Execute o comando:

PowerShell

Update-Database
4. Executando a API
Pressione F5 ou clique no botão de "Play" (ProjetosComPropositoAPI) no Visual Studio.

Um console (tela preta) irá aparecer indicando que o servidor está rodando.

5. Testando no Swagger
O navegador será iniciado. Se não, abra-o manualmente e acesse a URL indicada no console (geralmente https://localhost:7024/swagger).

A documentação do Swagger será exibida, pronta para os testes.

Fluxo de Teste Recomendado:
POST /api/v1/Projetos: Crie um novo projeto.

POST /api/v1/Usuarios: Crie um novo usuário.

POST /api/v1/Candidaturas: Crie uma candidatura usando o projetoId e o usuarioId criados nos passos anteriores.

GET /api/v1/Projetos/{id}: Consulte o projeto criado no passo 1 (usando o ID dele) e verifique se a candidatura aparece na lista candidaturas.

PUT /api/v1/Projetos/{id}: Teste a atualização do projeto.

DELETE /api/v1/Projetos/{id}: Teste a exclusão do projeto.

-----

👨‍💻 Autores
Pedro henrique menezes mariano silva | RM97432
Victoria Franceschini Pizza | RM550609

Turma: 3ESPX
