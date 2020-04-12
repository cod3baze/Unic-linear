# Terminal

> se quer saber oque um comando faz so digitar (`man nome_do_comando`)

[programar para bash](https://devhints.io/bash)

---

## Shell

> executa comandos no sistema

- pode executar no shell:
  - bibários do sistema
  - scripts com permisão
  - comandos

---

## Snippets

Abaixo os Snippets para iniciante

|                         Comando | Descrição                                            |
| ------------------------------: | ---------------------------------------------------- |
|                         `woami` | retorna o usuário logado                             |
|                   `ls` ou `dir` | mostra os diretórios existente da pasta atual        |
|                         `ls -l` | mostra os diretórios de forma mais detalhada         |
|                `ls -a` ou `-la` | mostra até os diretórios ocultos                     |
|               `touch "arquivo"` | cria um novo arquivo                                 |
|        `mkdir "nome diretorio"` | cria um novo diretório                               |
|                `cd "diretorio"` | muda de diretório                                    |
|                   `rm file.txt` | apaga arquivo                                        |
|                    `rm -Rf dir` | deleta o dir e seus arquivos                         |
|             `mv file.txt /dir2` | move file.txt para dir2                              |
|                           `pwd` | exibe o diretório atual                              |
|                `less "arquivo"` | abri o arquivo no terminal                           |
| `echo "mensagem" > arquivo.txt` | grava mensagem em aquivo.txt                         |
|    `echo "nova" >> arquivo.txt` | grava a msg no final em aquivo.txt                   |
|               `cat arquivo.txt` | concatena arquivos                                   |
|           `tail -f arquivo.txt` | monitora aquivo.txt mostrando o comteudo no terminal |

---

### hashs | anotações

\| `$` : denota uma variável de abiente | - EX: `cd $HOME` muda para Variável HOME. |

| `~` : referece a var HOME | - EX: `cd ~/Docs` muda para o diretório Docs na variável HOME |

---

### Rel

- `link simbólico`: é um atalho para algum caminho | arquivo
- `usr`: unix system resources
- `dir`: diretório
- `|`: pipe
- `grep`: globally search a regular expression and print

### packages instalados

- FOR DEVELOPER
  - `silversearch-ag`: mesmo que o comando grep. (expressão regular)
  - `build-essencial`
  - `default-jdk`
  - `libssl-dev`
  - `exuberant-ctags`
  - `ncurses-term`
  - `ack-grep`
  - `fontconfig`
  - `imagemagick`
  - `libmagickwand-dev`
  - `software-properties-common`
  - `git`
  - `vim-gtk3`
  - `curl`

---

### anotações

| diretorio, arquivo | função, descrição                             |
| ------------------ | --------------------------------------------- |
| **vmlinuz**        | o kernel do linux                             |
| **~/dev**          | ficam os dispositivos: drive, USB, PenDrive.. |
| `df -h`            | mostra os dispositivos que estao montados     |
| **/root**          | dir do superusuario                           |
| **/opt**           | onde alguns programas são instalados          |
| **/sbin**          | programas/binário do sistema                  |
| **/bin**           | outros programas simples do Sistema           |
| **/usr**           | fica maior parte das aplicações instaladas    |
| **/tmp**           | ficam coisas temporárias                      |
| `ps aux`           | processos acontecendo no sistema              |

---

### Globally

| command             | instruction                     |
| ------------------- | ------------------------------- |
| `grep "text"`       | expressão regular               |
| `chmod +X file.txt` | da alguma permissão no file.txt |

### exemplos

- [x] mostra nos processos do sistema apenas os que termiam com "bash"
      `ps aux | grep bash`

- [x] mostra a segunda coluna nos processos que terminam com bash
      `ps aux | grep bash | awk '{ print $2 }'`

---

### sudo

| Uso                               | Descrição                             |
| --------------------------------- | ------------------------------------- |
| `sudo apt upgrade`                | atualiza os pacotes necessários       |
| `sudo apt dist-upgrade 'package'` | Atualiza algum pacote particularmente |
| `su 'user'`                       | muda de user. ex: `su root`           |
|                                   |                                       |
|                                   |                                       |
|                                   |                                       |
|                                   |                                       |

---

### estrutura de listagem dos arquivos

> comando `ls -l`

ex:
`Permissões` | `links` | `proprietário` | `Grupo` | `tamanho` | `data e hora` | `Nome`
drwxr.xr-x | 2 | elias | alias | 4067 | Abril 11 22:50 | Música

- Permissões

proprietario | grupo | outros
`rwx` :---------: `r-x` :--: `r-x`

`r`: read (leitura)
`w`: write (Escrita)
`x`: Execution (Execução)
`-`: Sem permissão

1º caractere (tipo do arquivo)

- `d` = dir
- (`-`) = arquivo comum de user
- `c` = arquivo de caractere
- `b` = arquivo de bloco
- `l` = link (atalho)

## Alterar permissões de acesso em arquivos

- Síntaxe
  - `chmod [permissões] [arquivo]`

permissões

**orden:** `rwx`

- Execução: 1
- Escrita: 2
- Leitura: 4

Em bit:
111 : `1 = ligado` / `0 = desligado`

ex:

| permissão | equivalente à |
| --------- | ------------- |
| --x       | 1             |
| -W-       | 2             |
| r--       | 4             |

OU:

- [x] `rw-`
      110 = 4 + 2 = `6`
- [x] `rwx`
      111 = 4 + 2 + 1 = `7`

| instrução             | descrição                                           |
| --------------------- | --------------------------------------------------- |
| `chmod 000 teste.txt` | retira toda permissão do arquivo teste.txt          |
| `chmod 777 teste.txt` | concede todas as pemissões para o arquivo teste.txt |

---

## commands

| Comando                           | Descrição                                                                          |
| --------------------------------- | ---------------------------------------------------------------------------------- |
| `uname -r`                        | mostra a versão do kernel                                                          |
| `lsb_release -a`                  | versão do sistema instalado                                                        |
| `sed -i 's/velha/nova/g' arquivo` | substituir a ocorrência de uma determinada palavra em um arquivo (velha para nova) |
| `cut [opcção] arquivo`            | "cortar" campos ou colunas selecionados de cada linha de um arquivo                |
| `head -n15 arquivo`               | mostra as 15 primeiras linhas de um arquivo                                        |
| `cut -d'' -f2 file | head -5n`    | no file corta o especificado e joga a saída no head                                |
