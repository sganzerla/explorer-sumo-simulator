# setup-sumo-ubuntu

Tutorial simples, para realizar a configuração da ferramenta de simulação SUMO (Version 1.10.0) em sistema operacional Linux nas derivações Debian/Ubuntu.

## Pré-Requisito

### SUMO

Instalação do simulador

    sudo apt-get install sumo sumo-tools sumo-doc

Testar se pograma foi instalado

    sumo-gui

Verificar se variável de ambiente está setada (deve retornar path do SUMO)

    echo $SUMO_HOME


### Python (3.8.10): 

Realizei a instalação da versão 3.8.10 (pode ser que versões mais novas ou mais antigas também funcionem)

Comando  para verificar versão instalada

    python --version

Comando para instalar 3.8 [by digitalocean](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-programming-environment-on-an-ubuntu-20-04-server-pt)

    sudo apt update
    sudo apt -y upgrade
    python3 -V

Para gerenciar os pacotes de software do Python, instalar o pip

    sudo apt install -y python3-pip

Kit de pacotes e ferramentas de desenvolvimento

    sudo apt install -y build-essential libssl-dev libffi-dev python3-dev

### Ambiente de desenvolvimento Python

Criar pasta em qualquer diretório

    mkdir environments
    cd environments

Criar um ambiente de desenvolvimento

    python3 -m venv my_env

Ativar o ambiente de desenvolvimento

    cd my_env
    source bin/activate

## Criando primeira simulação

Criar diretório de preferência

    cd home/user/Documentos/my_project
    sumo -c example.sumocfg

Criando rede de simulação com mapa importado do Open Street Map (OSM)

    /usr/share/sumo/tools/osmWebWizard.py

Colocar no campo de busca local desejado para a simulação, clicando em `Search`, com o resultado selecionar a área desejada e clicar em `Generate Scenario`.
Pode-se ainda escolher alguns itens opcionais para importar junto com a simulação como o sistema do transporte público e o tráfego de veículos gerados (caminhões, motos, trens, bicicletas etc...

![image](start-ubuntu/OSM.png)

## Fonte

Digital Ocean[Configurando Python](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-programming-environment-on-an-ubuntu-20-04-server-pt). Acessado em Dezembro 2021.

SUMO [doc Linux](https://sumo.dlr.de/docs/Installing/Linux_Build.html). Acessado em Dezembro 2021.

UNICAMP [tutorial Hello World](https://cst.fee.unicamp.br/sites/default/files/sumo/sumo-roadmap.pdf). Acessado em Dezembro 2021.