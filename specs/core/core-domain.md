# Core Domain

## 📌 Objetivo

Definir as principais entidades, responsabilidades e relações do sistema Mentor App.

Este documento representa o núcleo do domínio da aplicação.

---

# 👤 User

Representa qualquer usuário autenticado na plataforma.

Todos os usuários possuem:

- id
- nome
- email
- senha
- foto de perfil
- data de criação
- permissões

---

## Tipos de Usuário

### Student (Aluno)

Usuário principal da plataforma.

Pode:

- assistir aulas
- participar de chats
- responder quizzes
- enviar atividades
- acompanhar progresso
- acessar materiais

---

### Teacher (Professor)

Responsável pela criação e gerenciamento de conteúdos acadêmicos.

Pode:

- criar cursos
- criar turmas
- publicar aulas
- criar atividades
- moderar chats
- promover mentores

---

### Mentor

Aluno promovido por um professor para auxiliar outros estudantes.

Pode:

- responder dúvidas
- ajudar alunos
- moderar conversas
- criar resumos
- auxiliar alunos com dificuldades

---

### Admin (Administrador)

Responsável pelo gerenciamento global da plataforma.

Pode:

- gerenciar usuários
- aplicar punições globais
- visualizar relatórios
- administrar o sistema

---

# 🏫 Classroom

Representa uma sala acadêmica criada por um professor.

Uma sala pode possuir:

- alunos
- mentores
- aulas
- atividades
- quizzes
- chat
- materiais complementares

---

## Regras

- toda sala deve possuir um professor responsável
- alunos devem estar matriculados para acessar conteúdos
- mentores pertencem a uma sala específica

---

# 📚 Course

Representa um curso disponibilizado na plataforma.

Pode ser:

- gratuito
- pago

---

## Possui

- título
- descrição
- thumbnail
- aulas
- categoria
- professor responsável

---

# 🎥 Lesson

Representa uma aula individual.

Pode conter:

- vídeo
- resumo
- anexos
- links
- comentários
- materiais extras

---

# 📝 Quiz

Representa questionários e avaliações acadêmicas.

Pode possuir:

- perguntas
- alternativas
- respostas corretas
- pontuação
- limite de tentativas

---

# 📄 Assignment

Representa atividades enviadas aos alunos.

Possui:

- título
- descrição
- prazo
- nota
- arquivos anexados

---

# 💬 ChatRoom

Representa ambientes de comunicação da plataforma.

Tipos:

- chat geral
- dúvidas por aula
- mentoria privada
- mensagens diretas

---

# 💬 Message

Representa mensagens enviadas em chats.

Possui:

- autor
- conteúdo
- horário
- anexos
- status

---

# 🛡️ Moderation

Representa o sistema de moderação da plataforma.

Inclui:

- avisos
- silenciamento
- suspensão
- controle de permissões

---

# 📚 Summary

Representa resumos acadêmicos publicados por professores ou mentores.

Pode conter:

- texto
- imagens
- links
- anexos

---

# 🎖️ Gamification

Representa o sistema de recompensas e engajamento.

Inclui:

- XP
- medalhas
- conquistas
- ranking

---

# 🔗 Relações Principais

## User ↔ Classroom

- professores criam salas
- alunos participam de salas
- mentores auxiliam salas

---

## Course ↔ Lesson

- um curso possui múltiplas aulas

---

## Classroom ↔ ChatRoom

- uma sala pode possuir múltiplos chats

---

## Lesson ↔ Quiz

- aulas podem possuir quizzes associados

---

## User ↔ Moderation

- usuários podem receber punições e restrições

---

# 📌 Regras Gerais do Sistema

- usuários suspensos possuem acesso limitado
- apenas professores podem criar cursos
- mentores dependem da aprovação de professores
- alunos só acessam conteúdos matriculados
- quizzes podem possuir limite de tentativas

---

# 📈 Escalabilidade

O domínio foi projetado para permitir:

- crescimento modular
- novas features
- múltiplas instituições
- expansão futura da plataforma

---

# 🧠 Arquitetura por Domínio

O sistema será organizado por funcionalidades e responsabilidades.

Exemplo:

```txt
auth/
chat/
classroom/
quizzes/
moderation/