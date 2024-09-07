# Chat em Rede Local

## Descrição

Este é um aplicativo de chat simples que permite a comunicação entre vários clientes em uma rede local (LAN). O sistema utiliza uma arquitetura cliente-servidor, onde o servidor central gerencia as mensagens enviadas e recebidas pelos clientes conectados.

### Funcionamento:
- O **servidor** é responsável por escutar conexões e transmitir as mensagens enviadas por qualquer cliente a todos os outros clientes conectados.
- Os **clientes** se conectam ao servidor e podem enviar e receber mensagens em tempo real.

## Tecnologias Utilizadas
- **Python 3**
- Bibliotecas padrão:
  - `socket`: Para gerenciar conexões de rede.
  - `threading`: Para permitir a comunicação simultânea entre múltiplos clientes.

## Funcionalidades
- Suporte para múltiplos clientes conectados ao mesmo tempo.
- Comunicação em tempo real através de uma rede local (LAN).
- Transmissão de mensagens de um cliente para todos os outros conectados.
- Interface de texto simples via terminal.

## Como Executar

### Pré-requisitos
- **Python 3** instalado.
- Computadores conectados à mesma rede local (LAN).

### 1. Executando o Servidor
Primeiro, inicie o servidor que ficará responsável por gerenciar as conexões de clientes.

```bash
python server.py
```

### 2. Conectando os Clientes

Em cada máquina cliente, execute o seguinte comando para conectar-se ao servidor e começar a enviar mensagens. Será necessário fornecer o endereço IP do servidor.

```bash
python cliente.py
```

Nota: Para descobrir o endereço IP do servidor, utilize o comando ipconfig no Windows ou ifconfig no Linux/Mac.

### Estrutura do Projeto
├── servidor.py
└── cliente.py
