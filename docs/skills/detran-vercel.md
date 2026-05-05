# Skill — Detran Vercel Seguro

## Objetivo

Configurar e operar projetos Vercel do Detran-RJ sem publicar dados sensíveis.

## Quando usar

- Criar preview protegido.
- Configurar projeto Vercel.
- Revisar política de deploy.
- Auditar se um app pode ou não ser público.

## Passos

1. Confirmar classificação do conteúdo.
2. Garantir que não há dados reais de SEI, patrimônio ou contratos.
3. Garantir que `.env` não está versionado.
4. Configurar secrets no painel Vercel.
5. Ativar proteção de deployment quando aplicável.
6. Usar domínio público apenas para conteúdo aprovado.

## Comandos seguros

```bash
vercel project inspect <project> --scope <scope>
vercel project protection <project> --scope <scope>
```

## Bloqueios

Não fazer deploy público se houver:

- dados pessoais;
- documentos internos;
- credenciais;
- anexos reais;
- dumps de banco;
- conteúdo `classification: sensitive` ou `secret`.
