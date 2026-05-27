# Diário de Bordo – Ana Letícia Melo Pereira

**Disciplina:** Gerência de Configuração e Evolução de Software (GCES)

**Equipe:** Gov Hub BR

**Comunidade/Projeto de Software Livre:** Gov Hub BR

---

## Sprint 0 – [06/04/2026 – 20/04/2026]

### Resumo da Sprint

Nesta sprint inicial, o foco foi a preparação do ambiente de desenvolvimento no WSL. O processo envolveu a clonagem do repositório da aplicação de dados do Gov Hub, a configuração de ferramentas de gerenciamento de versões de Python (pyenv) e de dependências (Poetry), culminando na subida do ambiente via containers Docker.

### Atividades Realizadas

| Data | Atividade | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status |
| --- | --- | --- | --- | --- |
| 07/04 | Clonagem do repositório `data-application-gov-hub` | Código | [GitHub](https://github.com/analeticiaa/data-application-gov-hub.git) | Concluído |
| 07/04 | Instalação e configuração do `pyenv` e `python 3.11` | Configuração | – | Concluído |
| 08/04 | Instalação do `Poetry` via `pipx` para gestão de pacotes | Configuração | – | Concluído |
| 08/04 | Execução do setup do projeto e orquestração Docker | Código | Makefile / Docker Compose | Concluído |

### Maiores Avanços

* **Isolamento de Ambiente:** Consegui configurar o `pyenv` com sucesso no WSL, garantindo que a versão do Python do projeto (3.11) não conflite com a do sistema operacional.
* **Automação de Build:** Utilizei o `make setup` para automatizar as tarefas iniciais, facilitando a padronização do ambiente conforme as diretrizes de GCES.
* **Orquestração:** Subi os serviços do projeto utilizando Docker Compose em modo *detached* (`-d`).
* **Acessos:** Acessei o Airflow e o Jupyter.

### Maiores Dificuldades

* **Dependências de Compilação:** Inicialmente, houve a necessidade de instalar diversas bibliotecas de sistema (`build-essential`, `libssl-dev`, etc.) para que o `pyenv` pudesse compilar o Python corretamente.
* **Configuração do Shell:** Foi necessário editar o `.bashrc` e recarregar as variáveis de ambiente para que o comando `pyenv` fosse reconhecido globalmente.
* **Configuração do Shell:** Inicialmente, eu tentei subir tudo pelo terminal do Windows, mas, devido às complicações encontradas durante as instalações, preferi seguir a instalação utilizando o WSL, que ajudou muito.

### Aprendizados

* **Gerenciamento de Versões:** Entendimento da diferença entre versões globais e locais com `pyenv local`.
* **Gestão de Dependências Modernas:** Uso do `Poetry` em substituição ao pip tradicional para maior controle de builds reprodutíveis.
* **Integração WSL/Windows:** Uso do comando `code .` para integrar o terminal Linux com o VS Code no Windows.

### Plano Pessoal para a Próxima Sprint

* [ ] Explorar a estrutura de diretórios do projeto `data-application-gov-hub`.
* [ ] Analisar os testes automatizados existentes no repositório.
* [ ] Realizar o primeiro commit de contribuição ou ajuste de documentação.

---

### Detalhamento Técnico (Bastidores)

Para fins de registro, os principais passos executados foram:

1. **Preparação:** `sudo apt update` e instalação de dependências de compilação.
2. **Pyenv:** Instalação via script `curl`, configuração de PATH no `.bashrc` e instalação da versão `3.11`.
3. **Poetry:** Instalação via `pipx` para isolamento da ferramenta de build.
4. **Projeto:** Clone do repo, definição de versão local (`pyenv local 3.11.15`) e subida do ambiente com `make setup` e `docker compose up -d`.
