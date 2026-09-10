---
name: android-quality
description: Investiga falhas, revisa código e cria testes para projetos Android. Use em debugging, code review, regressões ou proteção de comportamento; respeite se o pedido autoriza apenas diagnóstico ou também implementação.
---

# Android Quality

Identifique o modo solicitado antes de agir:

- **Debug:** existe falha, crash, build quebrado ou comportamento incorreto a investigar.
- **Testes:** o objetivo é proteger comportamento com testes unitários, de integração ou de UI.
- **Revisão:** o objetivo é encontrar riscos e reportar achados, sem alterar código automaticamente.

Não transforme análise ou revisão em autorização para modificar arquivos. Implemente uma correção
somente quando o pedido incluir correção ou implementação.

## Princípios compartilhados

- Baseie conclusões em comportamento reproduzível, código ou saída de ferramentas.
- Priorize corretude, lifecycle, concorrência, estado, dados, segurança e regressões.
- Faça validação proporcional ao risco e execute a menor task que cubra a mudança.
- Separe problemas preexistentes daqueles introduzidos pela alteração atual.
- Não reporte preferência estilística como defeito funcional.

## Referências

- Leia [debugging](references/debugging.md) quando houver uma falha concreta para investigar.
- Leia [testes](references/testing.md) quando criar ou modificar testes.
- Leia [code review](references/code-review.md) quando o pedido for revisão ou auditoria.
