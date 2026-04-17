# Diário de Bordo – Letícia de Cássia Hladczuk Rodrigues

**Disciplina:** Gerência de Configuração e Evolução de Software (GCES)

**Equipe:** Gov Hub BR

**Comunidade/Projeto de Software Livre:** Gov Hub BR

---

## Sprint 0 – [06/04/2026 – 20/04/2026]

### Resumo da Sprint
Essa sprint foi focada na familiarização com o projeto, o aprendizado do fluxo de contribuições e a configuração do ambiente.

### Atividades Realizadas
| Data  | Atividade | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status |
| ----- | --------- | --------------------------------- | --------------- | ------ |
| 15/04 | Leitura e estudo da documentação do projeto | Estudo | [link - Documentação](https://gov-hub.io/govhub/sobre-projeto/overview/) | Concluído |
| 17/04 | Configuração inicial do ambiente | Código | [link - Guia de instalação](https://gov-hub.io/govhub/documentacao/instalacao/) | Concluído |
| 17/04 | Rastreamento de good first issues | Estudo | [link - GitHub](https://github.com/GovHub-br/data-application-gov-hub/issues) | Em andamento |

### Maiores Avanços
* Consegui rodar a aplicação localmente. Containers Dockers rodando:

![Containers Docker](./assets/containersDocker.png)

* Entendi melhor a organização do repositório.

* Configuração do Airflow e Superset.


### Maiores Dificuldades
* Logo no início, tive problema com a versão do Python, precisando fazer o ajuste para a versão 3.11. 
![Erro Versão do Python](./assets/erro_pyVersion.png)

* Lidei com falha na compilação da biblioteca `openlineage-sql`, o que exigiu a instalação do `Visual Studio Build Tools` para compilar o código Rust/C++. 
![Erro Biblioteca Openlineage](./assets/erro_openlineage.png)

* Enfrentei erros de leitura de arquivos (`\r` invisível / formato CRLF) ao executar scripts `.sh` do projeto e ao configurar o Git Hooks no WSL.

### Aprendizados
* Entendimento na prática do fluxo de contribuição e arquitetura do projeto.
* Aprendi como a diferença de codificação de texto (CRLF vs LF) afeta a execução de scripts Bash em contêineres e como limpar esses arquivos via terminal.
* Melhoria na leitura de logs do Docker para diagnosticar falhas de dependência entre serviços.


### Plano Pessoal para a Próxima Sprint
* [ ] Buscar good first issues para começar a contribuir.
* [ ] Contribuir com pelo menos 1 PR.
* [ ] Participar da revisão de código de um colega.