<!-- README institucional da organização Detran-RJ no GitHub -->

<div align="center">

# DTIC — Detran-RJ

![Detran-RJ](https://img.shields.io/badge/DETRAN--RJ-005D9F?style=for-the-badge&logoColor=white)
![DTIC](https://img.shields.io/badge/DTIC-298098?style=for-the-badge&logoColor=white)
![Gov.RJ](https://img.shields.io/badge/Gov.RJ-02BF4F?style=for-the-badge&logoColor=white)

**Tecnologia pública, governança e automação a serviço do cidadão fluminense.**

[Site oficial](https://www.detran.rj.gov.br) · [Serviços](https://www.detran.rj.gov.br/_servico/) · [Ouvidoria](https://www.detran.rj.gov.br/_inst/ouvidoria/)

</div>

---

## Objetivo da organização

Esta organização centraliza projetos de tecnologia, IA, documentação e automação relacionados à DTIC/Detran-RJ, com prioridade para segurança, rastreabilidade, LGPD e governança institucional.

## Projetos ativos

| Domínio | Projeto | Descrição |
|---|---|---|
| Patrimônio | [`detran-patrimonio`](https://github.com/Detran-RJ/detran-patrimonio) | Sistema de patrimônio DTIC/DETRAN com dashboard, chatbot e levantamento 2026 |
| SEI | [`detran-sei`](https://github.com/Detran-RJ/detran-sei) | Monorepo SEI: pipeline e bundles por setor/funcionário/processo |
| SEI | [`detran-sei-pipeline`](https://github.com/Detran-RJ/detran-sei-pipeline) | Pipeline sanitizado para extração, validação, metadados e documentação SEI |
| Apps | [`detran-apps`](https://github.com/Detran-RJ/detran-apps) | Monorepo de aplicativos DETRAN-RJ: contratos, wiki e ferramentas DTIC |
| IA | [`detran-ai`](https://github.com/Detran-RJ/detran-ai) | Agentes Prometheus e Atlas para processos, patrimônio e conhecimento institucional |
| Infra | [`detran-infra`](https://github.com/Detran-RJ/detran-infra) | Infraestrutura, CI, governança, dev-env e identidade visual |

## Mapa operacional

```text
DTIC / DETRAN-RJ
├─ Patrimônio       → detran-patrimonio
├─ SEI              → detran-sei + detran-sei-pipeline
├─ Contratos/Apps   → detran-apps
├─ IA institucional → detran-ai
└─ Infra/Governança → detran-infra + .github
```

## Convenções

| Item | Padrão |
|---|---|
| Branch principal | `main` |
| Commits | Conventional Commits em português |
| Segurança | Não abrir issue pública com vulnerabilidade |
| Dados sensíveis | Nunca publicar `.env`, PDFs internos, bases extraídas ou dados pessoais |
| IA/HF | Spaces privados; datasets públicos somente sintéticos/anônimos |

## Segurança e LGPD

Consulte [`SECURITY.md`](../SECURITY.md). Vulnerabilidades devem ser reportadas de forma privada e coordenada.

---

<div align="center">

**🏛️ Governo do Estado do Rio de Janeiro**

<sub>Desenvolvido e mantido para uso institucional da DTIC/Detran-RJ.</sub>

</div>
