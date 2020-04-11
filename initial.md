# Passos de iniciante

> a prática leva ao aprimoramento, só depende de você.

## passos para se tornar um pentester

- [x] cybersegurança: Tecnicas, vetores, truques, perfis de ameaças e a anatomia de cyberattacks.
- [x] Hardware e rede.
- [x] sistemas operacionais, base de dados.
- [x] Aplicações, incluindo web apps e APIs.
- [x] Analista de dados: analise de problemas de segurança e apresentação de soluções

## Dicas

- leia livros e blogs
- aprenda Linux/Unix
- junta-se a comunidade
- aprenda programação
- pratica hacking em labs de testes

---

## Port

- em rede, uma porta é um ponto final de comunicação. Em nível de software uma porta é uma contrução lógica que identifica um tipo de serviço de rede.

## Server

- um servidor é um computador sedignado para processar requisições e entregar dados para outros computadores na internet ou em rede local.

## MAC ADDRESS VS IP ADDRESS

| `MAC`              | `IP`            |
| ------------------ | --------------- |
| Endereço físico    | Endereço lógico |
| endereço de 48 Bit | 32 ou 128 Bit   |
| cammada OSI 2      | camada OSI 3    |
| Fixo               | Pode mudar      |
| por fabricante     | por ISP         |

---

## Ferramentas que automatizam um teste

- Exploit DB
- Burp suite
- Zed attack proxy
- Aircrack-ng
- SQLmap
- Nmap
- Wireshark
- Metasploit
- THC Hydra
- Jhon the Ripper
- Meterpreter

## Ferramentas

- [x] `mitmproxy`: (proxy) analisa o tráfego http\s

- [x] `iptables`: (firewall) filtro de rede em pacotes

- [x] `arpspoof`: redireciona pacotes de um host de destino na LAN destinado a outro host na LAN, forjando respostas ARP.

- [x] `SSLSplit`: é um proxy TLS/SSL genérico transparente, para performatizar ataques **man-in-the-middle** em todos os tipos de protocolos de segurança.

- [x] `kismet`: detector de rede, farejador de pacotes, e detector de intrusão.

- [x] `Hashcat`: quebra passwords.

- [x] `Nikto`: é um scaner de servidor web que performatiza compreensões de testes contra serves web de multiplos items.

### MITMproxy

- [x] **interativo**: modifica requisições e respostas
- [x] **extensível**: invoca módulos python para conteudo especializado
- [x] **solicitações** de requisições e/ou respostas
