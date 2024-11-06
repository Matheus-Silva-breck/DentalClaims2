# **Dental Claims - Sistema de Agendamento de Consultas**

## Descrição

O **Dental Claims** é um sistema desenvolvido para gerenciar agendamentos de consultas odontológicas, facilitando o processo de agendamento e controle de dados dos pacientes e procedimentos realizados. O sistema permite o registro de pacientes, datas dos agendamentos e procedimentos realizados, garantindo uma visão clara e eficiente dos atendimentos.

Este projeto foi desenvolvido com **.NET Core**, **Oracle** como banco de dados e **Entity Framework Core** para a interação com o banco de dados.

---

## **Tecnologias Utilizadas**

- **Backend**:
  - [.NET Core](https://dotnet.microsoft.com/en-us/learn/dotnet/what-is-dotnet) (C#)
  - [Entity Framework Core](https://docs.microsoft.com/en-us/ef/core/) para mapeamento objeto-relacional (ORM)
  - [Oracle Database](https://www.oracle.com/database/)
  
- **Frontend**:
  - **MVC (Model-View-Controller)** com **Razor Pages**
  - **HTML**, **CSS**, **JavaScript** para a construção das páginas

---

## **Funcionalidades**

- **Cadastro de Pacientes**: Registrar informações sobre pacientes, como nome, data de nascimento e contato.
- **Agendamento de Consultas**: Agendar consultas com informações como data, hora e procedimento.
- **Gerenciamento de Procedimentos**: Registrar e atualizar os procedimentos realizados durante a consulta.
- **Visualização de Agendamentos**: Visualizar todos os agendamentos realizados, com filtros por data e paciente.

---

## **Estrutura do Projeto**

O projeto está organizado em diversas pastas e arquivos para melhor manutenção e escalabilidade. A estrutura básica do projeto é a seguinte:


---

## **Configuração e Instalação**

1. **Clone o repositório**
   Clone o repositório do projeto para a sua máquina local:
   
    git clone https://github.com/SeuUsuario/DentalClaims.git
    cd DentalClaims

2. **Instale as dependências**
  Execute o comando para restaurar os pacotes do projeto:

    dotnet restore

3. **Configure o banco de dados**
  Abra o arquivo appsettings.json e configure a connection string com as credenciais do seu banco de dados Oracle:

    "ConnectionStrings": {
    "DefaultConnection": "User Id=seu_usuario;Password=sua_senha;Data Source=(DESCRIPTION=(ADDRESS_LIST=(ADDRESS=(PROTOCOL=TCP)(HOST=oracle.fiap.com.br)(PORT=1521)))(CONNECT_DATA=(SERVER=DEDICATED)(SID=ORCL)));"
}

4. **Crie o banco de dados e as tabelas**
  Com o banco de dados configurado, execute os seguintes comandos para aplicar as migrações e criar as tabelas no banco:

    dotnet ef migrations add InitialCreate
    dotnet ef database update

Se você estiver usando Oracle, verifique se as permissões de banco estão configuradas corretamente para a criação de objetos no banco.

## Rodando a Aplicação
**Depois de configurar o banco de dados e as dependências, execute o projeto com o seguinte comando:**
  dotnet run

**A aplicação estará disponível em http://localhost:5000.**

## Licença
**Este projeto está licenciado sob a MIT License - veja o arquivo LICENSE para mais detalhes.**

## Integrantes do grupo
- **Nome: Eduardo Rodrigues Shiraga**
- **RM: 553705**
- **Nome: Giovani Shiraishi Borba**
- **RM: 553724**
- **Nome: Matheus Rodrigo da Silva **
- **RM: 553180**
