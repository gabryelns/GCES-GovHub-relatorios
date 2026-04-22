# Diário de Bordo – Maria Eduarda Denis 

**Disciplina:** Gerência de Configuração e Evolução de Software (GCES)  
**Equipe:** Gov Hub BR  
**Comunidade/Projeto de Software Livre:** Gov Hub BR  

---

## Sprint 0 – [06/04/2026 – 20/04/2026]

### Resumo da Sprint
Esta sprint foi dedicada ao reconhecimento da arquitetura do projeto GovHub BR, mapeamento das ferramentas de Gerência de Configuração e superação dos obstáculos técnicos para configurar o ambiente de desenvolvimento em sistema operacional Windows. O foco principal foi garantir a paridade do ambiente local com a stack tecnológica da comunidade através da containerização.

### Atividades Realizadas

| Data  | Atividade | Tipo | Link/Referência | Status |
| ----- | --------- | ---- | --------------- | ------ |
| 16/04 | Estudo da arquitetura Medallion e leitura do E-book | Estudo | [E-book GovHub](https://github.com/govhub-br/ebook) | Concluído |
| 20/04 | Troubleshooting de instalação do Docker no Windows | Infra | PowerShell Admin | Concluído |
| 20/04 | Setup manual de dependências e variáveis (.env) | Código | Docker Compose | Concluído |
| 20/04 | Mapeamento de Issues e Labels no repositório oficial | Discussão | GitHub Issues | Concluído |

---

### Detalhamento das Atividades Realizadas

Para consolidar a configuração do ambiente e validar as atividades no projeto GovHub, realizei testes e validações locais focadas na infraestrutura Docker. Abaixo estão detalhadas as etapas principais:

#### 1. Containers Docker em Execução
Resultado do comando `docker-compose up -d` mostrando o status saudável (healthy) e o download das imagens, provando que a stack completa do Data Warehouse (Airflow, Jupyter, PostgreSQL e Superset) foi montada corretamente.

![Pull das imagens](./assets/status_docker_01.png)
![Containers ativos](./assets/status_docker_02.png)
*Fonte: Maria Eduarda Denis Duarte*

#### 2. Interface do Airflow Validada
Painel de login do Apache Airflow em execução local (localhost:8080). A página foi habilitada após a configuração manual das variáveis de ambiente e do arquivo `.env`, permitindo o acesso ao orquestrador de DAGs.

#### 2. Interface do Airflow Validada
Acesso garantido à interface web do Apache Airflow em localhost:8080.

![Interface Airflow](./assets/airflow_login.png)  
*Fonte: Maria Eduarda Denis Duarte*

#### 3. Mapeamento da Comunidade
Análise das demandas atuais e etiquetas de padronização utilizadas pelos mantenedores.

![Issues Mapeadas](./assets/mapeamento_issues.png)
![Labels de Padronização](./assets/labels_comunidade.png)
*Fonte: Maria Eduarda Denis Duarte*

---

### Maiores Avanços
* **Orquestração de Ambiente:** Sucesso na configuração da aplicação localmente, superando barreiras de permissões específicas do Windows.
* **Mapeamento de GCES:** Entendimento da comunicação entre os containers e identificação de como o projeto utiliza o Poetry e Makefile para gerência de configuração.
* **Governança:** Compreensão das políticas de qualidade e padrões exigidos pela documentação oficial (Guia de Contribuição).

### Maiores Dificuldades
* **Conflitos de Sistema:** Erros de segurança na pasta `ProgramData` do Windows que impediram a instalação inicial do Docker Desktop.
* **Ambiente Windows:** Ausência do comando `make` nativo, exigindo a execução manual dos scripts de instalação e a criação manual do arquivo `.env` para suprir as variáveis de ambiente.

### Aprendizados
* **Intervenção em Containers:** Manipulação de shell em ambientes containerizados para diagnóstico de falhas.
* **Fluxo de Contribuição:** Entendimento prático do uso de Conventional Commits e labels para organização de backlogs em larga escala.
* **Resolução de Dependências:** Gerenciamento de bibliotecas Python via Poetry em ambientes isolados.

### Plano Pessoal para a Próxima Sprint
- [ ] Identificar e selecionar uma "Good First Issue" no repositório oficial.
- [ ] Contribuir com pelo menos 1 Pull Request focado em melhorias de infraestrutura ou documentação.
- [ ] Participar da revisão de código (Code Review) de um colega da equipe.