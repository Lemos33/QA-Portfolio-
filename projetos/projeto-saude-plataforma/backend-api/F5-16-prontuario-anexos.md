# F5-16 (back) — Prontuário: um card por consulta + anexos
**Tipo:** manual, API · **Branch:** `feat/F5-16-prontuario-card-anexos` · **Prioridade:** alta

## Escopo
- `GET .../patients/:id/chart` → 1 evento por consulta (anexos com data, notas/evolução e exame no mesmo card)
- `POST .../appointments/:appointmentId/chart-files` → upload multipart (limite MVP: 5 arquivos × 10 MB)
- A clínica **não** exclui card, nota nem anexo

## Cenários sugeridos
| Cenário | Esperado |
|---|---|
| Upload dentro do limite | 201 + anexo no card |
| 6º arquivo / arquivo > 10 MB | rejeitado |
| Tentativa de exclusão | negada |
| Consulta de outra clínica | 403/404 |

**Status:** em teste.
