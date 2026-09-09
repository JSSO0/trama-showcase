# Stack — Tecnologias

> Resumo público da stack técnica. Justificativas profundas e decisões registradas são mantidas em
> repositório privado.

## Frontend

| Tecnologia | Uso |
|---|---|
| **React 18 + TypeScript 5** | SPA, tipagem estrita em todo o código |
| **Vite 5** | Build e dev server (HMR) |
| **Tailwind CSS 3** | Estilização com dark mode |
| **TanStack Query 5** | Dados de servidor, cache e invalidação |
| **Zustand 5** | Estado global (autenticação, tema) |
| **React Router 6** | Navegação |
| **Axios** | HTTP com refresh automático de token (single-flight) |

## Backend

| Tecnologia | Uso |
|---|---|
| **Python 3.12 + FastAPI** | API REST, tipada (OpenAPI gerado automaticamente) |
| **Pydantic v2** | Validação e schemas |
| **SQLAlchemy 2 (async)** | ORM |
| **Alembic** | Migrações de banco versionadas |
| **Celery + Redis** | Fila assíncrona para análises pesadas (opcional) |
| **PyJWT + Argon2** | Autenticação e hash de senha |
| **SlowAPI** | Rate limiting |

## Dados e IA

| Tecnologia | Uso |
|---|---|
| **PostgreSQL 16 + pgvector** | Persistência e buscas vetoriais |
| **Camada de provedores de IA plugável** | OpenAI · Gemini · xAI · GLM · Anthropic — configurável e substituível; suporta modelo local |
| **Rastreamento de uso** | Contagem de tokens e custo por operação (transparência para o operador) |

## Infraestrutura

| Tecnologia | Uso |
|---|---|
| **Docker Compose** | Ambiente de dev e produção com um comando |
| **Nginx** | Servir o frontend e fazer proxy da API |
| **GitHub Actions** | Pipeline de segurança: segredos, análise estática, dependências, teste dinâmico |

## Estrutura de pastas (nível 1)

```
apps/
  web/     → SPA React/TypeScript
  api/     → Backend FastAPI/Python
site/      → Páginas institucionais (projeto de estudo)
docs/      → Documentação (planejamento)
```

> O código-fonte completo não está neste repositório de demonstração.