# APT: advanced packaging tool

> Software que permite o gerencimento de pacotes em distro Linux.

## funcionamento

Usa um arquivo que lista as **fontes** de onde ele obterá os pacotes.

- `/etc/apt/sorces.list`

| comando                   | descrição                                               |
| ------------------------- | ------------------------------------------------------- |
| sudo `apt update`         | atualiza as listas de pacotes existente                 |
| `apt -u upgrade`          | atualiza os pacotes (-u: ver os pacotes)                |
| `apt dist-upgrade`        | Atualiza a distribuição linux                           |
| `apt-cdrom add`           | add pacotes para entrada CD/DVD                         |
| `apt install tree`        | instala o pacote _tree_                                 |
| `apt remove tree`         | remove o pacote _tree_                                  |
| `apt clean`               | apaga todos os pacotes baixados                         |
| `apt autoclean`           | apaga todos os pacotes que não possam mais ser baixados |
| `apt autoremove`          | remove pacotes (sem utilidade, dependencias...)         |
| `apt -d`                  | baixa o arquivo mas não o instala                       |
| `apt-cache`               | trata os pacotes instalados                             |
| `apt-cache dump`          | lista todos os pacotes instalados                       |
| `apt -f install`          | verifica lista de dependencias quebradas e corrigi.     |
| `apt --purge remove tree` | remove o pacote e suas configurações                    |
| `apt-cache pkgnames`      | retorna os pacotes instalados                           |
| `apt-cache show tree`     | exibi as info do pacote _tree_                          |
| `apt-cache depends tree`  | mostra as dependências do tree                          |
| `apt-cache search pacote` | exibi o pacotes com esse nome                           |

## Variáveis de ambiente

Pemitem mudar o shell de váirias formas +ara adaptalos às necessidades do usuário.

EX:

| Variável | Descrição                                                      |
| -------- | -------------------------------------------------------------- |
| \$PS1    | Prompt da linha de comandos                                    |
| \$HOME   | Diretório **/home** de um usuário                              |
| \$PATH   | Lista de diretórios vasculhados quando um comando é executado. |

| comanods          | descrição                                    |
| ----------------- | -------------------------------------------- |
| `env`             | mostra as variáveis de ambiente              |
| `echo $VAR`       | mostra o conteúdo da \$VAR                   |
| `NOME = elias`    | cria uma variável de ambiemte (escopo local) |
| `export NOME`     | torna a variável NOME global                 |
| `PATH=$PATH:/var` | anexa **/var** as variável de ambiente       |
