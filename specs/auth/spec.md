# Auth Spec

## Objetivo

Gerenciar autenticação, acesso, sessões e permissões iniciais dos usuários da plataforma.

---

# Funcionalidades

O sistema de autenticação deve permitir:

- cadastro de usuários
- login
- logout
- recuperação de senha
- gerenciamento de sessão
- definição de tipo de conta
- controle de acesso
- persistência de autenticação

---

# Tipos de Conta

Durante o cadastro o usuário deve escolher um tipo de conta:

- aluno
- professor

O cargo de mentor não pode ser escolhido durante cadastro.

Mentores são definidos posteriormente por professores dentro das turmas.

Administradores são definidos apenas pelo sistema.

---

# Cadastro

O sistema deve permitir:

- cadastro com nome
- email
- senha
- confirmação de senha
- escolha de tipo de conta

O sistema deve validar:
- email único
- senha mínima
- confirmação correta da senha

---

# Login

O sistema deve permitir autenticação utilizando:

- email
- senha

Após login:
- sessão deve ser criada
- permissões devem ser carregadas
- usuário deve ser redirecionado para dashboard

---

# Sessão

O sistema deve manter:

- usuário autenticado
- permissões carregadas
- persistência da sessão

A sessão pode ser encerrada por:
- logout manual
- expiração
- suspensão da conta por um administrador

---

# Recuperação de Senha

O sistema deve permitir:

- solicitação de recuperação
- redefinição de senha
- validação de token de recuperação

---

# Controle de Acesso

O sistema deve restringir funcionalidades com base no cargo do usuário.

Tipos de acesso:
- aluno
- mentor
- professor
- administrador

---


# Persistência de Login

O sistema deve manter login ativo entre sessões até:

- logout manual
- expiração da sessão
- revogação de acesso