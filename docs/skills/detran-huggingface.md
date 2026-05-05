# Skill — Detran Hugging Face Seguro

## Objetivo

Operar Spaces, datasets e modelos do Detran-RJ no Hugging Face com segurança institucional.

## Regras

- Spaces privados por padrão.
- Datasets públicos somente sintéticos/anônimos.
- Nunca subir documentos reais do SEI, patrimônio ou contratos.
- Usar `HF_TOKEN` com escopo mínimo.
- Rotacionar token exposto antes de uso operacional.

## Fluxo para `Detran-RJ/detran-ai`

1. Confirmar token HF com permissão na org `Detran-RJ`.
2. Criar Space privado com SDK Docker.
3. Sincronizar ignorando `.env`, bancos locais e dados.
4. Configurar secrets no Space.
5. Validar build.
6. Documentar URL e escopo no knowledge-base.

## Comando local esperado

```bash
# usar script administrativo local em _hf-admin para ensure/sync/audit
```
