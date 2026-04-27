# Política de Segurança — Detran-RJ

## Reportando uma vulnerabilidade

A segurança dos sistemas do DETRAN-RJ é prioridade institucional. Se você identificou uma vulnerabilidade em qualquer projeto desta organização:

### ❌ NÃO

- Abrir uma issue pública.
- Discutir o problema em chats públicos, redes sociais ou comentários de PR.
- Explorar a vulnerabilidade além do mínimo necessário para confirmar sua existência.
- Acessar, modificar ou destruir dados de terceiros.

### ✅ SIM

1. **Envie um email para** moises.costa@detran.rj.gov.br com:
   - Descrição clara da vulnerabilidade
   - Passos para reproduzir
   - Impacto potencial estimado
   - Sugestão de mitigação (se houver)
   - Se quer ser creditado publicamente após o fix
2. **Aguarde retorno** em até 5 dias úteis com ack inicial.
3. **Mantenha sigilo** até o fix ser publicado e a comunicação coordenada.

## Fluxo de resposta

```
Recebimento  →  Triagem (CVSS) →  Fix  →  Patch coordenado  →  Disclosure público
   ≤ 5d           ≤ 10d           SLA por severidade        após patch
```

| Severidade | SLA Fix |
|---|---|
| Crítica (CVSS 9-10) | 7 dias |
| Alta (CVSS 7-8.9) | 30 dias |
| Média (CVSS 4-6.9) | 90 dias |
| Baixa (CVSS < 4) | next minor |

## Escopo

Esta política cobre os repositórios públicos e privados sob `github.com/Detran-RJ` e os sistemas em produção do DETRAN-RJ acessíveis via internet.

**Fora de escopo:**

- Vulnerabilidades em dependências de terceiros já reportadas upstream (reporte ao mantenedor da dep).
- Engenharia social contra funcionários.
- Ataques DoS sem evidência de vulnerabilidade subjacente.
- Configuração local do usuário.

## Hall da Fama

Pesquisadores de segurança que reportarem vulnerabilidades válidas seguindo este processo serão listados (com seu consentimento) em `SECURITY-HALL-OF-FAME.md` após o disclosure coordenado.

## LGPD

Em caso de incidente envolvendo dados pessoais, o DPO (Encarregado de Dados) do DETRAN-RJ será acionado conforme Lei nº 13.709/2018 e a ANPD será notificada quando aplicável.

---

> Esta política é viva. Sugestões de melhoria via issue (sem expor vulnerabilidades) são bem-vindas.
