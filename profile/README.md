<div align="center">

# DTIC — Detran-RJ

**Tecnologia pública, governança, segurança e automação a serviço do cidadão fluminense.**

[Site oficial](https://www.detran.rj.gov.br) · [Serviços](https://www.detran.rj.gov.br/_servico/) · [Ouvidoria](https://www.detran.rj.gov.br/_inst/ouvidoria/)

</div>

## Objetivo

A organização `Detran-RJ` reúne sistemas e documentação técnica relacionados à DTIC, com foco em governança, segurança, LGPD, automação e rastreabilidade.

Conteúdo institucional e dados operacionais são privados por padrão.

## Estrutura atual

| Repositório | Estado | Responsabilidade |
|---|---|---|
| `detran-rj-portal` | Ativo e privado | Monorepo dos sistemas internos |
| `.github` | Ativo e público | Perfil e configuração da organização |

O `detran-rj-portal` é a fonte de verdade para Portal, Guardian, patrimônio e Wiki. Repositórios antigos já consolidados não devem continuar listados como ativos.

## Convenções

| Item | Padrão |
|---|---|
| Branch principal | `main` |
| Organização | Um domínio institucional, um monorepo canônico |
| Segurança | Privado por padrão |
| Dados sensíveis | Nunca publicar bases, documentos internos, credenciais ou dados pessoais |
| Mudanças críticas | Revisão e testes antes de incorporar à `main` |
| Histórico | Git e documentação na Alexandria, sem branches permanentes de backup |

## Credenciais e publicação

- credenciais reais nunca entram em README, issue, PR ou commit;
- tokens expostos devem ser tratados como comprometidos e rotacionados;
- logs devem remover cookies, tokens e dados pessoais;
- material público precisa usar dados aprovados, sintéticos ou anonimizados.

---

<div align="center"><sub>Governo do Estado do Rio de Janeiro</sub></div>
