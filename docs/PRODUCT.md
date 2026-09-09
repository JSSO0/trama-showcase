# Product — Visão pública do produto

## O problema

Escrever uma história longa — um romance, uma série, um mundo — exige manter muita coisa na cabeça ao
mesmo tempo:

- Quem é cada personagem e como ele **se comporta** (voz, valores, motivações);
- O que cada personagem **sabe** e o que **não sabe** a cada momento;
- O que foi **prometido** ao leitor (mistérios, profecias, dívidas, armas de Chekhov);
- O que já aconteceu, **onde** e **em que ordem**;
- As **regras do mundo** e o que as viola.

Quando o texto cresce (dezenas de capítulos, dezenas de personagens), essa memória se perde. O autor
começa a cometer inconsistências: um personagem que esquece o que deveria saber, um tom de fala que
muda, uma promessa que nunca se cumpre, um evento que contradiz o capítulo 3.

## A solução

**Trama** acompanha a obra **enquanto ela é escrita** e constrói, progressivamente, um **mapa vivo**
da narrativa:

- Extrai e atualiza entidades (personagens, locais, eventos, objetos) e suas **relações**;
- Mantém **fichas de personagem** e um **fingerprint de voz** de cada um;
- Rastreia **promessas narrativas** e **fatos secretos** (quem sabe o quê);
- Detecta **inconsistências** e violações das **regras de mundo**;
- Devolve isso ao autor **no momento da escrita** — na "margem viva" do editor — e em
  visualizações (grafo, timeline, curva de tensão).

O resultado: o autor mantém a coerência de uma obra longa **sem abandonar o fluxo criativo** — e sem
que ninguém (nem a IA) reescreva seu texto.

## Princípios do produto

1. **O autor manda.** A IA sugere, analisa e alerta. Nenhuma alteração acontece sem aceite explícito.
   O texto é sempre do autor.
2. **Consciência estrutural em tempo real.** Cada capítulo salvo atualiza o entendimento global da obra.
3. **Análise incremental.** Não se re-analisa tudo do zero: apenas o delta é processado e reconciliado
   com o estado anterior — rápido e econômico.
4. **Privacidade por padrão.** A arquitetura prevê IA local no computador do autor; provedores remotos
   são plugáveis e ficam a critério de quem usa.
5. **Apoio, nunca substituição.** Não existe geração automática de capítulos. A ferramenta ajuda o
   escritor a escrever melhor, não a escrever por ele.

## Para quem é

- **Escritores de ficção longa** (romances, séries, sagas) que querem manter consistência sem abrir mão do fluxo;
- **Estudantes e pesquisadores** interessados em IA aplicada à análise narrativa;
- **Beta readers** e colaboradores que desejam explorar uma obra por um codex público, sem spoilers.

## Como o projeto nasceu

O projeto começou como um **estudo**: "uma IA consegue ler uma história?" A partir dessa pergunta, o
escopo evoluiu para uma plataforma completa de inteligência narrativa — sempre preservando a premissa
de que **a história é do autor**.