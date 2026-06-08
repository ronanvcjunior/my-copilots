# 🧩 Modos do Copiloto (Ask, Plan, Study, Agent, Refactor, Debugger)

O Copiloto oferece diferentes modos de interação para você escolher como quer trabalhar: desde tirar dúvidas sem mexer no código, até planejar mudanças maiores, aprender novos conceitos, delegar tarefas complexas, refatorar estruturas ou depurar erros. A ideia é simples: você seleciona o modo que melhor combina com seu objetivo no momento e ganha velocidade com mais controle.

## ❓ Ask
O modo **Ask** é para fazer perguntas e entender coisas, **sem alterar seu código**. Você pode perguntar sobre um arquivo específico, um erro, uma função, uma stack trace ou até conceitos gerais.

O Copiloto lê o contexto do projeto (arquivos abertos, seleção, etc.) e responde como um “mentor técnico”, explicando o que está acontecendo e por quê. Ele **não modifica nada** — só analisa e explica.

📄 **Prompt:** [prompts/prompt-ask.md](prompts/prompt-ask.md)

---

## 🧭 Plan
Quando você pede algo mais complexo, o Copiloto pode entrar no modo **Plan**, onde ele **pensa e descreve os passos antes de sair codando**.

Ele:
- divide o problema em etapas
- explica o que vai fazer
- só depois executa (se você permitir)

Isso é muito útil para mudanças grandes, novas features ou quando você quer validar a abordagem antes de mexer no código.

📄 **Prompt:** [prompts/prompt-plan.md](prompts/prompt-plan.md)

---

## 📚 Study
O modo **Study** é focado em **aprendizado ativo**, não só em chegar à resposta ou ao código final.

Em vez de simplesmente explicar ou executar, ele:
- ensina e guia o raciocínio
- destaca conceitos e trade-offs
- faz perguntas reflexivas
- avança em progressão gradual de dificuldade

Funciona quase como um **tutor particular**.

📄 **Prompt:** [prompts/prompt-study.md](prompts/prompt-study.md)

---

## 🤖 Agent
O **Agent** é o modo mais **“autônomo”**. Ele pode navegar pelo projeto, criar arquivos, modificar múltiplos pontos e manter contexto entre passos, como se fosse um dev júnior trabalhando com você.

Você dá um objetivo (ex.: *“implemente login com JWT”*) e ele decide o que precisa ser feito em vários arquivos para chegar lá.

📄 **Prompt:** [prompts/prompt-agent.md](prompts/prompt-agent.md)

---

## ♻️ Refactor
O modo **Refactor** é especializado em **reescrever código existente sem alterar seu comportamento externo**.

Ideal para:
- melhorar legibilidade
- remover duplicação
- aplicar padrões de projeto
- extrair funções/variáveis
- renomear símbolos de forma segura
- reestruturar pastas ou módulos

Aqui o foco é: *“deixe o código mais limpo, mantendo o que ele faz”*.

📄 **Prompt:** [prompts/prompt-refactor.md](prompts/prompt-refactor.md)

---

## 🐞 Debugger
O modo **Debugger** é feito para **encontrar e corrigir erros** de forma sistemática.

Ele pode:
- analisar stack traces e logs
- sugerir hipóteses para bugs
- adicionar pontos de verificação (logs/asserts)
- explicar comportamentos inesperados
- propor correções com justificativa

Diferente do modo Ask (que só explica), o Debugger **atua ativamente no diagnóstico e na correção**.

📄 **Prompt:** `prompts/prompt-debugger.md`

---

## 🧠 Resumo mental rápido

| Modo       | Quando usar                                      |
|------------|--------------------------------------------------|
| Ask        | entender, perguntar, aprender sem mudar código   |
| Plan       | planejar antes de agir (passos complexos)        |
| Study      | aprendizado profundo com perguntas e progressão  |
| Agent      | executar tarefas grandes sozinho (vários arquivos) |
| Refactor   | melhorar estrutura/código sem mudar comportamento|
| Debugger   | encontrar e corrigir bugs                        |
