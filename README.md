# CV_Match_IA
Uma plataforma que utiliza Inteligência Artificial para analisar a compatibilidade entre currículos e vagas de emprego, ajudando candidatos a tomarem decisões mais assertivas antes de se candidatarem.

# App de geração de currículo ATS Friendly com Vibe Coding
Criar soluções com IA de forma criativa, guiando ferramentas como o Copilot e o Lovable com uma comunicação simples e natural. O foco é desenvolver o conceito de um App de geração de currículos , mas, acima de tudo, aprender o jeito Vibe de programar com IA.

✨ O que é Vibe Coding
Vibe Coding é uma forma leve e criativa de desenvolver com IA, baseada em conversas naturais e bem estruturadas. Você não precisa escrever código linha por linha. Em vez disso, aprende a guiar a IA descrevendo suas ideias de forma clara, com intenção e contexto. Em outras palavras:

🎯 Desafio
Problema: Muitas pessoas que se canditam a vagas de emprego tem dificuldades de comparar ou até mesmo identificar se o seu currículo é condizente com a vaga, então esse app busca tornar essa identificação entre currículo e vaga um pouco mais amigavél e rápida.
Você deve utilizar as ideias de Vibe Coding e MVP (Produto Mínimo Viável) para desenvolver o conceito de um aplicativo que resolva o problema citado.

# Contexto
Quero criar um aplicativo de geração de currículo que funcione por meio de interações com o usuário.  
A ideia é facilitar a candidatura a vaga de emprego, assim como tornar o usuário ciente de quanto o seu currículo é compatível com a vaga desejada.

# Problema
Muitas pessoas desistem de se candidatar a algumas vagas de emprego por não saber se seu currículo é compatível com a vaga e algumas empresas de RH também tem dificuldades de expressar corretamente os principais requisitos para algumas vagas.  
Quero resolver isso com uma experiência de conversa e recomendações automáticas de  compatibilidade curricular e também de dicas para melhorar o currículo para cada vaga pretendida.

# Público-Alvo
Pessoas que buscam vagas de emprego e que não querem perder seu tempo candidatando para vagas que não aderem seu perfil e também para RHs que buscam os perfil exato de candidato para a vaga disponível. 

# Funcionalidades-Chave
1. Registro do currículo.
2. Definir o perfil do candidato e da vaga.
3. Classificação de compatibilidade entre curriculo  e vaga.  
4. Receber dicas de melhoria do currículo  do “Agente Financeiro”.  

# Entregável da IA
Gerar um plano de MVP com as principais telas, recursos necessários e um esboço de validação inicial.  
Usar tom educativo e linguagem acessível, em português.


O seu prompt final (PRD) usado com a IA;
...
# CV Match AI

Uma plataforma que utiliza Inteligência Artificial para analisar a compatibilidade entre currículos e vagas de emprego, ajudando candidatos a tomarem decisões mais assertivas antes de se candidatarem.

---

## 📌 Sobre o Projeto

Muitos profissionais deixam de se candidatar a vagas por não saberem se possuem o perfil adequado. Ao mesmo tempo, recrutadores frequentemente recebem candidaturas com baixa aderência aos requisitos da posição.

O CV Match AI busca resolver esse problema através de uma experiência simples e intuitiva, permitindo que o usuário compare seu currículo com uma vaga específica e receba uma análise detalhada com recomendações de melhoria.

---

## 🎯 Objetivo

Permitir que candidatos:

- Avaliem sua compatibilidade com uma vaga.
- Economizem tempo em candidaturas pouco aderentes.
- Recebam feedback personalizado sobre seus currículos.
- Identifiquem competências que precisam desenvolver.
- Melhorem suas chances de aprovação em processos seletivos.

---

## 🚀 Principais Funcionalidades

### ✅ Cadastro de Usuário

- Login por e-mail e senha.
- Autenticação segura.
- Gerenciamento de conta.

### ✅ Cadastro de Currículo

- Upload de currículo em PDF.
- Inserção manual de texto.
- Armazenamento do histórico de currículos.

### ✅ Cadastro de Vaga

- Título da vaga.
- Descrição completa da oportunidade.
- Requisitos e competências desejadas.

