# Diário de Bordo – Milena Fernandes Rocha

**Equipe:** Gov Hub BR
**Comunidade/Projeto de Software Livre:** Gov Hub BR

---

## Sprint 0 – [06/04/2026 – 20/04/2026]

### Resumo da Sprint

Esta sprint teve como foco a ambientação técnica no projeto, abrangendo a configuração do ambiente de desenvolvimento, análise da documentação oficial e compreensão da arquitetura de dados adotada pela plataforma.

Foi realizada a exploração dos pipelines existentes e da organização do repositório, com ênfase na estrutura de DAGs e no fluxo de ingestão de dados. Como resultado prático, foram desenvolvidas as primeiras DAGs, consolidando o entendimento sobre orquestração de workflows e integração entre componentes do sistema.

---

### Atividades Realizadas

| Data  | Atividade                                                            | Tipo   | Link/Referência                                                                                                 | Status    |
| ----- | -------------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------------- | --------- |
| 06/04 | Configuração do ambiente local (containers, dependências e serviços) | Código | [imagem](assets/dags.png)                                                                                       | Concluído |
| 08/04 | Estudo da documentação oficial e fluxo de contribuição               | Estudo | [Guia](https://gov-hub.io/govhub/comunidade/guia-contribuicao/)                                                 | Concluído |
| 12/04 | Análise da estrutura do repositório e pipelines de dados existentes  | Estudo | [fork de exploração](https://github.com/MilenaFRocha/data-application-cidades)                                  | Concluído |
| 13/04 | Criação de templates padronizados para issues (bug/feature)          | Código | [commit](https://github.com/GovHub-br/data-application-cidades/commit/61a36c70f40d2e3fd211749a9fb6cec04cc0b6cc) | Concluído |
| 15/04 | Desenvolvimento de DAGs para ingestão de dados (ETL inicial)         | Código | [branch](https://github.com/GovHub-br/data-application-cidades/commits/feature/ingestao-dados-habitacao/)       | Concluído |

---

### Maiores Avanços

* Compreensão da arquitetura do projeto, incluindo organização em camadas e separação entre ingestão, processamento e disponibilização de dados.
* Entendimento do funcionamento de pipelines orquestrados por DAGs, incluindo dependências entre tarefas e agendamento.
* Capacidade de configurar e executar o ambiente local com os serviços necessários (ex: banco de dados, orquestrador, containers).
* Implementação das primeiras DAGs de ingestão, aplicando conceitos básicos de ETL (extração, transformação e carga).
* Padronização inicial do processo de contribuição por meio da criação de templates para issues.

---

### Maiores Dificuldades

* Configuração do ambiente local, especialmente em relação a conflitos de portas, variáveis de ambiente e dependências entre serviços.
* Curva de aprendizado inicial na compreensão da estrutura das DAGs e do fluxo completo de execução dos pipelines.
* Entendimento das integrações entre os componentes do sistema (ex: fontes de dados, armazenamento e orquestração).

---

### Aprendizados

* Uso prático de GitHub em fluxo colaborativo: criação de branches, commits, issues e organização de contribuições.
* Estruturação de pipelines de dados utilizando DAGs, incluindo definição de tarefas, dependências e agendamento.
* Conceitos fundamentais de ETL aplicados ao contexto do projeto.
* Boas práticas iniciais de padronização e documentação em projetos de software livre.

---

### Plano Pessoal para a Próxima Sprint

* [ ] Submeter pelo menos 1 Pull Request com código revisado e validado.
* [ ] Participar ativamente de revisões de código (code review).
* [ ] Evoluir as DAGs desenvolvidas, incluindo tratamento de erros e validação de dados.
* [ ] Implementar testes básicos para garantir a confiabilidade dos pipelines.
* [ ] Aprofundar o entendimento sobre a arquitetura de dados do projeto (armazenamento e consumo).


