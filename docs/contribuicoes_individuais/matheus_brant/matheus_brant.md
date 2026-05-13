# Diário de Bordo – Matheus de Siqueira Brant

**Disciplina:** Gerência de Configuração e Evolução de Software (GCES)

**Equipe:** Gov Hub BR

**Comunidade/Projeto de Software Livre:** Gov Hub BR

---

## Sprint 0 – [06/04/2026 – 20/04/2026]

### Resumo da Sprint
Nesta sprint, o foco principal foi configurar o ambiente do projeto e entender melhor como funciona o processo de contribuição.

### Atividades Realizadas
| Data  | Atividade | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status |
| ----- | --------- | --------------------------------- | --------------- | ------ |
| 17/04 | Leitura e estudo da documentação do projeto | Estudo | [link - Documentação](https://gov-hub.io/govhub/sobre-projeto/overview/) | Concluído |
| 19/04 | Configuração inicial do ambiente | Código | [link - Guia de instalação](https://gov-hub.io/govhub/documentacao/instalacao/) | Concluído |
| 20/04 | Rastreamento de good first issues | Estudo | [link - GitHub](https://github.com/GovHub-br/data-application-gov-hub/issues) | Em andamento |

### Atividades realizadas - detalhamento 



<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">1
. Subindo o ambiente com `docker compose`</span></summary>

![docker](assets/imagem01.png)

<p align="center"></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">2
. Configuração do Airflow e Superset + conexão do superset com o banco de dados bem sucedida</span></summary>

![airflow](assets/imagem02.png)
![superset](assets/imagem03.png)
<p align="center"></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">3.Configurando e utilizando o Superset</span></summary>

![airflow](assets/imagem04.png)
![superset](assets/imagem05.png)
<p align="center"></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">4. Api contratos dag e dados carregados</span></summary>

![airflow](assets/imagem06.png)
![superset](assets/imagem07.png)
<p align="center"></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">5. Configurações dbt</span></summary>

![airflow](assets/imagem06.png)
![superset](assets/imagem07.png)
<p align="center"></p>
</details>

### Maiores Avanços
* Consegui finalizar na configuração do ambiente local.
* Entendi melhor a estrutura do repositório.
* Comecei a explorar as issues do projeto.
* Aprendi melhor como o projeto está organizado.

### Maiores Dificuldades
* A configuração do ambiente levou mais tempo do que eu esperava.
* Tive dificuldade com algumas dependências e comandos.
* Entendimento inicial do projeto.


### Aprendizados
* Fluxo de contribuição do projeto.
* Organização geral do repositório.
* Etapas para rodar o projeto localmente.

### Plano Pessoal para a Próxima Sprint
* [ ] Escolher uma issue para trabalhar.
* [ ] Contribuir com pelo menos 1 PR.
* [ ] Participar da revisão de código de um colega.

---

## Sprint 1 – [21/04/2026 – 04/05/2026]

### Resumo da Sprint
Nesta sprint, estudei a estrutura do GovHub até identificar uma oportunidade de contribuição na documentação. A partir disso, abri a issue [#104](https://github.com/GovHub-br/gov-hub/issues/104) e desenvolvi uma nova página chamada `Sistemas Integrados`.

O diferencial dessa entrega foi criar uma página prática e objetiva, complementar à página `Sistemas Estruturantes`. Enquanto a página já existente explica o contexto dos sistemas, a nova página apresenta um panorama direto das integrações já implementadas no projeto.

### Atividades Realizadas
| Data | Atividade | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status |
| ----- | --------- | --------------------------------- | --------------- | ------ |
| 21/04 - 23/04 | Estudo do repositório e da documentação até identificar uma oportunidade de contribuição | Estudo | GovHub BR | Concluído |
| 24/04 | Definição e abertura da issue sobre panorama das integrações do GovHub | Discussão/Doc | [Issue #104](https://github.com/GovHub-br/gov-hub/issues/104) | Concluído |
| 25/04 - 28/04 | Criação da página `Sistemas Integrados` no fork do projeto | Doc | [Issue #104](https://github.com/GovHub-br/gov-hub/issues/104) | Concluído |
| 29/04 | Ajuste do escopo da página para diferenciá-la de `Sistemas Estruturantes` | Doc | [Issue #104](https://github.com/GovHub-br/gov-hub/issues/104) | Concluído |
| 30/04 - 02/05 | Inclusão no menu e validação manual da documentação em ambiente local | Doc/Teste | [Issue #104](https://github.com/GovHub-br/gov-hub/issues/104) | Concluído |
| 04/05 | Abertura do Pull Request com a contribuição no fork | Doc | PR do fork GovHub | Concluído |

### Implementação da Issue #104

O foco desta entrega foi criar uma nova página de documentação voltada ao panorama das integrações existentes no GovHub.

As principais atividades foram:

- **Estudo do sistema:** analisei a estrutura do portal e da documentação até encontrar uma lacuna que pudesse ser tratada com uma contribuição pequena e útil.
- **Abertura da issue #104:** formalizei a proposta de criar uma página voltada às integrações já existentes no GovHub.
- **Criação da página `Sistemas Integrados`:** desenvolvi uma página com foco prático, listando sistemas e bases integrados.
- **Ajuste de escopo:** refinei o conteúdo para que a página não repetisse `Sistemas Estruturantes` e funcionasse como um inventário objetivo.
- **Validação local:** testei a navegação e o carregamento da página no ambiente local da documentação.

### Maiores Avanços
* Identifiquei uma oportunidade de contribuição após estudar o sistema.
* Criei uma página complementar à documentação existente, sem repetir o conteúdo conceitual.
* Validei a contribuição localmente antes de abrir o PR.
* Relacionei a entrega à issue #104 do repositório principal.

### Maiores Dificuldades
* No início, a página ficou muito parecida com `Sistemas Estruturantes`.
* Foi necessário entender a navegação do `mkdocs.yml` para posicionar corretamente a nova página.
* A validação precisou ser feita com Docker Compose, e não com `mkdocs` direto.

### Aprendizados
* Entendi melhor a organização da documentação do GovHub.
* Aprendi a diferenciar uma página conceitual de uma página de inventário prático.
* Pratiquei o fluxo de contribuição com fork, issue, commit e Pull Request.
* Aprendi a validar localmente um portal MkDocs com Docker Compose.

### Comprobatórios da Issue #104

- Página criada: `docs/sobre-projeto/sistemas-integrados.md`
- Item adicionado ao menu em `mkdocs.yml`
- Issue aberta no repositório principal: [#104](https://github.com/GovHub-br/gov-hub/issues/104)
- Pull Request aberto a partir do fork para o repositório GovHub

### Plano Pessoal para a Próxima Sprint
* [ ] Acompanhar a revisão do Pull Request e responder aos comentários dos mantenedores.
* [ ] Buscar uma nova contribuição no GovHub, preferencialmente envolvendo documentação ou integração de dados.
