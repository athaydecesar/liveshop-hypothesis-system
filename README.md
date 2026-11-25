# liveshop-hypothesis-system

**Organização:** LiveShop Turbo · **Repositório:** `liveshop-hypothesis-system`
https://github.com/liveshop-turbo/liveshop-hypothesis-system

Sistema de hipóteses para mídia paga da LiveShop Turbo. A ideia central é que **nenhum anúncio sobe na Meta sem uma hipótese registrada antes**, e que tudo que cada teste ensina vira conhecimento reaproveitável.

## O que o sistema vai fazer

- Registrar hipóteses de teste no formato Se / Então / Porque, com métrica e meta definidas antes do teste.
- Gerar os nomes padronizados de campanha, conjunto e anúncio.
- Conciliar, todo dia, o que está rodando na Meta com o que foi registrado.
- Sugerir ações para cada criativo (cortar, aguardar, promover, validar) com base em uma régua.
- Guardar os aprendizados e a confiança de cada um.

O sistema apenas **lê** dados da Meta. Ele nunca cria, edita, pausa ou exclui nada lá.

## Status

Em construção. Estamos na fundação do repositório (Épico E1, Feature F1.1). Ainda não há código do produto.

## Como contribuir

Todas as mudanças entram pela `main` por Pull Request. Leia o [fluxo de git](docs/fluxo-de-git.md) antes de abrir o primeiro.

Regras da `main`:

- Não aceita push direto.
- O PR só é mesclado com o job `all-checks-passed` aprovado.
- O PR precisa da aprovação de uma pessoa diferente do autor (exceção prevista em `docs/fluxo-de-git.md`, §4).
- Só são permitidos merge por **squash** ou **rebase**.
- A branch é apagada depois do merge.

## Estrutura do repositório

```
.
├── .github/workflows/ci.yml   # verificações do PR (inclui o all-checks-passed)
├── docs/
│   └── fluxo-de-git.md        # regras de branch, commit e PR
└── README.md
```
