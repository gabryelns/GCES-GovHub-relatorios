# Diário de Bordo – Gabriel Saraiva Canabrava

**Disciplina:** Gerência de Configuração e Evolução de Software (GCES)

**Equipe:** Gov Hub BR

**Comunidade/Projeto de Software Livre:** Gov Hub BR

---

## Sprint 0 – [06/04/2026 – 20/04/2026]

### Resumo da Sprint

Foco integral em configurar, inicializar e diagnosticar a infraestrutura principal do **Gov Hub BR** de forma local. Atuei desde a rodagem da documentação oficial (`Gitpage/govhub-dev`) até a estabilização completa da Stack de Dados (`app-lappis-ipea`), realizando deploy via Docker-Compose e conectando o Apache Superset ao Apache Airflow e Banco de Dados (PostgreSQL) interno. Enfrentei também o troubleshooting ativo de falhas nos drivers e dependências dos pipelines.

### Atividades Realizadas

| Data  | Atividade | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status |
| ----- | --------- | --------------------------------- | --------------- | ------ |
| 20/04 | Criação do fork | Código | [Link](https://github.com/gabrielsarcan/GCES-GovHub-relatorios) | Concluído |
| 20/04 | Estudo das políticas de contribuição e diretrizes do projeto | Estudo | [Guia de Contribuição](https://gov-hub.io/govhub/comunidade/guia-contribuicao/) | Concluído |
| 20/04 | Configuração do ambiente local | Código | [Guia de Instalação](https://gov-hub.io/govhub/documentacao/instalacao/#make-test) | Concluído |



### Detalhamento das Atividades Realizadas

Para consolidar a configuração do ambiente e validar as resoluções de problemas no projeto GovHub, realizei testes e validações locais. Abaixo estão detalhadas as etapas principais:

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">1. Rodando Interface da Plataforma GovHub</span></summary>

Página inicial do Gov Hub BR em execução local (localhost:8000), demonstrando os domínios disponíveis

![Site do GovHub Docs](assets/govhub.png)
<p align="center"><i><b>Fonte:</b> Gabriel Saraiva Canabrava</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">2. Containers Docker em Execução</span></summary>

Terminal listando o status saudável (healthy) via `docker ps` provando que a stack completa do Data Warehouse engatou corretamente.

![Containers Docker](assets/terminal.png)
<p align="center"><i><b>Fonte:</b> Gabriel Saraiva Canabrava</i></p>
</details>



<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">3. Configurando Variáveis no Airflow e Disparando DAG</span></summary>

Configuração das Variáveis Ambientais no Airflow mapeando `airflow_orgao` para "IPEA" garantindo que a rotina automatizada de extração efetuasse as requisições REST com a chave da Unidade Gestora correta.

![Airflow Variables](assets/airflow.png)
<p align="center"><i><b>Fonte:</b> Gabriel Saraiva Canabrava</i></p>
</details>



### Maiores Avanços
* Entendi a comunicação entre os vários contêineres e a identificação de *hostnames*.
* Consegui abrir o SQL Lab para operar consultas no schema alimentado pelo *Data Warehouse* interno.
* Aprendi a preencher as lacunas de um banco vazio configurando as variáveis corretas dentro do Apache Airflow e manipulando CLI Docker.

### Maiores Dificuldades
* Configuração sugerida nas documentações apontou conflito com os controles de pacotes do host Ubuntu (PEP-668 / *externally managed env*), exigindo o isolamento da instalação e execução via ferramentas específicas na máquina primária.
* Falta da extensão `psycopg2` na montagem do contêiner padrão do Apache Superset exigiu intervenção minuciosa diretamente do shell do container isolado.
* Entender primeiramente todo o fluxo inicial da arquitetura Medallion do projeto, identificando a falta de ingestão padrão de arquivos e localizando que a resposta aos inserts estava nos workers do Airflow.

### Aprendizados
* Intervenção e manipulação ágil dentro dos ambientes containerizados para instalar bibliotecas cruciais em serviços como Superset.
* Dinâmica e fluxo dos pipelines REST engatilhados por variáveis DAG para trazer dados reais até a montagem DW local.
* Identificação clara de dependências base do Python formatados para Data Environments com bibliotecas cruciais como o SQLAlchemy.

### Plano Pessoal para a Próxima Sprint
* [ ] Buscar good first issues para começar a contribuir.
* [ ] Contribuir com pelo menos 1 PR.
* [ ] Participar da revisão de código de um colega.