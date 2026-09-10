---
name: android-presentation
description: Cria ou modifica a camada de apresentação Android, incluindo telas Compose, ViewModels, estado de UI e navegação. Use quando a tarefa afetar interação ou fluxo de tela; não use para mudanças restritas a dados ou domínio.
---

# Android Presentation

Examine telas semelhantes, design system, mecanismo de estado e navegação antes de implementar.
Preserve as bibliotecas e convenções existentes; não presuma Compose ou uma solução de navegação.

## Limites compartilhados

- A UI renderiza estado e comunica ações; regras de negócio e infraestrutura ficam fora dela.
- Componentes reutilizáveis não conhecem ViewModels nem controladores de navegação.
- ViewModels não referenciam Composables, Views ou controladores de navegação.
- Estado observável é exposto somente para leitura e atualizado de forma imutável.
- Dependências são explícitas e seguem o mecanismo de injeção existente.
- Estado durável, estado local visual e efeitos transitórios têm responsabilidades diferentes.

Implemente loading, conteúdo, vazio e erro somente quando fizerem parte do comportamento. Verifique
compilação, lifecycle, restauração de estado, acessibilidade e fluxos alterados conforme aplicável.

## Referências

- Leia [Compose](references/compose.md) para telas, componentes, recomposição, estado local ou efeitos.
- Leia [ViewModel e estado](references/viewmodel-and-state.md) para lógica de apresentação, estado
  observável, coroutines ou concorrência.
- Leia [navegação](references/navigation.md) para destinos, argumentos, deep links ou retorno.
- Leia [acessibilidade](references/accessibility.md) quando criar ou alterar elementos interativos.
