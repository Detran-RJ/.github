# Configuração padrão da organização Detran-RJ

## Visibilidade

- Repositórios privados por padrão.
- Repositórios públicos somente para perfil, documentação institucional aprovada ou conteúdo sintético.

## Fluxo de trabalho

1. Abrir issue.
2. Criar branch curta.
3. Abrir PR.
4. Solicitar revisão automatizada quando disponível.
5. Aguardar CI/quality.
6. Merge squash.

## Branches

| Branch | Uso |
|---|---|
| `main` | estado estável |
| `feat/*` | features |
| `fix/*` | correções |
| `docs/*` | documentação |
| `chore/*` | manutenção |

## Topics recomendados

- `detran-rj`
- `dtic`
- `governance`
- `private-by-default`
- `ai-agents`
- `sei`
- `patrimonio`
- `contratos`
- `academy`
- `infra`

## Vercel

- Projetos Detran devem ser protegidos por padrão.
- Deploy público somente com conteúdo sintético/aprovado.
- Secrets apenas via Vercel Environment Variables.
- Não usar dados reais de SEI, patrimônio ou contratos.

## Hugging Face

- Spaces privados por padrão.
- `Detran-RJ/detran-ai` deve ser privado.
- Datasets públicos somente sintéticos/anônimos.
- Token com escopo mínimo e rotacionado.

## GitHub Actions

Usar workflows reutilizáveis de `detran-infra` quando possível:

- secret scan;
- node quality;
- python quality;
- markdown quality.
