# AWS Identity and Access Management (IAM)

AWS Identity and Access Management (IAM) é um serviço da AWS que permite gerenciar de forma segura o acesso aos serviços e recursos da AWS. Este guia fornece uma introdução aos conceitos principais do IAM e um tutorial passo a passo para configuração inicial.

## Índice
- [Componentes Principais do IAM](#componentes-principais-do-iam)
- [Tutorial: Como Utilizar o IAM](#tutorial-como-utilizar-o-iam)
  - [Passo 1: Acessar o Console do IAM](#passo-1-acessar-o-console-do-iam)
  - [Passo 2: Criar um Usuário IAM](#passo-2-criar-um-usuário-iam)
  - [Passo 3: Atribuir Permissões](#passo-3-atribuir-permissões)
  - [Passo 4: Revisar e Criar o Usuário](#passo-4-revisar-e-criar-o-usuário)
  - [Passo 5: Configurar Política de Senha](#passo-5-configurar-política-de-senha)
  - [Passo 6: Gerenciar Funções (Roles)](#passo-6-gerenciar-funções-roles)
- [Práticas Recomendadas](#práticas-recomendadas)

## Componentes Principais do IAM

1. **Usuários:** Representam uma pessoa ou aplicação que interage com os serviços da AWS. Cada usuário possui um conjunto de credenciais.
2. **Grupos:** Conjuntos de usuários para gerenciamento simplificado de permissões.
3. **Políticas:** Definem permissões, especificando o que usuários, grupos ou funções podem ou não podem fazer.
4. **Funções (Roles):** Permitem atribuir permissões a entidades confiáveis, como serviços da AWS ou usuários externos.
5. **Política de Senha:** Regras para criação de senhas fortes.

## Tutorial: Como Utilizar o IAM

### Passo 1: Acessar o Console do IAM

1. Faça login no [Console de Gerenciamento da AWS](https://aws.amazon.com/console/).
2. No menu de serviços, selecione **IAM**.

### Passo 2: Criar um Usuário IAM

1. No painel de navegação, clique em **Users** (Usuários).
2. Clique em **Add user** (Adicionar usuário).
3. Insira um nome de usuário.
4. Selecione o tipo de acesso:
   - **Acesso programático**: Gera uma chave de acesso e um segredo de acesso para APIs, SDKs e CLI.
   - **Acesso ao Console da AWS**: Cria uma senha para login no console da AWS.
5. Clique em **Next: Permissions** (Próximo: Permissões).

### Passo 3: Atribuir Permissões

1. Escolha como atribuir permissões ao usuário:
   - **Adicionar usuário a um grupo**: Adicione o usuário a um grupo existente com políticas definidas.
   - **Anexar políticas diretamente**: Selecione políticas específicas para o usuário.
   - **Copiar permissões de um usuário existente**: Copie permissões de outro usuário.

2. Clique em **Next: Tags** (Próximo: Tags).

### Passo 4: Revisar e Criar o Usuário

1. Adicione tags (opcional).
2. Revise as informações e clique em **Create user** (Criar usuário).
3. Forneça a senha temporária para usuários com acesso ao console.

### Passo 5: Configurar Política de Senha

1. No painel de navegação, clique em **Account settings** (Configurações da conta).
2. Em **Password policy** (Política de senha), configure as regras de senha.
3. Clique em **Apply password policy** (Aplicar política de senha).

### Passo 6: Gerenciar Funções (Roles)

1. No painel de navegação, clique em **Roles** (Funções).
2. Clique em **Create role** (Criar função).
3. Escolha a entidade confiável (serviço da AWS, conta da AWS, etc.).
4. Siga as instruções para selecionar permissões e definir tags.
5. Revise e crie a função.

## Práticas Recomendadas

1. **Uso de Políticas de Menor Privilégio:** Conceda apenas as permissões necessárias.
2. **Uso de MFA (Autenticação Multifator):** Habilite MFA para segurança adicional.
3. **Rotação de Credenciais:** Altere regularmente as credenciais de segurança.

---

Este guia fornece uma introdução ao uso básico do IAM. Para informações mais detalhadas, consulte a [Documentação Oficial da AWS](https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html).


## Relacionado à AWS Identity and Access Management (IAM)
   - [AWS Organizations](./aws-organizations.md)
   - [Aws Identity Center](./aws-identity-center.md)
   - [Aws Credential Report e Aws Access Advasory ](./aws-credential-report.md)
