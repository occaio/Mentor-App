# Fluxos do Sistema

## Cadastro de Usuário

Visitante acessa tela de cadastro  
→ informa nome, email e senha  
→ seleciona tipo de conta:
- aluno
- professor

→ sistema valida dados  
→ sistema verifica se email já existe  
→ conta é criada  
→ usuário é redirecionado para login

---

## Login

Usuário acessa tela de login  
→ informa email e senha  
→ sistema valida credenciais  
→ sistema verifica status da conta

Possíveis status:
- ativo
- silenciado
- suspenso

→ sessão é criada  
→ permissões do usuário são carregadas  
→ usuário é redirecionado para dashboard correspondente ao cargo

---

## Criação de Turma

Professor acessa painel acadêmico  
→ cria nova turma  
→ define:
- nome
- descrição
- imagem
- categoria
- regras da turma

→ sistema cria turma  
→ chat e calendário da turma são inicializados

---

## Entrada em Turma

Aluno acessa página da turma  
→ sistema verifica:
- existência da turma
- permissões de acesso
- matrícula
- possíveis restrições

→ aluno entra na turma  
→ conteúdos são liberados  
→ chats e materiais ficam acessíveis

---

## Criação de Curso

Professor acessa painel de cursos  
→ cria curso  
→ define:
- título
- descrição
- preço
- categoria
- capa

→ sistema valida dados  
→ curso é salvo  
→ curso pode receber aulas e materiais

---

## Publicação de Aula

Professor acessa curso ou turma  
→ cria aula  
→ adiciona:
- vídeo
- resumo
- anexos
- links
- materiais complementares

→ sistema valida conteúdo  
→ aula é publicada  
→ alunos recebem acesso

---

## Criação de Questionário

Professor cria questionário  
→ adiciona perguntas e alternativas  
→ define:
- resposta correta
- pontuação
- limite de tentativas
- tempo limite

→ sistema salva questionário  
→ questionário é disponibilizado aos alunos

---

## Resolução de Questionário

Aluno acessa questionário  
→ sistema verifica disponibilidade e tentativas restantes  
→ aluno responde perguntas  
→ sistema calcula pontuação  
→ resultado é salvo  
→ progresso do aluno é atualizado

---

## Envio de Atividade

Professor cria atividade  
→ define:
- descrição
- prazo
- anexos
- critérios de avaliação

→ atividade é publicada  
→ aluno envia resposta  
→ sistema registra envio  
→ professor corrige atividade  
→ nota e feedback são registrados

---

## Promoção para Mentor

Professor acessa gerenciamento da turma  
→ seleciona aluno  
→ sistema verifica elegibilidade  
→ aluno recebe cargo de mentor na turma

Novas permissões:
- auxiliar alunos
- responder dúvidas
- moderar conversas
- publicar resumos

---

## Comunicação no Chat

Usuário acessa chat  
→ sistema valida permissões  
→ usuário envia mensagem  
→ mensagem é registrada  
→ participantes recebem atualização em tempo real

---

## Silenciamento de Usuário

Mentor ou professor seleciona usuário  
→ define duração do silenciamento  
→ sistema remove permissão de envio de mensagens temporariamente  
→ usuário permanece apenas com leitura no chat

---

## Suspensão de Usuário

Professor ou administrador seleciona usuário  
→ sistema registra motivo da suspensão  
→ acesso à sala de aula é bloqueado  

---

## Sistema de Gamificação

Usuário realiza ações acadêmicas:
- assistir aulas
- concluir atividades
- responder questionários
- participar de chats
- auxiliar outros alunos

→ sistema calcula XP  
→ progresso é atualizado  
→ conquistas e medalhas podem ser desbloqueadas