# Diário de Bordo - Cardoso Evangelista Brandão

**Disciplina:** Gerência de Configuração e Evolução de Software (GCES)

**Equipe:** Gov Hub BR

**Comunidade/Projeto de Software Livre:** Gov Hub BR

---

## Sprint 0 – [06/04/2026 – 20/04/2026]

### Resumo da Sprint
Essa sprint inicial teve como foco a familiarização com o projeto Gov Hub e a configuração do ambiente do mesmo, ainda, de maneira mais coletiva o aprendizado do fluxo d>

### Atividades Realizadas
| Data  | Atividade | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status |
| ----- | --------- | --------------------------------- | --------------- | ------ |
| 16/04 | Criação do fork | Código | [Fork][link-Fork] | Concluído |
| 16/04 | Leitura do e-book | Estudo | [E-book][link-Ebook] | Concluído |
| 20/04 | Leitura e estudo da documentação do projeto | Estudo | [Documentação][link-Documentação] | Concluído |
| 20/04 | Configuração do ambiente | Código | [Configuração][link-Config] | Incompleto |
| 20/04 | Adicionando meu diário de bordo ao GitHub Pages | Documentação | - | Concluído |

### Detalhamento das Atividades Realizadas

Ao realizar a configuração do ambiente localmente eu consegui com que 2 das 3 ferramentas necessárias fossem abertas.

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">1. Rodando o Jupyter</span></summary>

Print da tela com o Jupyter aberto.

