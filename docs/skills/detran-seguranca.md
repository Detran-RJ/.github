# Skill — Detran Segurança e LGPD

## Objetivo

Revisar mudanças, documentos e deploys sob ótica de segurança, LGPD e publicação segura.

## Checklist

- [ ] Existe issue vinculada?
- [ ] O conteúdo tem classificação?
- [ ] Há dados pessoais?
- [ ] Há documento interno real?
- [ ] Há credenciais ou URLs com senha?
- [ ] O deploy é público ou protegido?
- [ ] O PR remove/evita `.env` real?
- [ ] O CI de secret scan passou?

## Classificação

| Classificação | Ação |
|---|---|
| `public` | pode publicar se aprovado |
| `internal` | privado por padrão |
| `private` | privado |
| `sensitive` | nunca publicar |
| `secret` | remover e rotacionar |

## Resposta a incidente

1. Parar deploy/publicação.
2. Remover segredo do repositório.
3. Recriar histórico se necessário.
4. Revogar/rotacionar credencial.
5. Registrar incidente sem repetir segredo.
