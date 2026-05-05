# Credenciais — política segura Detran-RJ

## Regra principal

Não registrar credenciais reais neste repositório, no GitHub, em issues, PRs, READMEs ou chats.

## Onde guardar

| Plataforma | Local correto |
|---|---|
| GitHub Actions | Repository/Organization Secrets |
| Vercel | Project Environment Variables |
| Hugging Face | Space Secrets |
| VPS/servidores | Secret manager, SSH key protegida, variáveis de ambiente |
| Desenvolvimento local | `.env` local ignorado por Git |

## Proibido

- Tokens GitHub, Hugging Face, Vercel, OpenAI, Anthropic, Gemini etc.
- Senhas de banco, VPS ou painel.
- URLs com usuário/senha.
- Chaves privadas SSH.
- Dumps de banco ou `.db` locais.
- `.env` real.

## Permitido

- `.env.example` com placeholders.
- Nome da variável esperada.
- Descrição do uso.
- Link para painel onde configurar a variável, sem valor.

## Variáveis padrão por domínio

### Vercel

```env
VERCEL_TOKEN=<configurar-no-secret-manager>
VERCEL_ORG_ID=<configurar-no-secret-manager>
VERCEL_PROJECT_ID=<configurar-no-secret-manager>
```

### Hugging Face

```env
HF_TOKEN=<configurar-com-escopo-minimo>
HF_SPACE_REPO=Detran-RJ/detran-ai
```

### LLM providers

```env
OPENAI_API_KEY=<secret>
ANTHROPIC_API_KEY=<secret>
GOOGLE_API_KEY=<secret>
OPENROUTER_API_KEY=<secret>
```

### Banco

```env
DATABASE_URL=<secret>
```

## Rotação

Quando uma credencial for exposta:

1. Revogar imediatamente no provedor.
2. Criar nova credencial com escopo mínimo.
3. Atualizar apenas nos secret managers.
4. Remover do histórico, se tiver entrado no Git.
5. Registrar incidente sem repetir o valor do segredo.

## Checklist antes de PR

- [ ] `rg` local por padrões de segredo.
- [ ] Sem `.env` real.
- [ ] Sem URL com senha.
- [ ] Sem PDF/base sensível.
- [ ] CI de secret scan passando.
