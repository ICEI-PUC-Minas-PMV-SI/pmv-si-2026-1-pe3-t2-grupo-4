# 1. INTRODUÇÃO

Desde 2019, o preço de carros novos aumentou aproximadamente 85% (BALCÃO AUTOMOTIVO, 2025). Isso tem levado os proprietários de veículos automotivos a manterem seus bens por mais tempo, necessitando cada vez mais de manutenções preventivas e corretivas. A média mensal de veículos atendidos em oficinas saiu de 80, em 2020, para 122 em 2024, segundo a mesma fonte. No cenário atual, manter um carro em boas condições se tornou mais viável do que comprar um veículo novo. Nesse contexto, os consumidores estão constantemente à procura de oficinas mecânicas de confiança, que têm ganhado cada vez mais importância.

O aumento no fluxo de serviços nas oficinas mecânicas exige a implementação de um modelo organizado e com priorização, visando um melhor desempenho e manter a competitividade no mercado. Nesse contexto, de acordo com Reparação Automotiva (2021a), diversos setores de prestação de serviços já têm adotado um sistema de agendamento. Contudo, muitos empresários do setor mecânico automotivo ainda são relutantes em adotar essa modernização, seja pela dificuldade de implementação desse modelo, pela cultura do setor ou pelo pensamento de alguns que acreditam que o sistema pode resultar em mais burocracia.

A implementação de um sistema de agendamento implica o amadurecimento da empresa, consequentemente afetando o seu crescimento. Segundo Reparação Automotiva (2021b), esse modelo de agendamento traz maior eficiência, controle e previsibilidade, proporcionando ao empresário uma visão antecipada da demanda, facilitando a gestão da compra de insumos e distribuição dos serviços, evitando prejuízos à produtividade. Além disso, uma agenda traz inúmeros benefícios, desde que implementada de maneira correta.

## 1.1. Problema

Nesse momento você deve apresentar o problema que a sua aplicação deve resolver. No entanto, não é a hora de comentar sobre a aplicação. 
Descreva também o contexto em que essa aplicação será usada, se houver: empresa, tecnologias, etc. Novamente, descreva apenas o que de fato existir, pois ainda não é a hora de apresentar requisitos detalhados ou projetos.

## 1.2. Objetivos do Trabalho
### Objetivo Geral
Este trabalho tem o objetivo de desenvolver um software para tornar a rotina dos profissionais do setor de mecânica e manutenção automotiva mais prática e eficiente, eliminando a burocracia e o descontrole nos processos de estoque, financeiro e agendamento. Por meio da automatização dessas tarefas, o profissional poderá concentrar-se em prestar um serviço de qualidade, economizando tempo, recursos e energia.
### Objetivos Específicos
- Implementar um sistema de agendamento online que permita ao cliente visualizar a disponibilidade do profissional em tempo real e acompanhar o status de seu atendimento por meio de um painel Kanban.
- Desenvolver um módulo de controle de estoque com rastreio de fornecedores, cotação de preços e verificação de compatibilidade de peças com o veículo em atendimento.
- Disponibilizar um painel gerencial integrado que ofereça à equipe visibilidade centralizada sobre agendamentos, estoque, financeiro e procedimentos em andamento.
- Criar um marketplace que permita ao cliente localizar oficinas credenciadas, consultar a disponibilidade de peças e serviços por localidade e realizar buscas por itens específicos.
- Implementar um sistema de cotação de preços que possibilite a comparação de valores entre fornecedores cadastrados, promovendo transparência e auxiliando o cliente na tomada de decisão.


## 1.3. Justificativa

A implementação de uma plataforma digital que conecte prestadores de serviços automotivos a proprietários de veículos é um ecossistema similar ao modelo marketplace de serviços, justificando-se pela necessidade urgente de mitigar o gap entre a explosão da demanda e a baixa maturidade digital do setor, esta aplicação traz soluções importes e necessárias para o cenário de serviços mecânicos, melhorando a visibilidade e a organização das oficinas, alem de dar um ênfase em empresas de alta qualidade e também da oportunidade para empresas menores de entrar no "cardápio" dos consumidores. Alem disso facilita para os consumidores (Público-alvo primário) a identificação de prestadores mais qualificados e um controle de manutenção no seu veiculo, o que soma na valorização do veiculo, onde veiculos com o gestão da manutenção realizada é bem visado no momento de venda. Esse é o futuro de uma relação de qualidade e transparência entre prestador e consumidor, segue abaixo mais alguns beneficios direcionados.

## 1.3.1. Sob a Ótica do Cliente (Público-alvo primário)
Para o consumidor, a solução ataca as principais "dores" do mercado atual:

* **Confiabilidade e Transparência:** Em um cenário onde manter o veículo é mais econômico do que trocar, o usuário busca segurança. O sistema permite avaliações, histórico de manutenções e comparação de orçamentos.
* **Comodidade:** Assim como no setor de alimentação e transporte, o cliente moderno exige agilidade. O agendamento online elimina a incerteza de filas e a perda de tempo em deslocamentos desnecessários.

## 1.3.2. Sob a Ótica das Oficinas (Público-alvo secundário)
Para o empresário do setor, a tecnologia deixa de ser uma "burocracia" e passa a ser uma ferramenta de sobrevivência e escala:

* **Otimização Operacional:** Com o aumento de 80 para 122 atendimentos mensais (um salto de 52,5%), o controle manual torna-se inviável. O sistema permite o escalonamento inteligente da mão de obra.
* **Previsibilidade Financeira:** A gestão antecipada da demanda permite uma compra de insumos mais estratégica, reduzindo estoques parados e melhorando o fluxo de caixa.
* **Quebra de Barreiras Culturais:** Ao oferecer uma interface intuitiva, a solução remove o receio da modernização, inserindo a oficina de bairro na economia digital sem a necessidade de grandes investimentos em TI própria.

## 1.3.3. Viabilidade de Mercado
O projeto se sustenta na mudança de comportamento do consumidor brasileiro, que já está habituado ao modelo de marketplaces, no nosso caso, sendo um de serviço. Unir a necessidade de manutenção preventiva (decorrente do envelhecimento da frota) com a facilidade tecnológica cria um ambiente propício para a fidelização e para o crescimento sustentável de toda a cadeia automotiva.

## 1.4. Público alvo

O público-alvo desse projeto é composto por dois grupos de usuários, os proprietários de veículos automotores e os prestadores de serviços automotivos, cada qual com suas especificidades.

Público-alvo primário: Consiste em proprietários de veículos automotores, de ambos os gêneros, com idade entre 25 e 60 anos e renda média entre 2 e 10 salários mínimos. Espera-se também que possuam veículos com aproximadamente 3 a 15 anos de fabricação e que realizem manutenção preventiva ou corretiva em oficinas mecânicas independentes, buscando maior praticidade no agendamento dos serviços automotivos.

Público-alvo secundário: Composto por micro e pequenas empresas do setor automotivo, como oficinas mecânicas, centros automotivos, auto elétricas, entre outras. É desejável que sejam estabelecimentos com pelo menos 1 ano de atuação no mercado, que atendam veículos regularmente e necessitam organizar o fluxo de serviços e horários de atendimento, pois fazem isso por meios informais, portanto necessitam de uma solução digital para otimizar a gestão dos atendimentos.

