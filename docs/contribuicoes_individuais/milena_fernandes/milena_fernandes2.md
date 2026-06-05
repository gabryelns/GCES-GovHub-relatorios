

## Sprint 2 – [12/05/2026 – 26/05/2026]

### Resumo da Sprint

Sprint dedicada à contribuição no projeto Gov Hub BR. Implementei minha segunda feature junto com o [Lucas Martins](/contribuicoes_individuais/lucas_martins/lucas_martins.md): um helper para enviar notificações de falhas de tasks do Airflow via Telegram. A feature foi implementada, testada e teve um pull request aberto no repositório principal do projeto.

### Atividades Realizadas

| Data  | Atividade                                      | Tipo (Código/Doc/Discussão/Outro) | Link/Referência                                                                      | Status    |
|-------|------------------------------------------------|-----------------------------------|-------------------------------------------------------------------------------------|-----------|
| 23/05 | Análise da issue #293 de Telegram                | Análise                           | [Issue #293](https://github.com/GovHub-br/data-application-gov-hub/issues/293)       | Concluído |
| 24/05 | Implementação do helper de notificação via Telegram | Código                            | [telegram_helpers.py](https://github.com/martinsglucas/data-application-gov-hub/blob/feat/webhook-alerta-telegram/airflow_lappis/helpers/telegram_helpers.py)         | Concluído |
| 24/05 | Testes da feature e abertura de PR              | Código                            | [PR #321](https://github.com/GovHub-br/data-application-gov-hub/pull/321)            | Concluído |
| 02/0 | Documentação do diário de bordo                 | Documentação                      | -                                                                                    | Concluído |

### Detalhamento das Atividades Realizadas

Os seguintes prints documentam o processo de desenvolvimento da feature de notificações via Telegram:

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">1. Issue #293 - Observabilidade com Telegram</span></summary>

Issue de feature que propõe a implementação de um webhook do Airflow para notificar falhas de tasks via Telegram

![Issue #293 - Observabilidade com Telegram](../lucas_martins/assets/sprint-2/issue.png)
<p align="center"><i><b>Fonte:</b> Lucas Martins</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">2. Fork do Repositório</span></summary>

Fork do repositório data-application-gov-hub criado para realização das contribuições

![Fork do Repositório](../lucas_martins/assets/sprint-2/fork.png)
<p align="center"><i><b>Fonte:</b> Lucas Martins</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">3. Dashboard do Airflow</span></summary>

Dashboard do Airflow exibindo os logs de execução da DAG api_contratos_dag com as tasks relacionadas à feature implementada

![Dashboard do Airflow](../lucas_martins/assets/sprint-2/airflow.png)
<p align="center"><i><b>Fonte:</b> Lucas Martins</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">4. Implementação da Feature - telegram_helpers.py</span></summary>

Código da implementação do helper para envio de mensagens via Telegram, incluindo função de callback para notificar falhas de tasks

![Implementação - telegram_helpers.py](../lucas_martins/assets/sprint-2/code.png)
<p align="center"><i><b>Fonte:</b> Lucas Martins</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">5. Notificação de Falha via Telegram</span></summary>

Screenshot da notificação de falha recebida no Telegram, mostrando detalhes da DAG, task, data de execução, erro e logs

![Notificação de Falha via Telegram](../lucas_martins/assets/sprint-2/alerta.png)
<p align="center"><i><b>Fonte:</b> Lucas Martins</i></p>
</details>

<details>
<summary><span style="font-size: 1.25em; font-weight: bold; cursor: pointer;">6. Pull Request #321 - Webhook Alerta Telegram</span></summary>

Pull request com a implementação completa da feature de notificações de falhas do Airflow via Telegram

![Pull Request #321](assets/pr_issue_293.png)
<p align="center"><i><b>Fonte:</b> Milena Rocha</i></p>
</details>

### Maiores Avanços

* Segundo pull request aberto no projeto Gov Hub BR.
* Implementação bem-sucedida de feature de observabilidade com Telegram para o Airflow.
* Compreensão da arquitetura e fluxo de desenvolvimento do projeto Gov Hub BR.

### Maiores Dificuldades

* Sem maiores dificuldades significativas, mas o processo de configuração do ambiente local e entendimento da estrutura do projeto exigiu um esforço inicial considerável.

### Aprendizados

* Arquitetura do projeto Gov Hub BR e seu pipeline de dados.
* Integração de webhooks do Airflow para observabilidade e notificações.
* Uso de bibliotecas externas (httpx) para fazer requisições HTTP.
* Uso do bot do Telegram

### Plano Pessoal para a Próxima Sprint

- [ ] Revisar feedback do PR #321 e implementar melhorias sugeridas
- [ ] Trabalhar em novas features ou bug fixes relacionados ao projeto
- [ ] Aprofundar conhecimento em Airflow DAGs e tasks
- [ ] Colaborar com outros membros da equipe em code reviews


    


