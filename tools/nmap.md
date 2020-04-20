# Nmap

> uso: nmap [Scan Type(s)][options] {target specification}

| Args                        | Descrição                                               |
| --------------------------- | ------------------------------------------------------- |
| `-A`, `-o`                  | descrobir o sistema operacional e a versão              |
| `-T4, -F`                   | executar mais rápido, menos portas                      |
| `-p <port-ranges>`          | scaneia apenas as portas específicadas. EX: -p22, 80... |
| `--exclude-ports <ports>`   | exclui as postas especificadas.                         |
| `-sV`                       | testa as portas abertas, verifica os serviços           |
| `-f`                        | spoofing de firewall/IDS                                |
| `-S <IP_Address>`           | passa um ip de origem falso                             |
| `--spoof-mac <mac address>` | falsifique seu endereço MAC                             |
| `-6`                        | abilita scanner de ipv6                                 |
| `-sS/sT/sA/sW/sM`           | varredura TCP SYN/ACK/...                               |
| `--traceroute`              | rastreia o caminho do salto para cada host              |
|                             |                                                         |
