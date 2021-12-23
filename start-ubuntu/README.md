# setup-sumo-ubuntu

Tutorial simples, para realizar a configuração da ferramenta de simulação SUMO (Version 1.10.0) em sistema operacional Linux nas derivações Debian/Ubuntu.

## Pré-Requisito

Instalação do Python e outras libs úteis

    sudo apt-get install cmake python g++ libxerces-c-dev libfox-1.6-dev libgdal-dev libproj-dev libgl2ps-dev swig

## Instalação do SUMO

    sudo add-apt-repository ppa:sumo/stable
    sudo apt-get update
    sudo apt-get install sumo sumo-tools sumo-doc
    /usr/share/sumo/tools/osmWebWizard.py

Criando rede de simulação com mapa importado do Open Street Map (OSM)

    /usr/share/sumo/tools/osmWebWizard.py

Colocar no campo de busca local desejado para a simulação, clicando em `Search`, com o resultado selecionar a área desejada e clicar em `Generate Scenario`.
Pode-se ainda escolher alguns itens opcionais para importar junto com a simulação como o sistema do transporte público e o tráfego de veículos gerados (caminhões, motos, trens, bicicletas etc...

![image](ubuntu.gif)

## Fonte

SUMO [doc Linux](https://sumo.dlr.de/docs/Installing/Linux_Build.html). Acessado em Dezembro 2021.

UNICAMP [tutorial Hello World](https://cst.fee.unicamp.br/sites/default/files/sumo/sumo-roadmap.pdf). Acessado em Dezembro 2021.
