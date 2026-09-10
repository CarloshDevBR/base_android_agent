# Compose

- Reutilize tema, componentes e convenções existentes antes de criar algo novo.
- Mantenha componentes stateless quando isso simplificar uso e teste.
- Não extraia componentes sem ganho de clareza ou reutilização.
- Mantenha estado puramente efêmero no componente visual apropriado.
- Colete fluxos respeitando o lifecycle do host.
- Use `remember` para estado que pode ser perdido com recriação e `rememberSaveable` somente para
  estado pequeno que precisa sobreviver à recriação.
- Use efeitos apenas para sincronização com algo externo à composição.
- Escolha keys de `LaunchedEffect` e `DisposableEffect` que representem quando o efeito deve reiniciar.
- Não use efeitos para derivar valores calculáveis durante a composição.
- Evite gravar estado durante composição ou capturar callbacks obsoletos em efeitos longos.
- Adicione previews úteis quando o projeto os adotar.
