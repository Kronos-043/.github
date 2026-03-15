# Guia de contribuição

Obrigado por contribuir! Leia este guia antes de abrir um PR ou issue.

---

## Fluxo de trabalho

```
main          → produção (protegida, merge via PR)
develop       → integração contínua
feature/xxx   → nova funcionalidade
fix/xxx       → correção de bug
chore/xxx     → manutenção, deps, infra
docs/xxx      → documentação
```

1. Crie sua branch a partir de `develop`
2. Desenvolva e faça commits seguindo a convenção abaixo
3. Abra um PR apontando para `develop`
4. Aguarde revisão e aprovação
5. Após merge, delete a branch

---

## Convenção de commits

Seguimos [Conventional Commits](https://www.conventionalcommits.org/pt-br/):

```
<tipo>: <descrição curta no imperativo>

[corpo opcional]

[rodapé opcional — ex: Closes #123]
```

### Tipos válidos

| Tipo | Quando usar |
|------|-------------|
| `feat` | Nova funcionalidade |
| `fix` | Correção de bug |
| `refactor` | Refatoração sem mudança de comportamento |
| `chore` | Atualizações de deps, configs, CI |
| `docs` | Apenas documentação |
| `test` | Adição ou correção de testes |
| `perf` | Melhoria de performance |
| `revert` | Reverte um commit anterior |

### Exemplos

```
feat: add a new Auth JWT
fix: fix the user listing pagination
chore: updating the project dependencies
docs: updating README.md
```

---

## Pull Requests

- Use o template fornecido — não apague as seções
- Título no mesmo formato dos commits
- PR deve ter **escopo pequeno e focado** — evite PRs com múltiplas responsabilidades
- Mínimo de **1 aprovação** antes do merge
- CI deve estar 100% verde
- Sem código comentado ou `console.log` esquecido

---

## Code review

**Para quem abre o PR:**
- Descreva bem o contexto — o revisor não viveu o problema com você
- Responda todos os comentários antes de pedir nova revisão
- Use "Resolve conversation" apenas após o problema ser de fato resolvido

**Para quem revisa:**
- Prazo: até **2 dias úteis** para dar o primeiro feedback
- Seja específico: aponte o que, onde e por quê
- Use prefixos para classificar o feedback:
  - `[blocker]` — precisa ser resolvido antes do merge
  - `[sugestão]` — melhoria opcional
  - `[dúvida]` — pergunta, não necessariamente um problema
  - `[elogio]` — reconheça o que está bom

---

## Testes

- Todo código novo deve ter cobertura de testes
- Testes devem rodar localmente antes de abrir o PR
- Não faça merge se algum teste estiver quebrando

---

## Dúvidas?

Abra uma **Discussion** ou pergunte no canal do time.
