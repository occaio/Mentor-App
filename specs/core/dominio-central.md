# Domínio Central

## Objetivo

Definir as principais entidades, responsabilidades e relações do sistema Mentor App.

---

# Usuário

Representa qualquer usuário autenticado na plataforma.

Todos os usuários possuem:

- id
- nome
- email
- senha
- foto de perfil
- permissões
- data de criação
- status da conta

Status possíveis:

- ativo
- silenciado
- suspenso

---

# Tipos de Usuário

- Aluno
- Professor
- Mentor
- Administrador

# Sala de Aula

Representa uma turma acadêmica criada por um professor.

Possui:

- professor responsável
- alunos
- mentores
- aulas
- atividades
- questionários
- calendário
- chats
- materiais acadêmicos

---

# Curso

Representa um curso disponível na plataforma.

Pode ser:

- gratuito
- pago

Possui:

- título
- descrição
- aulas
- materiais
- avaliações
- progresso
- certificado

---

# Aula

Representa uma aula individual.

Pode conter:

- vídeo
- resumo
- anexos
- links
- comentários
- materiais complementares

---

# Questionário

Representa quizzes e avaliações.

Possui:

- perguntas
- alternativas
- respostas corretas
- pontuação
- limite de tentativas
- tempo limite

---

# Atividade

Representa tarefas acadêmicas enviadas aos alunos.

Possui:

- título
- descrição
- prazo
- anexos
- nota
- feedback

---

# Chat

Representa ambientes de comunicação.

Tipos:

- chat geral
- dúvidas por aula
- mentoria privada
- mensagens diretas

---

# Mensagem

Representa mensagens enviadas no sistema.

Pode possuir:

- texto
- anexos
- horário
- autor
- resposta
- edição

---

# Moderação

Representa o sistema de controle disciplinar.

Inclui:

- avisos
- silenciamento temporário
- suspensão
- controle de permissões
- histórico de punições

---

# Resumo

Representa materiais resumidos criados por professores ou mentores.

Pode conter:

- texto
- imagens
- anexos
- links
- observações

---

# Gamificação

Representa o sistema de recompensas.

Inclui:

- XP
- medalhas
- conquistas
- ranking
- níveis

---

# Relações Principais

## Usuário ↔ Sala de Aula

- professores criam salas
- alunos participam das salas
- mentores auxiliam as salas

---

## Curso ↔ Aula

- um curso possui múltiplas aulas

---

## Sala de Aula ↔ Chat

- uma sala pode possuir múltiplos chats

---

## Aula ↔ Questionário

- aulas podem possuir questionários associados

---

## Usuário ↔ Moderação

- usuários podem receber punições e restrições