# Skills operacionais — Detran-RJ

Este diretório reúne skills/padrões operacionais para agentes humanos e de IA trabalharem com segurança nos projetos Detran-RJ.

## Skills

| Skill | Arquivo | Finalidade |
|---|---|---|
| detran-vercel | [`detran-vercel.md`](./detran-vercel.md) | Deploy e gestão de projetos no Vercel (ambientes, domínios, variáveis de ambiente, rollback) |
| detran-huggingface | [`detran-huggingface.md`](./detran-huggingface.md) | Spaces, datasets e modelos no Hugging Face; publicação e versionamento |
| detran-seguranca | [`detran-seguranca.md`](./detran-seguranca.md) | Segurança, conformidade com LGPD e resposta a incidentes |
| detran-sei | [`detran-sei.md`](./detran-sei.md) | Processamento de documentos SEI, regras de pipeline e automações |

## Regra global

Skills **não contêm credenciais reais** (tokens, senhas, chaves de API). Qualquer exemplo deve usar valores fictícios ou variáveis de ambiente.

## Revisão periódica

As skills devem ser revisadas **trimestralmente** (a cada 3 meses) para garantir alinhamento com:

- Mudanças nas plataformas (Vercel, Hugging Face, SEI)
- Atualizações na política de segurança e LGPD do Detran-RJ
- Novas práticas adotadas pela organização

Responsável pela revisão: mantenedor(a) do repositório `.github`.

Registro de revisões: atualizar a data no topo de cada arquivo de skill revisado.
