# lab-instancia-de-banco
📌 O que é uma Instância Gerenciada de SQL?
É um serviço de banco de dados gerenciado do Azure que oferece as funcionalidades do SQL Server com os benefícios da nuvem (alta disponibilidade, backups automáticos, etc.).

🧰 Pré-requisitos
Antes de começar, você precisa:

Ter uma assinatura ativa no Azure (ou criar uma gratuita).

Instalar o módulo Az.SQL no PowerShell ou usar a CLI do Azure (linha de comando).

🛠️ Como criar a Instância via Portal do Azure
Acessar o portal do Azure: https://portal.azure.com

No menu esquerdo, ir em SQL do Azure > Criar > Instâncias Gerenciadas de SQL

Escolher "Instância única" e clicar em Criar

🧾 Etapas do formulário de criação (várias abas)
🟦 Aba “Básico”
Preencha dados essenciais:

Assinatura e grupo de recursos

Nome da instância

Região

Autenticação (usar SQL Server)

Nome e senha do administrador

⚙️ Aba “Computação + Armazenamento”
Escolha o tipo de serviço: Uso Geral (mais comum)

Geração de hardware: Gen5 (padrão)

Defina:

vCores (poder de processamento)

Armazenamento em GB

Tipo de licença (ex: Benefício Híbrido do Azure)

🌐 Aba “Rede”
Criar ou usar uma rede virtual (VNet)

Tipo de conexão

Habilitar ou não ponto de extremidade público (acesso pela internet)

🔐 Aba “Segurança”
Pode manter as configurações padrão para início rápido

➕ Aba “Configurações adicionais”
Defina ordenação (Collation)

Fuso horário

Janela de manutenção

Se deseja replicação geográfica

🏷️ Aba “Marcas (tags)”
Adicione etiquetas para facilitar organização e rastreamento de custos (ex: "Ambiente = Produção")

✅ Finalizar criação
Clique em Revisar + Criar

Confirme os dados e clique em Criar

🔍 Após a criação
Acompanhe o progresso na aba de notificações do portal

Acesse o grupo de recursos para ver:

Tabela de rotas

Grupo de segurança de rede

🗄️ Criar um banco de dados na instância
Vá até a instância criada

Clique em + Novo banco de dados

Dê um nome, configure se será vazio ou baseado em backup

Clique em Criar

🔌 Conectar à instância
Pegue o FQDN (nome de domínio completo) na aba Visão Geral da instância

Use esse nome para se conectar via SQL Server Management Studio, Azure Data Studio, etc.

🔄 Outras funcionalidades
Restaurar backup de um SQL Server local

Conectar aplicativos à instância

Monitorar via ferramentas como Database Watcher
