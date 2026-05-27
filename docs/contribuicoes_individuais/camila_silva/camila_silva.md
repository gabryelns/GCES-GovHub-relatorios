# Diário de Bordo – Camila Silva Cavalcante

**Disciplina:** Gerência de Configuração e Evolução de Software (GCES)

**Equipe:** Gov Hub BR

**Comunidade/Projeto de Software Livre:** Gov Hub BR

---

## Sprint 0 – [06/04/2026 – 20/04/2026]

### Resumo da Sprint

Durante esta sprint, que foi focada na organização do grupo e familiarização com o projeto. Realizei a criação do fork, estudei a documentação técnica e políticas de contribuição do projeto. Fiz a configuração completa do ambiente de desenvolvimento do projeto, incluindo a instalação e ajuste de ferramentas.

Durante esta sprint, que foi focada na organização do grupo e familiarização com o projeto. Realizei a criação do fork, estudei a documentação técnica e políticas de contribuição do projeto. Fiz a configuração completa do ambiente de desenvolvimento do projeto, incluindo a instalação e ajuste de ferramentas.

### Atividades Realizadas

| Data  | Atividade | Tipo  | Link/Referência | Status |

| Data  | Atividade | Tipo  | Link/Referência | Status |
| ----- | --------- | --------------------------------- | --------------- | ------ |
| 15/04 | Leitura e estudo da documentação do projeto | Estudo | [Documentação](https://gov-hub.io/govhub/sobre-projeto/overview/) | Concluído |
| 18/04 | Mapeamento das políticas de contribuição | Estudo | [Guia de Contribuição](https://github.com/GovHub-br/gov-hub?tab=contributing-ov-file) | Concluído |
| 19/04 | Leitura do E-book | Estudo | [E-book](https://gov-hub.io/govhub/ebook-viewer/) | Concluído |
| 19/04 | Fork do repositório | Código | [Fork](https://github.com/CamilaSilvaC/gov-hub) | Concluído |
| 19/04 | Configuração do ambiente | Código | [Guia de Instalação](https://gov-hub.io/govhub/documentacao/instalacao/) | Concluído |

### Detalhamento das Atividades Realizadas

Para garantir que o ambiente estava bem configurado e que o projeto GovHub funcionava corretamente, foram feitos testes práticos utilizando todos os componentes da arquitetura (Docker, Airflow, PostgreSQL, dbt e Superset). A seguir, estão descritas as principais etapas realizadas:

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">1. Execução do ambiente via Docker</span></summary>

Print da tela mostrando os containers do Docker.

![Docker](assets/docker.png)
<p align="center"><i><b>Fonte:</b> Camila Silva Cavalcante</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">2. Ingestão de dados com Airflow</span></summary>
Painel do Airflow mostrando as DAGs e a DAG api_contratos_dag executada.

![Airflow](assets/airflow.png)
<p align="center"><i><b>Fonte:</b> Camila Silva Cavalcante</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">3. Superset — Conexão com Banco e Exploração Inicial</span></summary>
Painel do Superset com a conexão com o banco PostgreSQL local configurada.

![Superset](assets/superset.png)
<p align="center"><i><b>Fonte:</b> Camila Silva Cavalcante</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">4. Configuração e Validação do DBT</span></summary>
O comando dbt debug foi executado com sucesso, validando os arquivos de configuração (profiles.yml e dbt_project.yml) e a conexão com o banco PostgreSQL.

![Dbt](assets/dbt.png)
<p align="center"><i><b>Fonte:</b> Camila Silva Cavalcante</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">5. Consultas no banco de dados</span></summary>
Mostra os resultados das consultas SQL executadas para validar e explorar os dados da tabela contratos.contratos.

![Dbt](assets/consultas.png)
<p align="center"><i><b>Fonte:</b> Camila Silva Cavalcante</i></p>
</details>

### Maiores Avanços

* Consegui configurar completamente um ambiente complexo utilizando Docker + WSL.
* Entendi melhor a organização do repositório.
* Entendimento prático do funcionamento do Airflow, PostgreSQL e dbt.

### Maiores Dificuldades

* Dificuldade ao configurar o ambiente por falta de dependências.
* Incompatibilidade de versão do Python (3.12 vs 3.11 exigido pelo projeto).


### Aprendizados


* Fluxo de contribuição do projeto.
* Como configurar ambientes de desenvolvimento usando Docker e WSL.
* Funcionamento básico do Airflow (DAGs, Variables, Connections).
* Percebi melhor como seguir o passo a passo da documentação ajuda a evitar erros na configuração.

### Plano Pessoal para a Próxima Sprint

* [ ] Analisar as issues e encontrar uma para contribuir.
* [ ] Atuar em conjunto com a **Luísa Ferreira** para o diagnóstico e resolução de problemas técnicos identificados na nossa issue.
* [ ] Analisar as issues e encontrar uma para contribuir.

## Sprint 1 – [21/04/2026 – 11/05/2026]

### Resumo da Sprint

Nesta sprint, trabalhei em conjunto com a Luisa no desenvolvimento do pipeline de extração dos dados de Unidades de Conservação do Censo 2022. Participei da análise das fontes de dados, desenvolvimento das tasks no Airflow, validação dos dados no PostgreSQL e testes de integração com o Superset. Todo o escopo foi implementado com sucesso.

### Atividades Realizadas

| Data | Atividade | Tipo | Link/Referência | Status |
| :--- | :--- | :--- | :--- | :--- |
| 30/04 | Análise das estruturas de dados do IBGE | Estudo | [FTP IBGE](https://ftp.ibge.gov.br/Censos/Censo_Demografico_2022/Unidades_de_Conservacao/) | Concluído |
| 03/05 | Colaboração no desenvolvimento da DAG | Código | Airflow | Concluído |
| 06/05 | Implementação da task de extração | Código | `extrair_dados_excel` | Concluído |
| 06/05 | Validação do armazenamento no PostgreSQL | Validação | Schema `censo_demografico` | Concluído |
| 07/05 | Testes de qualidade dos dados | Teste | Consultas SQL | Concluído |
| 08/05 | Validação das 19 tabelas criadas | Validação | Padrão `UN_CONS_*` | Concluído |
| 08/05 | Testes de acesso via Superset | Teste | SQL Lab | Concluído |

### Detalhamento das Atividades Realizadas

Para validar a implementação do pipeline, realizamos testes em cada etapa:

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">1. Execução da DAG de Extração</span></summary>

Print do Airflow mostrando a DAG `ingestao_ibge_unidades_conservacao_dag` em execução com sucesso, com as 3 tasks: listar_arquivos_ftp, extrair_dados_excel e limpar_e_inserir_dados.

![DAG Execution](assets/airflow_dag_execution.png)
<p align="center"><i><b>Fonte:</b> Camila Silva Cavalcante</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">2. Validação das Tabelas Criadas</span></summary>

Query SQL mostrando a listagem das 19 tabelas criadas no schema `censo_demografico` com o padrão de nomenclatura `UN_CONS_*`.

![Tables Validation](assets/tables_validation.png)
<p align="center"><i><b>Fonte:</b> Camila Silva Cavalcante</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">3. Verificação dos Dados no Superset</span></summary>

Consulta aos dados no Superset mostrando os dados demográficos de Unidades de Conservação extraídos e prontos para visualização.

![Data Verification](assets/data_verification.png)
<p align="center"><i><b>Fonte:</b> Camila Silva Cavalcante</i></p>
</details>

### Maiores Avanços

* Compreensão profunda da arquitetura de extração do GovHub;
* Sucesso na implementação colaborativa do pipeline;
* Validação bem-sucedida de todos os critérios de aceitação;
* Experiência com tratamento de dados governamentais;
* Domínio das ferramentas da stack de dados (Airflow, PostgreSQL, Superset).

### Maiores Dificuldades

* Compreensão inicial da estrutura complexa de dimensões dos arquivos;
* Tratamento de inconsistências nos formatos de dados;
* Otimização das queries para grandes volumes de dados.

### Aprendizados

* Desenvolvimento de DAGs complexas no Airflow;
* Técnicas de validação de dados em pipelines;
* Importância de testar cada etapa independentemente;
* Padrões de nomenclatura em projetos de dados;
* Colaboração efetiva em desenvolvimento em pares.

### Plano Pessoal para a Próxima Sprint

* [ ] Participar da revisão de código do Pull Request.
* [ ] Contribuir com sugestões de melhoria.
* [ ] Documentar o pipeline no repositório.
* [ ] Trabalhar na integração final com Luisa.
