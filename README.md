# IHC 2026.2 – Grupo 07

Projeto final de Interação Humano-Computador (FCTE/UnB, 2026.2): guia de acessibilidade, pocket de IHC, avaliação do Portal da Câmara dos Deputados e avaliação com usuário.

**Site:** https://renanpr7.github.io/pocket_ihc/

## Rodar localmente

```bash
python3 -m venv .venv
.venv/bin/pip install -r requirements.txt
.venv/bin/mkdocs serve
```

O site abre em http://127.0.0.1:8000. Toda alteração em `main` é publicada automaticamente pelo workflow em `.github/workflows/deploy.yml`.

## Estrutura

| Pasta | Conteúdo |
| --- | --- |
| `docs/guia/` | Guia de acessibilidade e checklist de 143 itens |
| `docs/pocket/` | UX, ferramentas e técnicas, Do e Don't, conscientização |
| `docs/avaliacao-site/` | Checklist aplicado ao Portal da Câmara dos Deputados |
| `docs/avaliacao-usuario/` | Roteiro e resultados do teste de usabilidade |
| `docs/images/` | Capturas de tela usadas como evidência |

A gravação do teste com usuário e o termo de consentimento não ficam neste repositório: o termo assinado pelo participante garante que o nome dele não seja divulgado e que só o grupo, a professora e os monitores acessem a gravação.
