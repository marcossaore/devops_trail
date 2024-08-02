# AWS Credentials Report

## O que é o AWS Credentials Report?

O AWS Credentials Report é uma ferramenta que permite aos administradores da AWS visualizar e auditar as credenciais de segurança (como senhas e chaves de acesso) associadas a todos os usuários do IAM (Identity and Access Management) em uma conta da AWS. Esse relatório é essencial para manter boas práticas de segurança e conformidade, permitindo identificar usuários com credenciais desatualizadas ou comprometidas.

## Funcionalidades Principais

1. **Relatório Detalhado de Credenciais:**
   - Fornece informações sobre senhas, chaves de acesso e certificados de cada usuário do IAM.
   - Inclui detalhes como a data de criação das credenciais, última vez que foram usadas, e se estão ativas ou não.

2. **Segurança e Conformidade:**
   - Ajuda a garantir que as políticas de segurança sejam seguidas, como a rotação de chaves de acesso e a expiração de senhas.
   - Permite identificar rapidamente credenciais que não estão sendo usadas ou que não foram alteradas em muito tempo, o que pode indicar um risco de segurança.

3. **Facilidade de Acesso:**
   - O relatório pode ser gerado e baixado através do Console de Gerenciamento da AWS, AWS CLI, ou SDKs da AWS.
   - Gera um arquivo CSV que pode ser facilmente visualizado e analisado.

## Como Gerar o AWS Credentials Report

### Via Console de Gerenciamento da AWS

1. Acesse o console da AWS e vá para o IAM.
2. No painel de navegação, clique em "Reports".
3. Selecione "Download" ao lado de "Credentials Report" para gerar e baixar o relatório.

### Via AWS CLI

Use o seguinte comando para gerar e baixar o relatório:

```bash
aws iam generate-credential-report
aws iam get-credential-report
```

<br/>
<hr></hr>

# AWS IAM Access Advisor

## O que é o IAM Access Advisor?

O IAM Access Advisor é uma ferramenta no AWS Identity and Access Management (IAM) que ajuda a administrar e revisar as permissões dos usuários e funções. Ele fornece informações sobre quais serviços da AWS foram acessados por um usuário ou função e a última vez que esses serviços foram usados. Isso é útil para identificar e ajustar permissões excessivas, ajudando a manter uma postura de segurança mínima necessária.

## Principais Funcionalidades

1. **Histórico de Uso de Serviços:**
   - Exibe uma lista de serviços da AWS acessados por um usuário ou função, incluindo a data do último acesso.
   - Ajuda a determinar quais permissões podem ser removidas com segurança, caso não sejam usadas.

2. **Otimização de Permissões:**
   - Facilita a revisão e ajuste de políticas de IAM para garantir que os usuários e funções possuam apenas as permissões necessárias.

3. **Auditoria de Segurança:**
   - Auxilia na auditoria de segurança, garantindo que as políticas de permissões estejam alinhadas com os princípios de segurança de mínimo privilégio.

## Mini Tutorial

### Como Usar o IAM Access Advisor

#### Passo 1: Acessar o IAM Access Advisor

1. **Acesse o Console de Gerenciamento da AWS:**
   - Navegue até o [AWS Management Console](https://aws.amazon.com/console/).

2. **Vá para o IAM:**
   - No console, selecione o serviço IAM.

3. **Selecione um Usuário ou Função:**
   - No painel de navegação, escolha "Users" para selecionar um usuário ou "Roles" para selecionar uma função.

#### Passo 2: Visualizar o Uso de Serviços

1. **Acesse a Guia "Access Advisor":**
   - Dentro do perfil do usuário ou da função, clique na guia "Access Advisor".

2. **Analisar o Histórico de Uso:**
   - Revise a lista de serviços e a última vez que cada serviço foi acessado. O Access Advisor mostrará:
     - Nome do serviço.
     - Última data de acesso.
     - Status de uso (se ativo ou não).

#### Passo 3: Ajustar Permissões

1. **Identificar Permissões Não Utilizadas:**
   - Identifique serviços que não foram acessados recentemente ou nunca foram utilizados.

2. **Modificar Políticas de IAM:**
   - Baseado nas informações do Access Advisor, ajuste as políticas de IAM para remover permissões desnecessárias. Isso pode ser feito diretamente na guia "Permissions" do usuário ou função.

3. **Salvar Alterações:**
   - Após revisar e ajustar as permissões, salve as mudanças para aplicar as novas configurações de segurança.

## Conclusão

O IAM Access Advisor é uma ferramenta valiosa para revisar e otimizar permissões de usuários e funções na AWS. Ele fornece uma visão clara do uso de serviços, ajudando a garantir que as permissões estejam alinhadas com as necessidades reais, minimizando riscos de segurança.
