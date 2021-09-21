# :oncoming_automobile: explorer-sumo-simulator

## 📝 Índice

- 0 - 🏁 [Introdução](#0-introducao) 
- 1 - ⚡ [Tópicos](#-1-tópicos)
- 2 - 🔧 [Ferramentas](#-2-ferramentas)
  - 2.1 [Simulação](#21-simulação)  
  - 2.2 [Rede Viária](#22-rede-viária)  
  - 2.3 [Fluxo do Tráfego](#23-fluxo-do-tráfego)
- 3 - 🚦 [Conceitos Básicos de Tráfego](#-3-conceitos-básicos-de-tráfego)
  - 3.1 [Infraestrutura Viária](#31-infraestrutura-viária)
  - 3.2 [Veículos](#32-veículos)
  - 3.3 [Viagens](#33-viagens)
- 4 - 📗 [Fontes](#-4-fontes)

## 0 🏁 Introdução

Com simulador SUMO é possível fazer simulações de trânsito. Entre outras funcionalidades ele permite:
- Definir diferentes veículos
- Definir limite de velocidade, faixas exclusivas da pista
- Tempo dos semáfaros
- Ciclos do transporte público
- Comportamento diferente do fluxo: quantidade, sentido
- Importar rede e dados de outros simuladores
- Gerar relatórios e estatísticas

 ## ⚡ 1 Tópicos 

- [Instalando no W10](pages/README.md) - Tutorial de configuração do SUMO e importação de um fluxo extraído do Open Street Map (OSM)

## 🔧 2 Ferramentas

### 2.1 Simulação

- [SUMO](https://sumo.dlr.de/docs/) - Aplicação para microsimulação de fluxo de veículos

### 2.2 Rede Viária

- [OSMWebWizard](https://sumo.dlr.de/docs/Tutorials/OSMWebWizard.html) - Exporta uma rede viária com um mapa real com um fluxo de tráfego aleatório para ser executado dentro do SUMO.
- [NETCONVERT](https://sumo.dlr.de/docs/netconvert.html) - Importa/exporta redes viárias para outros formatos (console application)
- [NETEDIT](https://sumo.dlr.de/docs/Netedit/index.html) - Editor de rede viária (GUI)
- [NETGENERATE](https://sumo.dlr.de/docs/netgenerate.html) - Gera redes abstratas para o SUMO

### 2.3 Fluxo do Tráfego

- [DUAROUTER](https://sumo.dlr.de/docs/duarouter.html) - Calcula rota mais eficiente baseando-se no caminho mais curto
- [JTRROUTER](https://sumo.dlr.de/docs/jtrrouter.html) - Calcula rotas baseados no volume do tráfego e na junção dos cruzamentos
- [DFROUTER](https://sumo.dlr.de/docs/dfrouter.html) - Calcula rotas usando valores induzidos em laços de repetição
- [OD2TRIPS](https://sumo.dlr.de/docs/od2trips.html) - Importa matrizes O/D(Origem/destino) e as divide em um único veículo
- [ACTIVITYGEN](https://sumo.dlr.de/docs/activitygen.html) - Calcula a mobilidade desejada para uma população 

## 🚦 3 Conceitos Básicos de Tráfego

### 3.1 Infraestrutura viária  

#### Vias

- Tipo de piso (asfaltadas, chão batido)
- Faixas de rolamento (quantidade, largura)
- Declividade
- Resistência do piso (peso suportado)
- Conexões e outras vias

#### Sinalização

- Permissões de tráfego (restrições a veículos por horário)
- Limites operacionais (regras de velocidade, movimentos permitidos)
- Avisos e informações

#### Semáfaros

- Fases e seus tempos
- Vias e faixas controladas
- Programações ao longo do dia

#### Outros elementos

- Viadutos/passagens subterâneas
- Estacionamentos
- Entradas e saídas de veículos

### 3.2 Veículos  

#### Características

- Dimensões
- Capacidade e carga transportada
- Desempenho (aranque, frenagem, velocidade máxima, consumo ...)
- Restrições de acesso (tipo de via exigida: trilhos, rio, mar, rampa, calçada, ciclovia)
- Poluição (sonora, gases)

#### Comportamento Condutor

- Agressividade
- Escolha de rotas (flexíveis ou fixas)
- Tempo de reação (tempo para reagir sinal verde, manter distância do veículo da frente)

### 3.3 Viagens

#### Demanda

- Quantidade de veículos por rota
- Desempenho do pelotão (bloco uniforme ou distribuído)
- Distribuição temporal dos veículos (quantidade de veículos por tempo trafegam)
- Comportamento do bloco (agressivos ou pacientes)
- Tipos de veículos

#### Rota

- Itinerário
- Alterações

## 📗 4 Fontes

- [Curso Udemy Ferramenta de Microssimulação de Tráfego SUMO](https://www.udemy.com/course/ferramenta-de-microssimulacao-de-trafego-sumo) de Ednardo de Oliveira Ferreira - Acessado Set/2021