![Figura 1 - Jupyter Lab](./assets/sprint0/jupyter-telaInicial.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;"> 2. Superset rodando</span></summary>

Print da tela com o Superset aberto.

![Figura 2 - Superset](./assets/sprint0/superset-telaInicial.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">3. Airflow com problemas</span></summary>

Tive problemas ainda não solucionados com o Airflow, como é possível observar no print do terminal abaixo.

![Figura 3 - Erro não solucionado](./assets/sprint0/airflow-erro.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>
</details>

### Maiores Avanços
* Aprendi a rodar a maior parte da aplicação localmente;
* Entendi a organização do repositório após a leitura da documentação e do E-book disponibilizados pela equipe do Gov Hub.

### Maiores Dificuldades
* Dispositivo institucional não permitiu fazer a instalação do Docker, atrasei a configuração pois dependia exclusivamente do meu notebook pessoal, que não estava comigo;
* Abertura de ferramenta Airflow;
* Ambiente demorou para configurar por falta de dependências;
* Dispositivo pessoal não aguentou o uso do Docker.

### Aprendizados
* Fluxo de contribuição do projeto.

### Plano Pessoal para a Próxima Sprint
* [X] Solucionar a abertura da ferramenta Airflow.
* [X] Conferir as issues disponíveis para iniciar alguma contribuição.
* [X] Participar da revisão de código de um colega.
* [X] Preencher meu diário de bordo em paralelo as atividades realizadas (diminuir sobrecarga).

---

## Sprint 1 - [21/04/2026 - 04/05/2026]

### Resumo da Sprint

Nesta sprint continuei tentando resolver meus problemas com a configuração do ambiente GovHub. Descobri que o problema estava na minha máquina, que não suportava o Docke>

### Atividades realizadas

| Data  | Atividade | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status |
| ----- | --------- | --------------------------------- | --------------- | ------ |
| 02/05 - 03/05 | Configuração do 0 em máquina emprestada. | Configuração | [Configuração][link-Config] | Concluído |
| 04/05 | Pesquisas sobre possíveis issues para contribuição. | Estudo | [Issues][link-Issues] | Concluído |

### Detalhamento das atividades realizadas

Nessa sprint alcancei a configuração por completa do GovHub:

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">1. Airflow pós-login rodando</span></summary>

Print da tela com o Airflow pós-login.

![Airflow logado](./assets/sprint1/airflowRodando.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">2. Airflow configurado com o banco local</span></summary>

Print da tela com o Airflow pós-configurações e conexões.

![Airflow configurado com o banco local](./assets/sprint1/airflowConexaoRodando.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">3. Jupyter rodando</span></summary>

Print da tela com o Jupyter.

![Jupyter](./assets/sprint1/jupyterRodando.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">4. Superset pós-login rodando</span></summary>

Print da tela inicial do Superset logado.

![Superset logado](./assets/sprint1/supersetRodando.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">5. Superset com a conexão configurada</span></summary>

Print da tela com o Superset conectado.

![Superset conectado](./assets/sprint1/supersetConexaoRodando.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">6. dbt configurado</span></summary>

Print do terminal com a configuração do dbt.

![dbt](./assets/sprint1/dbt.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">7. Rodando modelo de contratos dbt</span></summary>

Print do terminal rodando modelos de contratos do dbt.

![Contratos dbt](./assets/sprint1/contratosDbt.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>
</details>

### Maiores Avanços

* Consegui configurar completamente o ambiente, após muita dificuldade.
* Pude praticar bastante o uso do WSL.
* Finalmente consegui voltar a atenção pras issues do projeto em si.

### Maiores Dificuldades

* O uso do Windows para rodar o projeto se mostrou bastante desafiador, precisei usar o WSL.
* Pouca experiência com WSL.

### Aprendizados

* Aprendi sobre a dificuldade de lidar com os problemas que usar Windows causou na configuração do projeto e contorná-los.
* Mais experiência com o uso do WSL.
* Funcionamento básico do Airflow.
* Funcionamento do padrão de issues.

### Plano Pessoal para a Próxima Sprint

* [X] Escolher após a análise feita nessa sprint uma issue para contribuir.
* [X] Iniciar projeto extra (UDA pipeline) explicado em sala.
* [X] Finalizar alguma atividade (extra, contribuição no GovHub, etc.).

---

## Sprint 2 - [05/05/2026 - 25/05/2026]

### Resumo da Sprint

Nessa sprint foi desenvolvido o projeto extra disponibilizado pela professora, que consistiu em desenvolver um pipeline automatizado que coletasse PDFs de relatórios trimestrais de incorporadoras (MRV, Direcional, Tenda), extraísse dados operacionais usando IA e disponibilizasse via API REST para alimentar um Boletim de Conjuntura do setor habitacional.
Para a resolução do problema, construí um sistema em três camadas: um coletor que varre os portais de RI das empresas diariamente e ignora PDFs já processados (via SHA-256); um motor de extração que usa PyMuPDF para ler o PDF e GPT-4 para interpretar os dados semanticamente (sem depender de posição ou formato do documento); e uma API FastAPI que entrega os dados filtrados por empresa, ano e trimestre. Todo dado extraído é rastreável até o PDF de origem, e 23 testes automatizados cobrem o pipeline sem necessidade de chave de API.

### Atividades realizadas

| Data | Atividade | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status |
|------|-----------|-----------------------------------|-----------------|--------|
| 07/05 | Leitura e análise do enunciado do projeto e do Boletim de Conjuntura 3T25 de exemplo | Estudo | [Boletim 3T25][link-ExtraBoletim] | Concluído |
| 07/05 | Definição da arquitetura: Full-Scan com PyMuPDF + GPT-4 + Instructor + FastAPI + APScheduler | Discussão | — | Concluído |
| 08/05 | Implementação do Contrato Semântico (`src/models.py`) com schema Pydantic, validações de range e blindagem contra alucinações | Código | [models.py][link-ExtraContratoSemantico] | Concluído |
| 10/05 | Implementação do Catálogo de Dados e Linhagem (`src/catalog.py`) com deduplicação SHA-256 dupla e data lineage por PDF | Código | [catalog.py][link-ExtraCatalogo] | Concluído |
| 12/05 | Implementação do Motor de Extração Full-Scan (`src/extractor.py`) com PyMuPDF + GPT-4o + system prompt com 7 regras semânticas | Código | [extractor.py][link-ExtraExtractor] | Concluído |
| 13/05 | Implementação dos Scrapers de RI e Scheduler (`src/collector.py`) para MRV, Direcional e Tenda com polling diário via APScheduler | Código | [collector.py][link-ExtraCollector] | Concluído |
| 17/05 | Implementação da API REST (`src/api.py`) com FastAPI, endpoints filtráveis por empresa/ano/trimestre e catálogo de linhagem | Código | [api.py][link-ExtraApi] | Concluído |
| 21/05 | Criação de 23 testes automatizados cobrindo contrato semântico, idempotência, CRUD e resiliência a dois layouts de PDF | Código | [tests/][link-ExtraTests] | Concluído |
| 21/05 | Validação local: 23/23 testes passando sem necessidade de API key | Teste | — | Concluído |

### Detalhamento das atividades realizadas

O link para o Fork onde foi adicionado todo o projeto extra desenvolvido pode ser encontrado [aqui][link-ExtraLinkGithub].

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">1. Resultado dos testes rodando</span></summary>

Print do terminal mostrando todos os testes passando.

![Testes gerais rodando](./assets/sprint2/extra04-1.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">2. Rodando sem precisar de API key</span></summary>

Print do terminal mostrando a execução do projeto ao não precisar de API key.

![Sem API key](./assets/sprint2/extra04-2.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">3. Rodando após injeção de dados</span></summary>

Print do resultado do terminal ao colocar o comando:

`# Todos os dados`
`curl -s "http://localhost:8000/api/conjuntura" | python3 -m json.tool`

![Resultado 1](./assets/sprint2/extra04-3.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>

Print do resultado do terminal ao colocar o comando:

`# Filtro por empresa`
`curl -s "http://localhost:8000/api/conjuntura?empresa=MRV" | python3 -m json.tool`

![Resultado 2](./assets/sprint2/extra04-4.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>

Print do resultado do terminal ao colocar o comando:

`# Filtro por ano e trimestre`
`curl -s "http://localhost:8000/api/conjuntura?ano=2025&trimestre=3" | python3 -m json.tool`

![Resultado 3](./assets/sprint2/extra04-5.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>

Print do resultado do terminal ao colocar o comando:

`# Status atualizado`
`curl -s "http://localhost:8000/api/status" | python3 -m json.tool`

![Resultado 4](./assets/sprint2/extra04-6.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>
</details>

### Maiores Avanços

* Desenvolvimento da solução por completo.
* Finalmente ter alguma task 100% feita na matéria.

### Maiores Dificuldades

* Indecisão na escolha de fazer a solução por FullScan ou Chunking.
* Pouca experiência em Python, tive que ir pesquisando tudo que fazia.
* Projeto com alta complexidade pra mim.

### Aprendizados

* Aprendi um pouco mais a utilizar Python.
* A integração com IA foi novidade pra mim.

### Plano Pessoal para a Próxima Sprint

* [X] Fazer mais algumas revisões, para garantir que está tudo certo no projeto extra.
* [X] Abrir PR do projeto extra.
* [X] Iniciar minha contribuição na issue escolhida.
* [X] Documentar tudo pendente no diário de bordo.

---

## Sprint 3 - [26/05/2026 - 08/06/2026]

### Resumo da Sprint

Nesta sprint, com o ambiente do Gov Hub já configurado nas sprints anteriores, voltei o foco para a primeira contribuição de código ao projeto. Analisei as issues abertas com o rótulo OSS (voltadas à comunidade), escolhi a issue [#309][link-Issue309] — que pedia a criação de testes unitários para o cliente `cliente_contratos.py` — e a desenvolvi do início ao fim: estudo do código a ser testado, implementação dos testes com mocks, validação local e abertura do Pull Request seguindo o guia de contribuição do projeto.

### Atividades realizadas

| Data | Atividade | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status |
|------|-----------|-----------------------------------|-----------------|--------|
| 26/05 | Análise das issues abertas e escolha da issue #309 (testes unitários para `cliente_contratos.py`) | Estudo | [Issue #309][link-Issue309] | Concluído |
| 03/06 | Comentário na issue manifestando interesse em assumi-la, conforme o guia de contribuição | Discussão | [Issue #309][link-Issue309] | Concluído |
| 03/06 | Estudo do `cliente_contratos.py` e da classe base `cliente_base.py` para entender o comportamento a ser testado | Estudo | — | Concluído |
| 04/06 | Implementação dos testes unitários cobrindo os seis métodos da classe `ClienteContratos`, com mocks do método `request` | Código | [test_cliente_contratos.py][link-TestContratoGovhub] | Concluído |
| 04/06 | Validação local: 18 testes passando, formatação (black) e lint (ruff) sem apontamentos, 100% de cobertura no arquivo-alvo | Teste | — | Concluído |
| 04/06 | Ajuste do fluxo de Git (rebase com `upstream/main`, padronização do commit) e abertura do Pull Request | Código | [Pull Request][link-PR1govhub] | Concluído |

### Detalhamento das atividades realizadas

A contribuição consistiu em escrever testes unitários para `airflow_lappis/plugins/cliente_contratos.py`. A classe `ClienteContratos` possui seis métodos, todos seguindo o mesmo padrão: realizam uma requisição HTTP por meio do método `request` (herdado de `ClienteBase`) e retornam a lista de dados apenas quando o status é 200 e o corpo da resposta é uma lista; caso contrário, retornam `None`.

Para cada um dos seis métodos, implementei três cenários de teste:
- **Sucesso:** status 200 com uma lista, esperando o retorno dos dados;
- **Status de erro:** status diferente de 200 (ex.: 404), esperando `None`;
- **Resposta fora do formato:** status 200 com um corpo que não é lista, esperando `None`.

Também validei que cada método chama o endpoint correto. As requisições foram simuladas com `unittest.mock`, sem nenhuma chamada real à API — atendendo ao pedido da issue por "mocks estruturados".

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">1. Comentário na issue manifestando interesse</span></summary>

Print do comentário deixado na issue #309 solicitando a atribuição, conforme orienta o guia de contribuição do projeto.

![Comentário](./assets/sprint3/comentarioIssue.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">2. Testes passando e cobertura do arquivo</span></summary>

Prints do terminal mostrando os 18 testes passando e a cobertura de 100% sobre `cliente_contratos.py`.

![Testes passando](./assets/sprint3/govhub-testesPassando1.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>

![Testes passando](./assets/sprint3/govhub-testesPassando.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">3. Verificação de formatação e lint</span></summary>

Print do terminal mostrando o arquivo aprovado em `black` e `ruff`, sem apontamentos.

![Black e Ruff](./assets/sprint3/govhub-blackRuffCheck.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">4. Pull Request aberto</span></summary>

Prints da página do Pull Request no repositório principal.

![PR](./assets/sprint3/govhub-printPR1.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>

![PR](./assets/sprint3/govhub-printPR2.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>

![PR](./assets/sprint3/govhub-printPR3.png)
<p align="center"><i><b>Fonte:</b> Anna Clara Brandão</i></p>
</details>

### Maiores Avanços

* Primeira contribuição de código ao Gov Hub levada do início ao fim, seguindo o fluxo completo do projeto (fork, branch, commit padronizado, rebase com o upstream e Pull Request).
* Cobertura de 100% do arquivo-alvo, com todos os métodos e cenários relevantes testados.
* Compreensão prática de como escrever testes unitários isolando dependências externas (API) com mocks.

### Maiores Dificuldades

* Os hooks de Git do projeto (pré-commit e pré-push) executam formatação e lint sobre o repositório inteiro, falhando por causa de problemas pré-existentes em arquivos não relacionados à minha contribuição. Precisei investigar a fundo para confirmar que meu arquivo estava correto e que os erros não eram meus, comparando com o estado original do `main` e verificando o CI do projeto.
* A configuração do `mypy` reportava o import como não encontrado quando rodado de forma isolada, comportamento que ocorre igualmente em todo o projeto e está ligado à forma como o `pythonpath` é resolvido.
* Pouca experiência prévia com `unittest.mock` e com o fluxo de rebase no Git.

### Aprendizados

* Como escrever testes unitários com `pytest` e `unittest.mock`, simulando respostas de uma API sem depender dela.
* Importância de validar uma contribuição isoladamente (apenas o arquivo alterado) quando as ferramentas de qualidade do projeto rodam sobre todo o repositório.
* Fluxo de manutenção de uma branch atualizada com o `upstream` via rebase, e a diferença entre os remotes `origin` (fork) e `upstream` (repositório principal).
* Convenções de Conventional Commits aplicadas tanto ao nome da branch quanto à mensagem de commit.

### Plano Pessoal para a Próxima Sprint

* [ ] Acompanhar o code review do Pull Request e implementar eventuais ajustes solicitados pelos mantenedores.
* [ ] Buscar uma segunda issue para contribuir.
* [ ] Manter o diário de bordo atualizado em paralelo às atividades.

[link-Documentação]: https://gov-hub.io/govhub/sobre-projeto/overview/
[link-Fork]: https://github.com/annacbrandao/gov-hub
[link-Ebook]: https://gov-hub.io/govhub/ebook-viewer/
[link-Config]: https://gov-hub.io/govhub/documentacao/instalacao/
[link-Issues]: https://github.com/orgs/GovHub-br/projects/4/views/1?filterQuery=oss
[link-ExtraBoletim]: https://github.com/unb-Sistemas-de-Machine-learning/Projetos-Individuais-2026-1/blob/main/projeto-individual-4/exemplo_Boletim_Conjuntura_2025_3T.pdf
[link-ExtraContratoSemantico]: https://github.com/annacbrandao/Projetos-Individuais-2026-1/blob/anna-brandao/projeto-4/anna-brandao/projeto-4/src/models.py
[link-ExtraCatalogo]: https://github.com/annacbrandao/Projetos-Individuais-2026-1/blob/anna-brandao/projeto-4/anna-brandao/projeto-4/src/catalog.py
[link-ExtraExtractor]: https://github.com/annacbrandao/Projetos-Individuais-2026-1/blob/anna-brandao/projeto-4/anna-brandao/projeto-4/src/extractor.py
[link-ExtraCollector]: https://github.com/annacbrandao/Projetos-Individuais-2026-1/blob/anna-brandao/projeto-4/anna-brandao/projeto-4/src/collector.py
[link-ExtraApi]: https://github.com/annacbrandao/Projetos-Individuais-2026-1/blob/anna-brandao/projeto-4/anna-brandao/projeto-4/src/api.py
[link-ExtraTests]: https://github.com/annacbrandao/Projetos-Individuais-2026-1/tree/anna-brandao/projeto-4/anna-brandao/projeto-4/tests
[link-ExtraLinkGithub]: https://github.com/annacbrandao/Projetos-Individuais-2026-1/tree/anna-brandao/projeto-4
[link-Issue309]: https://github.com/GovHub-br/data-application-gov-hub/issues/309
[link-PR1govhub]: https://github.com/GovHub-br/data-application-gov-hub/pull/339#issuecomment-4625996046
[link-TestContratoGovhub]: https://github.com/annacbrandao/data-application-gov-hub/blob/test/cliente-contratos/tests/test_cliente_contratos.py
