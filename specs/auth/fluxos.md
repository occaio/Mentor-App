# Auth Flows

## Cadastro de Usuário

Usuário acessa tela de cadastro  
→ informa:
- nome
- email
- senha
- confirmação de senha
- tipo de conta

→ sistema valida:
- campos obrigatórios
- formato do email
- senha mínima
- confirmação de senha
- email único

→ conta é criada  
→ usuário é redirecionado para login

---

## Login

Usuário acessa tela de login  
→ informa:
- email
- senha

→ sistema valida credenciais  
→ sistema verifica status da conta

Possíveis estados:
- ativo
- silenciado
- suspenso

→ sessão é criada  
→ permissões são carregadas  
→ usuário é redirecionado para dashboard

---

## Logout

Usuário solicita logout  
→ sistema invalida sessão  
→ dados de autenticação são removidos  
→ usuário retorna para tela inicial

---

## Recuperação de Senha

Usuário acessa recuperação de senha  
→ informa email  
→ sistema valida existência da conta  
→ token de recuperação é gerado  
→ instruções são enviadas ao usuário

Usuário acessa redefinição  
→ informa nova senha  
→ sistema valida token  
→ senha é atualizada

---

## Expiração de Sessão

Sessão atinge tempo limite  
→ sistema invalida autenticação  
→ usuário perde acesso às áreas privadas  
→ login é solicitado novamente

---

## Bloqueio por Suspensão

Administrador ou professor suspende usuário  
→ sistema altera status da conta para suspenso  
→ sessão ativa é encerrada  
→ novos logins são bloqueados

---

## Silenciamento

Professor ou mentor silencia usuário  
→ sistema altera status para silenciado  
→ envio de mensagens é bloqueado  
→ acesso geral permanece disponível