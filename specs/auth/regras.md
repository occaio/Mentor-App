# Auth Regras

## Cadastro

- email deve ser único
- email deve possuir formato válido
- senha deve possuir mínimo de 8 caracteres
- senha deve possuir ao menos 1 número
- senha deve possuir ao menos uma letra
- senha deve possuir confirmação
- confirmação de senha deve ser idêntica à senha
- tipo de conta é obrigatório
- apenas aluno e professor podem ser escolhidos durante cadastro

---

## Login

- login deve utilizar email e senha
- credenciais inválidas devem impedir autenticação
- usuários suspensos não podem realizar login
- sessão só deve ser criada após autenticação válida

---

## Sessão

- sessão deve possuir usuário autenticado
- sessão deve armazenar permissões do usuário
- logout deve invalidar sessão
- sessão expirada deve exigir novo login

---

## Recuperação de Senha

- recuperação deve exigir email válido
- token de recuperação deve possuir expiração
- senha redefinida deve seguir regras de senha
- token de recuperação não pode ser reutilizado

---

## Controle de Acesso

- permissões devem depender do cargo do usuário
- mentor não pode ser criado durante cadastro
- administrador não pode ser criado manualmente
- usuários sem autenticação não podem acessar áreas privadas

---

## Status da Conta

### Ativo

- possui acesso normal ao sistema

---

### Silenciado

- pode acessar a plataforma
- não pode enviar mensagens no curso no qual está silenciado

---

### Suspenso

- login deve ser bloqueado
- acesso à plataforma deve ser removido
- pode pedir análise da conta