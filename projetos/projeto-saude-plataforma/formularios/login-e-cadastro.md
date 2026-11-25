# Teste de formulários — Login e Cadastro
**Tipo:** manual, UI · **Roteiro:** critérios A–F · **Ambiente:** desktop + DevTools (mobile, largura mínima 298×512)

## Login (7 critérios)
| Item | Resultado |
|---|---|
| Estados do botão (item 7) | ✅ Aprovado |
| E-mail inexistente (item 5) | ❌ Falhou |

**BUG — E-mail inexistente redireciona para o Cadastro**
- Esperado: mensagem de erro genérica (sem revelar se o e-mail existe).
- Obtido: a aplicação redireciona o usuário para a tela de Cadastro.
- Observação: além da UX, expõe a existência/inexistência de contas.

## Cadastro
Campos: Nome, e-mail, celular, CPF, data de nascimento, senha, confirmar senha.

| Cenário | Resultado |
|---|---|
| E-mail sem `@` | testado |
| CPF repetido | testado |
| Celular incompleto | testado |
| Senha curta / longa | testado |
| Barra de força, confirmação de senha, erros do backend, loading, mobile | ✅ Passou |
| Data de nascimento 01/01/1900 e 01/01/1500 | ❌ Aceitas (deveriam ser rejeitadas) |
| "Continuar com Facebook" | ❌ Erro de configuração (`APP_ID` não configurado) |

**BUG — Datas de nascimento absurdas aceitas** → originou o ticket de endurecimento de validação (piso/teto de idade, CPF com dígitos verificadores, política de senha).

> Evidências: `evidencias/formularios/`
