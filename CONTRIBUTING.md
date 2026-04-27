# Contribuindo para projetos DETRAN-RJ

Obrigado pelo interesse em contribuir! Este documento descreve como participar dos projetos da organização **Detran-RJ** no GitHub.

> Este arquivo vive em `.github/CONTRIBUTING.md` e é herdado por todos os repositórios da organização.

## Antes de começar

1. Leia o [Código de Conduta](./CODE_OF_CONDUCT.md).
2. Verifique se já existe issue/PR aberto sobre o assunto.
3. Para mudanças grandes, abra uma issue de discussão antes de codar.

## Fluxo padrão (Kaizen)

```
1. Issue  →  2. Discussão  →  3. Branch  →  4. PR  →  5. Review  →  6. Merge  →  7. Deploy
```

### 1. Abra (ou comente) uma issue
- **Bug:** descreva passos para reproduzir, comportamento esperado vs. atual, ambiente.
- **Feature:** descreva o problema, não a solução. Quem se beneficia? Qual o impacto?

### 2. Branch
```bash
git checkout -b feat/<descricao-curta>
# ou
git checkout -b fix/<descricao-curta>
```

Prefixos aceitos: `feat/`, `fix/`, `docs/`, `refactor/`, `test/`, `chore/`, `ci/`.

### 3. Commits — Conventional Commits

```
<tipo>(<escopo opcional>): <descrição imperativa em PT-BR>

[corpo opcional]
[footer opcional: Closes #123]
```

Exemplos:
- `feat(auth): adiciona login via gov.br SSO`
- `fix(api): corrige paginação ao filtrar por placa`
- `docs(readme): inclui seção de variáveis de ambiente`

### 4. Pull Request
- Título no mesmo formato Conventional Commit.
- Descrição: o que muda, por quê, como testar, screenshots se UI.
- Vincule a issue: `Closes #123`.
- CI deve estar verde.
- Pelo menos **1 review aprovado** (2 para mudanças sensíveis).

### 5. Review
- Reviewers do mesmo time têm 2 dias úteis para responder.
- Discordâncias resolvem-se na issue, não em discussão de código.
- Comentário com `nit:` é sugestão, não bloqueante.

## Padrões de código

| Tema | Regra |
|---|---|
| Linter | `npm run lint` deve passar sem warnings |
| Testes | Cobrir o caminho feliz + ao menos 1 erro esperado |
| Logs | Nunca logar PII (CPF, RG, placa do cidadão) em produção |
| Secrets | Nunca commitar `.env` ou chaves; usar GitHub Secrets |
| Idioma | Código em inglês; mensagens, docs e commits em PT-BR |

## Setup local

Cada repo tem seu próprio guia em `README.md`. Em geral:

```bash
git clone https://github.com/Detran-RJ/<repo>.git
cd <repo>
cp .env.example .env
npm install
npm run dev
```

## Reportar problemas de segurança

**Não abra issue pública.** Siga o processo em [SECURITY.md](./SECURITY.md).

## Dúvidas?

Abra uma issue com label `question` ou entre em contato com a equipe DTIC.
