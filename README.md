# explorer-sumo-simulator :oncoming_automobile:

## Tópicos :zap:

- [Instalando no W10](pages/README.md) - Tutorial de configuração do SUMO e importação de um fluxo extraído do Open Street Map (OSM)

## Ferramentas :mag_right:

### Simulação :point_right: 

- [SUMO](https://sumo.dlr.de/docs/) - Aplicação para microsimulação de fluxo de veículos

### Editar rede viária :point_right: 

- [OSMWebWizard](https://sumo.dlr.de/docs/Tutorials/OSMWebWizard.html) - Exporta uma rede viária com um mapa real com um fluxo de tráfego aleatório para ser executado dentro do SUMO.
- [NETCONVERT](https://sumo.dlr.de/docs/netconvert.html) - Importa/exporta redes viárias para outros formatos (console application)
- [NETEDIT](https://sumo.dlr.de/docs/Netedit/index.html) - Editor de rede viária (GUI)
- [NETGENERATE](https://sumo.dlr.de/docs/netgenerate.html) - Gera redes abstratas para o SUMO

### Definir fluxo do tráfego :point_right: 

- [DUAROUTER](https://sumo.dlr.de/docs/duarouter.html) - Calcula rota mais eficiente baseando-se no caminho mais curto
- [JTRROUTER](https://sumo.dlr.de/docs/jtrrouter.html) - Calcula rotas baseados no volume do tráfego e na junção dos cruzamentos
- [DFROUTER](https://sumo.dlr.de/docs/dfrouter.html) - Calcula rotas usando valores induzidos em laços de repetição
- [OD2TRIPS](https://sumo.dlr.de/docs/od2trips.html) - Importa matrizes O/D(Origem/destino) e as divide em um único veículo
- [ACTIVITYGEN](https://sumo.dlr.de/docs/activitygen.html) - Calcula a mobilidade desejada para uma população 

## Conceitos Básicos de Tráfego :vertical_traffic_light: 

### Insfraestrutura viária :construction:

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

#### Semafáros

- Fases e seus tempos
- Vias e faixas controladas
- Programações ao longo do dia

#### Outros elementos

- Viadutos/passagens subterâneas
- Estacionamentos
- Entradas e saídas de veículos

### Veículos :car:

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

### Viagens :airplane:

#### Demanda

- Quantidade de veículos por rota
- Desempenho do pelotão (bloco uniforme ou distribuído)
- Distribuição temporal dos veículos (quantidade de veículos por tempo trafegam)
- Comportamento do bloco (agressivos ou pacientes)
- Tipos de veículos

#### Rota

- Itinerário
- Alterações
