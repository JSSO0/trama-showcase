# Trama — Plataforma de Inteligência Narrativa

> **Projeto de estudo.** Uma plataforma em que o escritor escreve sua obra por capítulos e uma IA
> **analisa progressivamente** o texto, construindo um **grafo de conhecimento narrativo** —
> personagens, locais, eventos, objetos e as relações entre eles. O sistema mantém **fichas de
> personagem**, detecta **inconsistências** e oferece **escrita assistida** (sugestões). A IA
> **nunca substitui o autor**: ela sugere, analisa e alerta — o autor decide.

![stack](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)
![stack](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)
![stack](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=black)
![stack](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript&logoColor=white)
![stack](https://img.shields.io/badge/Vite-5-646CFF?logo=vite&logoColor=white)
![stack](https://img.shields.io/badge/PostgreSQL-16-4169E1?logo=postgresql&logoColor=white)
![stack](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)

---

## O que é

Escrever uma história longa exige **memória**: quem é cada personagem, o que cada um sabe, o que foi
prometido, o que ainda está em aberto. Conforme o texto cresce, essa memória se perde e surgem
inconsistências.

**Trama** resolve isso acompanhando a obra enquanto ela é escrita. A cada capítulo, a IA extrai e
atualiza um **mapa vivo** da narrativa — e devolve ao autor percepções que ajudam a manter a história
coerente, profunda e bem armada — sem jamais reescrever o texto sem autorização.

### Princípios

- **O autor manda.** A IA sugere, analisa e alerta — nunca reescreve sem consentimento.
- **Análise incremental.** A cada capítulo, apenas o novo conteúdo é processado e reconciliado com o estado anterior.
- **Privacidade por padrão.** A arquitetura suporta IA local; provedores remotos são plugáveis.
- **Design de marca.** Nada de gerar capítulos inteiros por IA: o sistema apoia, não substitui, o escritor.

---

## Funcionalidades em destaque

| | |
|---|---|
| **Editor com "margem viva"** — ao escrever, a página mostra contexto da entidade citada: ficha, voz, promessas em aberto e últimas menções, sem spoilers. | **Grafo de conhecimento** — mapa interativo de personagens, locais, eventos e relações, com evolução ao longo dos capítulos. |
| **Fichas de personagem** — física, personalidade, motivações e voz; atualizadas pela análise e aprovadas pelo autor. | **Consistência** — detecção de contradições e violações das regras de mundo; alertas de voz fora do padrão do personagem. |
| **Livro de promessas** — juramentos, dívidas, segredos, armas de Chekhov e profecias, com status aberto/cumprido/quebrado. | **"Quem sabe o quê"** — fatos secretos, quem conhece cada um, vazamentos e fair-play de pistas. |
| **Raio de impacto** — simule remoção de uma entidade ou evento e veja quais capítulos seriam afetados; renomeie personagens com preview. | **Curva de tensão** — análise dramática por capítulo e leitura instrumentada (com consentimento) comparando o previsto com o real. |
| **Escrita assistida** — sugestões de continuação, melhoria de trecho, "e se...", leitor beta e sinopse; sempre com aceite/rejeição e diff. | **Colaboração** — versões com diff, comentários ancorados no texto, links de compartilhamento e codex público com teto de spoiler. |
| **Importação de manuscrito** — traga um arquivo existente (docx/epub/md) e a análise mapeia tudo automaticamente. | **Painel administrativo** — gestão de usuários, permissões, cotas, métricas de uso e auditoria. |

> Galeria completa com capturas de tela em [docs/FEATURES.md](./docs/FEATURES.md).

---

## Visão técnica (resumo)

| Camada | Tecnologia |
|---|---|
| Frontend | React 18 + TypeScript + Vite + Tailwind |
| Backend | Python 3.12 + FastAPI + SQLAlchemy (async) + Alembic |
| Banco de dados | PostgreSQL 16 + pgvector |
| Fila assíncrona | Celery + Redis (opcional) |
| IA | Camada de provedores plugáveis (OpenAI, Gemini, xAI, GLM, Anthropic) |
| Infra | Docker Compose (dev/prod) + Nginx + GitHub Actions (segurança) |

Detalhes em [docs/STACK.md](./docs/STACK.md) e [docs/ARCHITECTURE.md](./docs/ARCHITECTURE.md).

---

## Documentação

| Documento | Conteúdo |
|---|---|
| [docs/PRODUCT.md](./docs/PRODUCT.md) | O problema, a solução e os princípios do produto |
| [docs/FEATURES.md](./docs/FEATURES.md) | Tour completo das funcionalidades com capturas |
| [docs/ARCHITECTURE.md](./docs/ARCHITECTURE.md) | Visão de arquitetura de alto nível |
| [docs/STACK.md](./docs/STACK.md) | Stack técnica e justificativas |

---

## Sobre este repositório

Este é um **repositório de demonstração**: apresenta o projeto, as funcionalidades e o resultado do
trabalho realizado. O código-fonte e os detalhes técnicos internos são mantidos em repositório privado.

Status do projeto: **funcional** — as fases do roadmap (fundação, núcleo, análise narrativa,
consistência, escrita assistida, colaboração e funcionalidades disruptivas) foram implementadas e
integradas, conforme descrito em [docs/FEATURES.md](./docs/FEATURES.md).

## Licença

Todos os direitos reservados. Veja [LICENSE.md](./LICENSE.md).