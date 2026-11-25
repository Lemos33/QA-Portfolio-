# Vínculo médico ↔ procedimento com customização
**Tipo:** manual, API · **Rotas:** `GET` e `PUT` em `/clinic/:clinicId/specialists/:specialistId/procedures`
**Campos customizáveis:** valor, % de repasse, planos, instruções · **Modos:** `inherit` / `custom`

## Cenários sugeridos
| Cenário | Esperado |
|---|---|
| GET sem customização | valores herdados (`inherit`) |
| PUT em modo `custom` | persiste e GET reflete |
| Voltar para `inherit` | customização descartada |
| Valores inválidos (negativo, % > 100) | rejeitados |

**Status:** em teste.
