# Casos de Exceção

## Cadastro

- usuário tenta cadastrar email já existente
- email possui formato inválido
- senha possui menos de 8 caracteres
- senha e confirmação são diferentes
- campos obrigatórios não foram preenchidos
- tipo de conta não foi selecionado

---

## Login

- email não existe
- senha incorreta
- conta suspensa tenta realizar login
- usuário tenta acessar área privada sem autenticação
- múltiplos cliques no botão de login
- internet cai durante autenticação

---

## Sessão

- sessão expira durante uso da plataforma
- token de autenticação inválido
- usuário realiza logout em múltiplas abas
- permissões do usuário mudam durante sessão ativa

---

## Recuperação de Senha

- email de recuperação não existe
- token de recuperação expirou
- token de recuperação é inválido
- token já foi utilizado
- nova senha não segue regras do sistema

---

## Controle de Acesso

- aluno tenta acessar funcionalidades de professor
- mentor tenta acessar administração global
- usuário suspenso tenta acessar rotas privadas
- usuário sem permissão tenta moderar chat

---

## Status da Conta

### Conta Silenciada

- usuário tenta enviar mensagens no chat


---

### Conta Suspensa

- usuário tenta realizar login
- usuário tenta recuperar sessão ativa
- usuário tenta acessar URLs privadas diretamente