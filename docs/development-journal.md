# Development Journal — Basketball Referee Development Platform

Registro de decisões, mudanças, descobertas e aprendizados ao longo do desenvolvimento do projeto.

---

## 24/08/2026

**O que foi feito:**
- Definido o Product Backlog completo, organizado em 8 módulos (Conta/Perfil, Jogos, Autoavaliação, Avaliação Externa, Histórico, Dashboard, Competições, Administração).
- Feita a "peneira" do MVP: cada funcionalidade foi testada contra a pergunta "isso é necessário para provar que a plataforma funciona?".
- Definido oficialmente o escopo da V0.1: Cadastro/Login, Perfil básico, Novo jogo manual, Autoavaliação completa e Histórico simples.
- Módulos inteiros (Avaliação Externa, Dashboard, Competições, Administração) foram empurrados para versões futuras (V0.2 em diante), pois dependem de um segundo tipo de usuário ou de complexidade que não é essencial para o ciclo mínimo do árbitro sozinho.
- Criado o Roadmap oficial, de V0.1 até V1.0.
- Organizado o repositório no GitHub: pasta `/docs` com `product-backlog.md`, `mvp-v0.1.md` e `roadmap.md`, e o README atualizado com links para a documentação.

**Aprendizados:**
- Definir um critério claro para o MVP ("sem isso, o loop mínimo não fecha?") ajudou a evitar inflar a primeira versão com funcionalidades que pareciam importantes mas não eram indispensáveis.
- Organizar a documentação antes de escrever qualquer código está deixando o projeto mais claro e fácil de retomar entre sessões de trabalho.

**Próximos passos:**
- Continuar respondendo o formulário de autoavaliação após os jogos.
- Acumular entre 10 e 20 jogos respondidos antes de analisar os primeiros padrões.

- ## 24/08/2026 (atualização) — Primeira análise das respostas

**Contexto:** Foram respondidos 9 jogos até o momento (não 20 como planejado — o restante 
não chegou a ser preenchido).

**Descoberta principal:**
O maior obstáculo identificado não foi nenhuma pergunta específica, mas o preenchimento 
dos dados administrativos do jogo (equipes, data, categoria etc.), sentido como cansativo 
e repetitivo pelo próprio usuário-piloto. Isso é uma validação direta de uma necessidade 
já prevista no Product Backlog (Módulo 2 — Jogos): a obtenção automática desses dados via 
integração com sistemas oficiais da federação/liga.

**Impacto na priorização:**
- Reforça que a fricção no cadastro do jogo é um risco real de abandono, não só uma 
  melhoria "nice to have". Vale reavaliar se algo simples (ex: lembrar times/categorias 
  usados recentemente) pode entrar antes da V0.4/V0.5 originalmente planejada.

**Padrões observados nos dados (9 jogos):**
- Dificuldade em "contatos" (durante o drible, sem a bola, excessivos) foi a mais recorrente, 
  aparecendo em 4 dos 9 jogos.
- Comunicação com os parceiros teve as notas mais baixas e variáveis entre as categorias 
  avaliadas — possível ponto de atenção genuíno, não só ruído.
- Pressão externa raramente interferiu na concentração, exceto em um jogo com comportamento 
  mais tenso das equipes.

**Evolução do formulário:**
Perguntas foram adicionadas e removidas ao longo das respostas, conforme a necessidade 
percebida durante o uso real. Isso é esperado no processo de validação, mas gera dados 
incompletos nos registros mais antigos — comparações diretas entre o jogo 1 e o jogo 9 
não são totalmente equivalentes.

**Próximos passos:**
- Retomar o preenchimento do formulário para alcançar uma amostra maior antes de fechar 
  o `questionnaire-v2.md`.
- Ao desenhar a tela de "Novo Jogo" (Etapa 6), considerar desde já formas de reduzir a 
  fricção de preenchimento (ex: sugestão automática de times já usados, campos opcionais 
  bem definidos).
