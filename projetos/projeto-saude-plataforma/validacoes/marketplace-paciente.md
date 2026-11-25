# Revisão — Validações e feedback dos formulários (marketplace do paciente)
**Formulários:** Login, Cadastro, Agendamento, Edição de perfil · **Plataformas:** desktop e mobile

## Critérios de aceite
- Validações no front-end
- Tratamento de erros retornados pelo backend
- Estados habilitado/desabilitado dos botões
- Estados de loading
- Feedback visual para campos inválidos (vermelho padrão do sistema)
- Mensagens claras orientando a correção
- Comportamento consistente entre os formulários

## Ticket relacionado — validação de inputs do paciente (front)
- Escopo: nascimento (piso/teto de idade), CPF com dígitos verificadores, política de senha, telefone e nome — em cadastro, OAuth, perfil, dependentes e trocar/recuperar senha.
- Fora de escopo: OTP de cadastro, campo sexo, portal da clínica.

> Status Login/Cadastro: ver `../formularios/login-e-cadastro.md`. Agendamento e Edição de perfil: próximos na fila.
