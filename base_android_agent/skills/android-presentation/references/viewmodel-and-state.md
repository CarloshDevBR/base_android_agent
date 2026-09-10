# ViewModel e estado

- Modele somente informações observáveis necessárias à UI.
- Use estrutura imutável quando campos puderem coexistir e estados mutuamente exclusivos quando
  flags independentes permitiriam combinações inválidas.
- Escolha callbacks ou eventos conforme a clareza da API existente.
- Não exponha exceções ou detalhes de infraestrutura diretamente à UI.
- Mantenha códigos ou tipos de erro separados do texto localizado.
- Estado representa o que continua verdadeiro; efeitos representam ocorrências pontuais.
- Antes de criar Channel ou SharedFlow para efeitos, verifique se callback, estado ou navegação
  declarativa resolvem o caso sem perda de eventos.
- Use o escopo ligado ao ciclo de vida do ViewModel e preserve `CancellationException`.
- Cancele ou serialize operações concorrentes quando a anterior deixar de ser relevante.
- Impeça respostas antigas de sobrescrever estado mais recente.
- Use debounce somente quando fizer parte do comportamento esperado.
- Não bloqueie a Main Thread nem use `GlobalScope`, `Thread.sleep` ou `runBlocking` em produção.
- Em testes, controle scheduler e dispatcher; não dependa de atrasos reais.
