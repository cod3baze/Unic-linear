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
| **/opt**           | onde alguns programad são instalados          |
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
