# Configurando uma Instância de Banco de Dados no Microsoft Azure

Este guia descreve os passos para configurar uma instância de banco de dados no Azure utilizando o serviço **Azure SQL Database**. 

## Pré-requisitos

Antes de começar, certifique-se de que você tem:

- Uma conta ativa no [Microsoft Azure](https://azure.microsoft.com/).
- Acesso ao [Portal do Azure](https://portal.azure.com/).

## Passo a Passo

### 1. Acesse o Portal do Azure
- Acesse [portal.azure.com](https://portal.azure.com) e faça login com suas credenciais.

### 2. Inicie a Criação do Banco de Dados
- No menu à esquerda, clique em **"Criar um recurso"**.
- Na barra de pesquisa, digite **"SQL Database"** e selecione a opção **"SQL Database"**.
- Clique em **"Criar"** para iniciar o processo de configuração.

### 3. Configuração Básica do Banco de Dados
- **Assinatura:** Selecione a assinatura correta.
- **Grupo de Recursos:** Escolha um grupo de recursos existente ou crie um novo.
- **Nome do Banco de Dados:** Insira o nome desejado para o banco de dados.
- **Servidor:** 
  - Selecione um servidor existente ou clique em **"Criar novo"**.
  - Se criar um novo servidor, defina:
    - **Nome do Servidor**
    - **Login de Administrador do Servidor**
    - **Senha e Confirmação de Senha**
    - **Localização (Região)**
- **Modo de Compra:** Escolha entre o modelo **Provisão** (DTU-based) ou **VCore** (compute and storage-based).
- **Objetivo de Serviço:** Selecione o tipo de serviço baseado nas necessidades de desempenho (Basic, Standard, Premium para DTU; General Purpose, Business Critical, Hyperscale para VCore).

### 4. Configurações de Rede
- **Método de Conexão:** Selecione se o banco de dados deve ser acessível via rede pública ou privada.
- **Regras de Firewall:** Configure as regras de firewall para permitir o acesso ao servidor:
  - Permitir serviços do Azure e recursos a acessar este servidor.
  - Adicionar IP do cliente atual para acessar o banco de dados.

### 5. Configurações Adicionais (Opcional)
- **Fonte de Dados:** Você pode optar por começar com um banco de dados vazio ou utilizar uma base de dados existente para restaurar (backup, banco de dados de exemplo).
- **Recursos Avançados:** Configurações como Auditoria, Backup Automático, e Geo-Redundância podem ser configuradas aqui.

### 6. Revisar e Criar
- Revise todas as configurações na aba **"Revisar e criar"**.
- Clique em **"Criar"** para iniciar a implantação do banco de dados.

### 7. Conectar-se ao Banco de Dados
- Após a implantação, vá até **"SQL Databases"** no menu esquerdo.
- Selecione seu banco de dados e clique em **"Mostrar Cadeia de Conexão"** para obter as informações necessárias para conexão.
- Utilize o **SQL Server Management Studio (SSMS)** ou outra ferramenta de sua preferência para se conectar ao banco de dados usando as credenciais e a cadeia de conexão fornecidas.

## Conclusão

Você configurou com sucesso uma instância de banco de dados no Azure! Agora você pode começar a criar, gerenciar e escalar seu banco de dados conforme necessário.

## Recursos Adicionais

- [Documentação Oficial do Azure SQL Database](https://docs.microsoft.com/azure/sql-database/)
- [Treinamento Gratuito no Microsoft Learn](https://learn.microsoft.com/training/)
- [SQL Server Management Studio (SSMS) - Download](https://docs.microsoft.com/sql/ssms/download-sql-server-management-studio-ssms)

