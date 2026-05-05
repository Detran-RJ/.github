# Skill — Detran SEI Pipeline

## Objetivo

Trabalhar com documentação e automações relacionadas ao SEI sem expor dados reais.

## Regras

- PDFs, textos extraídos e metadados reais ficam fora de GitHub público.
- Repositório `detran-sei-pipeline` deve conter apenas estrutura sanitizada, docs e scripts seguros.
- Dados reais devem ir para storage privado com controle de acesso.

## Fluxo seguro

1. Separar código de dados.
2. Sanitizar exemplos.
3. Validar `.gitignore`.
4. Rodar secret scan.
5. Documentar processo sem anexar documentos reais.
6. Abrir PR vinculado à issue.

## Nunca publicar

- PDFs de processos.
- Textos extraídos de processos.
- Dados pessoais.
- Números/processos com contexto sensível sem autorização.
- Credenciais de sistemas internos.
