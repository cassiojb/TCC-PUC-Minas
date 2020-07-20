# TCC-PUC-Minas

PONTIFÍCIA UNIVERSIDADE CATÓLICA DE MINAS GERAIS  
NÚCLEO DE EDUCAÇÃO A DISTÂNCIA  
Pós-graduação Lato Sensu em Ciência de Dados e Big Data  

**Cássio Luís José Barbosa**

**AGRUPAMENTO DE MUNICÍPIOS PARA LICITAÇÕES DE CONCESSÃO DE SERVIÇOS DE SANEAMENTO BÁSICO USANDO TÉCNICAS DE MACHINE LEARNING**

Campinas-SP  
**2020**

**PROBLEMA PROPOSTO**  

Em 15/07/2020 entrou em vigor o novo marco legal do saneamento básico (Lei nº 14.026, de 15 de julho de 2020). Essa lei possibilita a entrada da iniciativa privada na prestação de serviços de saneamento na forma de concessão ou licitação. Além disso prevê blocos de municípios do mesmo estado, que poderão contratar os serviços de forma coletiva. Municípios de um mesmo bloco não precisam ser vizinhos.  

Existem municípios que despertam maior interesse econômico nas licitações de concessão e outros que despertam pouco interesse. Existe o risco de pequenos municípios não encontrarem empresas interessadas em investir em saneamento básico se abrirem sozinhos um processo de licitação. Técnicas de "Machine Learning" podem nos ajudar a identificar municípios com alto interesse econômico para investimento em saneamento básico e outros com baixo interesse econômico. Dessa forma poderão se formar blocos de municípios com uma mescla desses dois tipos, aumentando as chances dos pequenos municípios de conseguirem aumentar sua infraestrutura de saneamento básico.  

Nesse trabalho identificaremos agrupamentos ("clusters") de municípios usando algoritmos de aprendizado não supervisionado tendo como entrada alguns atributos dos municípios que indicam a sua infraestrutura de saneamento básico atual. Testaremos dois algoritmos para isso: K-Means e DBScan. Os "clusters" atribuídos pelos algoritmos a cada município serão adicionados ao conjunto de atributos do município e funcionarão como atributos de classe para o passo seguinte. Tendo como entrada alguns atributos dos municípios junto com o atributo classe gerado pelo algoritmo que apresentar o melhor resultado de agrupamento alimentaremos o algoritmo de aprendizado supervisionado "Árvore de Decisão". A ideia de se usar o algoritmo "Árvore de Decisão" é inferir regras humanamente inteligíveis de agrupamento. Como detalharemos em seguida, devido às grandes diferenças demográficas entre as regiões do Brasil, essa técnica deve ser aplicada por região. No nosso estudo de caso escolhemos a região Nordeste para aplicar a técnica de agrupamento, mas qualquer região poderia ser analisada mudando apenas um parâmetro do modelo.
