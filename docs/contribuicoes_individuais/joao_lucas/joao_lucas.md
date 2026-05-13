# Diário de Bordo – João Lucas Araujo Siqueira

**Disciplina:** Gerência de Configuração e Evolução de Software (GCES)

**Equipe:** Gov Hub BR

**Comunidade/Projeto de Software Livre:** Gov Hub BR

---

## Sprint 0 – [06/04/2026 – 20/04/2026]

### Resumo da Sprint
A Sprint 0 teve como principal objetivo a ambientação no projeto Gov Hub BR, com foco no entendimento da arquitetura, estudo das documentações e configuração do ambiente de desenvolvimento local. Durante esse período, consegui compreender o fluxo de contribuição do projeto, além de realizar a configuração do ambiente. 

### Atividades Realizadas
| Data  | Atividade | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status |
| ----- | --------- | --------------------------------- | --------------- | ------ |
| 15/04 | Leitura e estudo da documentação do projeto | Estudo | [link - Documentação](https://gov-hub.io/govhub/sobre-projeto/overview/) | Concluído |
| 17/04 | Configuração inicial do ambiente | Código | [link - Guia de instalação](https://gov-hub.io/govhub/documentacao/instalacao/) | Concluído |
| 19/04 | Rastreamento de good first issues | Estudo | [link - GitHub](https://github.com/GovHub-br/data-application-gov-hub/issues) | Em andamento |

### Maiores Avanços
* Consegui configurar e rodar todo o ambiente local utilizando Docker, incluindo serviços como Apache Airflow, Apache Superset e Jupyter.
![Containers Docker](./assets/airflow.png)
![Containers Docker](./assets/docker.png)
![Containers Docker](./assets/postgres.png)

* Entendi o fluxo completo do projeto de dados: ingestão (Airflow) → transformação (dbt) → visualização (Superset).
![Containers Docker](./assets/superset.png)


* Entendi melhor a organização do repositório, incluindo DAGs do Airflow, estrutura do dbt e configurações via .env.

### Maiores Dificuldades
* Problemas iniciais com dependências do ambiente (ex: conflito entre versões do Poetry e plugins).
* Entendimento inicial do fluxo entre múltiplas ferramentas (Airflow, dbt, Superset), que não é trivial.


### Aprendizados
* Como configurar conexões dentro do Airflow e do Superset.
* Boas práticas iniciais de padronização e documentação em projetos de software livre.
* Entendimento na prática do fluxo de contribuição e arquitetura do projeto.


### Plano Pessoal para a Próxima Sprint
* [X] Contribuir com pelo menos 1 PR.
* [ ] Participar da revisão de código de um colega.