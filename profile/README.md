<!-- README institucional da organização Detran-RJ no GitHub -->

<div align="center">

# DTIC — Detran-RJ

![Detran-RJ](https://img.shields.io/badge/DETRAN--RJ-005D9F?style=for-the-badge&logoColor=white)
![DTIC](https://img.shields.io/badge/DTIC-298098?style=for-the-badge&logoColor=white)
![Gov.RJ](https://img.shields.io/badge/Gov.RJ-02BF4F?style=for-the-badge&logoColor=white)
![Privado por padrão](https://img.shields.io/badge/Privado%20por%20padr%C3%A3o-Seguran%C3%A7a-red?style=for-the-badge)

**Tecnologia pública, governança, segurança e automação a serviço do cidadão fluminense.**

[Site oficial](https://www.detran.rj.gov.br) · [Serviços](https://www.detran.rj.gov.br/_servico/) · [Ouvidoria](https://www.detran.rj.gov.br/_inst/ouvidoria/)

</div>

---

## Objetivo

A organização `Detran-RJ` centraliza projetos, documentação e automações relacionados à DTIC/Detran-RJ, com foco em:

- governança e rastreabilidade;
- segurança e LGPD;
- automação de processos internos;
- IA institucional privada;
- documentação técnica e operacional.

## Projetos ativos

| Domínio | Projeto | Descrição |
|---|---|---|
| Patrimônio | [`detran-patrimonio`](https://github.com/Detran-RJ/detran-patrimonio) | Sistema de patrimônio DTIC/DETRAN com dashboard, chatbot e levantamento 2026 |
| SEI | [`detran-sei`](https://github.com/Detran-RJ/detran-sei) | Monorepo SEI: pipeline e bundles por setor/funcionário/processo |
| SEI | [`detran-sei-pipeline`](https://github.com/Detran-RJ/detran-sei-pipeline) | Pipeline sanitizado para extração, validação, metadados e documentação operacional |
| Apps | [`detran-apps`](https://github.com/Detran-RJ/detran-apps) | Monorepo de aplicativos DETRAN-RJ: contratos, wiki e ferramentas DTIC |
| IA | [`detran-ai`](https://github.com/Detran-RJ/detran-ai) | Agentes Prometheus e Atlas para processos, patrimônio e conhecimento institucional |
| Infra | [`detran-infra`](https://github.com/Detran-RJ/detran-infra) | Infraestrutura, CI reutilizável, governança, dev-env e políticas de publicação |
| Conhecimento | [`knowledge-base`](https://github.com/Detran-RJ/knowledge-base) | Vault Obsidian privado, governança e futura wiki interna DTIC |
| Organização | [`.github`](https://github.com/Detran-RJ/.github) | Perfil público, templates, segurança e skills operacionais |

## Mapa operacional

```text
DTIC / DETRAN-RJ
├─ Patrimônio       → detran-patrimonio
├─ SEI              → detran-sei + detran-sei-pipeline
├─ Contratos/Apps   → detran-apps
├─ IA institucional → detran-ai
├─ Infra/Governança → detran-infra + .github
└─ Conhecimento     → knowledge-base
```

## Convenções

| Item | Padrão |
|---|---|
| Branch principal | `main` |
| Commits | Conventional Commits em português |
| Fluxo | issue → branch → PR → quality → merge |
| Segurança | Não abrir issue pública com vulnerabilidade |
| Dados sensíveis | Nunca publicar `.env`, PDFs internos, bases extraídas, dados pessoais ou credenciais |
| Hugging Face | Spaces privados por padrão; datasets públicos somente sintéticos/anônimos |
| Vercel/Cloudflare | Deploy protegido por padrão; público somente com dados sintéticos/aprovados |

## Credenciais e publicação

- Credenciais reais nunca devem ser colocadas em README, issue, PR, commit ou chat.
- Use GitHub Actions Secrets, Vercel Environment Variables, Hugging Face Space Secrets ou secret manager equivalente.
- Todo token exposto deve ser considerado comprometido e rotacionado.
- Conteúdo Detran é **privado por padrão**.

Consulte:

- [`SECURITY.md`](../SECURITY.md)
- [`docs/credenciais.md`](../docs/credenciais.md)
- [`docs/config/organizacao.md`](../docs/config/organizacao.md)
- [`docs/skills/`](../docs/skills/)

---

<div align="center">

**🏛️ Governo do Estado do Rio de Janeiro**

<sub>Desenvolvido e mantido para uso institucional da DTIC/Detran-RJ.</sub>

</div>