### ✅ Análise de Compatibilidade

Comparação inteligente entre:

- Currículo do candidato.
- Requisitos da vaga.

A plataforma gera:

- Score de compatibilidade (0 a 100).
- Competências identificadas.
- Competências ausentes.
- Resumo da análise.

### ✅ Recomendações com IA

Sugestões personalizadas para:

- Melhorar o currículo.
- Destacar experiências relevantes.
- Evidenciar competências importantes.
- Aumentar a aderência à vaga desejada.

### ✅ Histórico de Análises

- Registro das análises realizadas.
- Consulta de resultados anteriores.
- Evolução do currículo ao longo do tempo.

---

## 🖥️ Fluxo do Usuário

```text
Login
  ↓
Cadastrar Currículo
  ↓
Inserir Descrição da Vaga
  ↓
Analisar Compatibilidade
  ↓
Visualizar Resultado
  ↓
Receber Recomendações
```

---

## 📱 Telas do MVP

### Landing Page

- Apresentação da solução.
- Benefícios da plataforma.
- Chamada para ação.

### Login

- Acesso à plataforma.

### Dashboard

- Currículos cadastrados.
- Histórico de análises.
- Acesso rápido às funcionalidades.

### Cadastro de Currículo

- Upload de PDF.
- Inserção manual de texto.

### Análise de Vaga

- Campo para descrição da vaga.
- Geração de compatibilidade.

### Resultado

- Score de aderência.
- Pontos fortes.
- Lacunas identificadas.
- Recomendações da IA.

---

## 🏗️ Arquitetura Simplificada

```text
Frontend (Lovable)
        ↓
     Supabase
        ↓
     OpenAI
```

### Frontend

- React
- TypeScript
- Tailwind CSS
- Shadcn UI

### Backend

- Supabase

### Banco de Dados

- PostgreSQL (Supabase)

### Inteligência Artificial

- OpenAI API

### Deploy

- Vercel

### Versionamento

- GitHub

---

## 📂 Estrutura do Projeto

```text
cv-match-ai/
│
├── src/
├── components/
├── pages/
├── services/
├── hooks/
├── lib/
├── supabase/
├── public/
├── docs/
├── README.md
├── .env.example
└── package.json
```

---

## 🗄️ Estrutura Inicial do Banco de Dados

### users

```sql
id
name
email
created_at
```

### resumes

```sql
id
user_id
content
created_at
```

### analyses

```sql
id
user_id
job_description
score
recommendations
created_at
```

---

## 🎯 MVP

O objetivo inicial é validar se usuários realmente valorizam:

1. A análise de compatibilidade entre currículo e vaga.
2. Recomendações geradas por IA.
3. Um score que auxilie na decisão de candidatura.

O MVP foi projetado para ser simples, escalável e compatível com plataformas low-code como Lovable.

---

## 📊 Métricas de Sucesso

### Produto

- Taxa de conclusão da análise.
- Número de análises realizadas por usuário.
- Retenção de usuários.

### Negócio

- Crescimento de usuários cadastrados.
- Taxa de retorno à plataforma.

### IA

- Avaliação positiva das recomendações.
- Utilidade percebida pelo usuário.

---

## 🔮 Próximos Passos

- Chat de carreira com IA.
- Sugestão automática de vagas.
- Integração com LinkedIn.
- Integração com plataformas de RH.
- Geração automática de currículo otimizado.
- Dashboard para recrutadores.

---

## 📄 Licença

Este projeto é open source e está disponível sob a licença MIT.

---

## 💡 Missão

Ajudar profissionais a encontrarem oportunidades mais alinhadas aos seus perfis e utilizarem Inteligência Artificial para acelerar seu crescimento profissional.
...

Interações com o Copilot/Lovable.

Um resumo do conceito do seu app;
Uma plataforma que utiliza Inteligência Artificial para analisar a compatibilidade entre currículos e vagas de emprego, ajudando candidatos a tomarem decisões mais assertivas antes de se candidatarem.

Uma breve reflexão sobre o que aprendeu no processo.
Cada IA tem suas particularidades ao atender um questionamento.


