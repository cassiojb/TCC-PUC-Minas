# TCC-PUC-Minas

PONTIFÍCIA UNIVERSIDADE CATÓLICA DE MINAS GERAIS  
NÚCLEO DE EDUCAÇÃO A DISTÂNCIA  
Pós-graduação Lato Sensu em Ciência de Dados e Big Data  

**Cássio Luís José Barbosa**

**AGRUPAMENTO DE MUNICÍPIOS PARA LICITAÇÕES DE CONCESSÃO DE SERVIÇOS DE SANEAMENTO BÁSICO USANDO TÉCNICAS DE MACHINE LEARNING**

Campinas-SP  
**2020**

**PROBLEMA PROPOSTO**  

Em 24/06/2020 foi aprovado pelo Senado o novo marco legal do saneamento básico (PL 4.162/2019). Esse projeto possibilita a entrada da iniciativa privada na prestação de serviços de saneamento na forma de concessão ou licitação. Além disso prevê blocos de municípios dentro do estado, que poderão contratar os serviços de forma coletiva. Municípios de um mesmo bloco não precisam ser vizinhos. Técnicas de  "Machine Learning" podem nos ajudar a identificar grupos de municípios de forma que os blocos formados contenham municípios que despertam maior interesse econômico nos leilões de concessão junto com município que despertam menor interesse, de forma que os municípios com menor interesse não corram o risco de ficar sem empresas interessadas em participar da licitação.  

Nesse trabalho agruparemos os municípios usando algoritmos de aprendizado não supervisionado tendo como entrada alguns atributos dos municípios. Testaremos dois algoritmos para isso: K-Means e DBScan. O "cluster" atribuído pelos algoritmos a cada município será adicionado ao conjunto de atributos do município e funcionará como um atributo de classe para o passo seguinte. O algoritmo que apresentar o melhor resultado de agrupamento será submetido ao algoritmo de aprendizado supervisionado "Árvore de Decisão". A ideia de se usar o algoritmo "Árvore de Decisão" é obter regras humanamente inteligíveis que possam auxiliar na criação de  critérios de formação de blocos de municípios dentro dos estados. Devido às grandes diferenças demográficas entre as regiões do Brasil essa técnica foi aplicada por região do Brasil. No nosso estudo de caso escolhemos a região Nordeste para aplicar a técnica de agrupamento, mas qualquer região poderia ser analisada mudando apenas um parâmetro do modelo.