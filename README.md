# Portfólio de QA — Érika

Analista de QA em formação (Engenharia de Software). Experiência prática em testes **manuais** de front-end e API em uma plataforma SaaS de gestão de clínicas: validação de formulários, testes de integração com API, regressão e registro de bugs (média de ~13 bugs/semana reportados).

## O que você vai encontrar aqui
| Área | Foco | Pasta |
|---|---|---|
| Formulários (Login e Cadastro) | Critérios A–F, validações, responsividade, estados de botão | `projetos/projeto-saude-plataforma/formularios` |
| Validações do marketplace/paciente | Feedback visual, erros do backend, loading, desktop/mobile | `projetos/projeto-saude-plataforma/validacoes` |
| Integração com API (Pacientes/Prontuário) | CRUD, 403/404, fluxo de ativação por e-mail | `projetos/projeto-saude-plataforma/integracao-api` |
| Back-end / API | Rotas de cargos e permissões, prontuário com anexos, vínculo médico ↔ procedimento | `projetos/projeto-saude-plataforma/backend-api` |

## Resumo dos testes
| ID | Tema | Tipo | Status |
|---|---|---|---|
| VITTA-393 | Notificações do módulo Comunicação | Manual / UI | Executado |
| Formulário de Login | Critérios A–F (7 itens) | Manual / UI | Concluído — 1 bug |
| Formulário de Cadastro | Validações de campos, senha, backend, mobile | Manual / UI | Concluído — 1 bug |
| F5-08 | Integração API de Pacientes + Prontuário | Manual / API + UI | Relatório com evidências |
| F5-12 | API de cargos e permissões (`/role`) | Manual / API | Aprovado |
| F5-16 (back) | Prontuário: card por consulta + anexos | Manual / API | Em teste |
| F5-16 / VITTA-434 | Validação de inputs do paciente (front) | Manual / UI | Escopo definido |
| Procedimentos do médico | GET/PUT de procedimentos vinculados | Manual / API | Em teste |

## Ferramentas e técnicas
Teste manual · DevTools (responsividade e rede) · teste de API (rotas REST) · análise de valor-limite · particionamento de equivalência · relatório de bug · rastreabilidade por ticket (Jira/branch).

## Estrutura do repositório
```
qa-portfolio/
├── README.md
├── templates/          # modelos de caso de teste e de bug
├── evidencias/         # prints e PDFs (anonimizados)
└── projetos/
    └── projeto-saude-plataforma/
        ├── formularios/
        ├── validacoes/
        ├── integracao-api/
        └── backend-api/
```

> ⚠️ Nomes de empresa, URLs internas, dados de pacientes e credenciais foram omitidos ou anonimizados.
