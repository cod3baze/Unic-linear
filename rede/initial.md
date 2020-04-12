# Inicial em rede

> trasmissão/circulação de pacotes de pacotes

## modelo OSI

- Composto por 7 camadas:
  - [x] Aplicação
  - [x] Apresentação
  - [x] Sessão
  - [x] Transporte
  - [x] Rede
  - [x] Link de dados
  - [x] Física

## Encapsulamento

cabeçalhos contendo informações são adicionadas aos dados a serem transmitidos.
É empacotar dados com informações adicionais em cada camada.

ex: (cada camada coloca seu cabeçalho)

- [x] 1º: |**cabeçalho** | _dados_ |

- [x] 2º: |**cabeçalho** | _cabeçalho_ + _dados_ |

## protocol Data Unit - PDU

| Camada          | PDU      |
| --------------- | -------- |
| _aplicação_     |
| _Apresentação_  | Dados    |
| _Sessão_        |
| -------------   | -------- |
| _Transporte_    | Segmento |
| _Rede_          | Pacote   |
| _Link de dados_ | Quadro   |
| _Física_        | Bits     |
