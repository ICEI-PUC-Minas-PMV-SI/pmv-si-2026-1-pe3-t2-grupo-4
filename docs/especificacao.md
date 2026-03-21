# 3. DOCUMENTO DE ESPECIFICAÇÃO DE REQUISITOS DE SOFTWARE

## 3.1 Objetivos deste documento
O objetivo deste documento é especificar as necessidades de prestadores de serviços automotivos e seus clientes que deverão ser atendidas pelo sistema proposto, denominado AgendaCar.

## 3.2 Escopo do produto

### 3.2.1 Nome do produto e seus componentes principais
O produto será denominado AgendaCar. O sistema consiste em uma plataforma digital cujo objetivo é facilitar a conexão entre clientes e prestadores de serviços automotivos, permitindo a busca por serviços, a visualização de prestadores disponíveis e o agendamento de atendimentos de forma online. O sistema possibilitará o cadastro e gerenciamento de usuários e prestadores de serviços, o controle de disponibilidade de horários, a realização de agendamentos e a avaliação de serviços prestados.

### 3.2.2 Missão do produto
Otimizar a organização dos atendimentos de prestadores de serviços automotivos e melhorar a experiência dos clientes por meio de um sistema que facilite a busca e o agendamento de serviços.

### 3.2.3 Limites do produto
O AgendaCar não irá abranger funcionalidades relacionadas ao controle de estoque e de gestão financeira dos prestadores de serviços, como controle de receitas, despesas ou emissão de relatórios financeiros. O foco do sistema será a realização de agendamentos de serviços e a intermediação entre clientes e prestadores.

### 3.2.4 Benefícios do produto

| # | Benefício | Valor para o Cliente |
|--------------------|------------------------------------|----------------------------------------|
|1	| Praticidade na busca por serviços automotivos |	Essencial |
|2	| Facilidade no gerenciamento de agendamentos	| Essencial | 
|3 | Acesso a informações detalhadas sobre prestadores e serviços | Essencial | 
|4 | Facilidade na contratação de serviços | Essencial | 
|5	| Organização dos agendamentos realizados	| Essencial | 
|6	| Maior transparência por meio de avaliações de usuários	| Desejável |
|7	| Melhoria na comunicação com os clientes	| Desejável | 



## 3.3 Descrição geral do produto

### 3.3.1 Requisitos Funcionais

| Código | Requisito Funcional (Funcionalidade) | Descrição | Prioridade |
|--------------------|------------------------------------|----------------------------------------|------------|
| RF1 | Acessos ao sistema |	O usuário deve realizar login utilizando e-mail e senha. | Essencial |
| RF2 |	Gerenciamento de usuários	| O usuário deve manutenir seus dados cadastrais no sistema. | Essencial |
| RF3	| Filtro de prestadores |	O cliente pode filtrar prestadores por categoria, localização e avaliação. | Essencial |
| RF4	| Agendamento de serviços |	O cliente deve agendar a prestação de serviços no sistema. | Essencial |
| RF5	| Gerenciamento da agenda |	O prestador deve gerenciar sua disponibilidade e quantidade de vagas na agenda. | Essencial |
| RF6	| Gerenciamento de serviços e produtos |	O prestador deve catalogar no sistema seus serviços e produtos oferecidos. | Essencial |
| RF7	| Alteração e cancelamento de agendamentos |	O usuário pode alterar/cancelar os agendamentos. | Essencial |
| RF8	| Avaliação dos prestadores |	O cliente pode avaliar os prestadores de serviços. | Desejável |
| RF9	| Emissão de relatórios |	O prestador pode emitir relatórios de agendamentos. | Desejável |
| RF10	| Solicitação de pré-diagnóstico |	O cliente pode solicitar um pré-diagnóstico ao prestador antes do agendamento. | Desejável |
| RF11	| Bloqueio de agendamentos |	O sistema deve bloquear conflitos de agendamentos. | Desejável |
| RF12	| Tempo limite para cancelamento |	O usuário não pode alterar/cancelar um agendamento com menos de 24 horas de antecedência. | Desejável |
| RF13	| Aprovação de orçamentos |	O prestador de serviços pode enviar orçamentos e solicitar a aprovação do cliente. | Opcional |

### 3.3.2 Requisitos Não Funcionais

| Código | Requisito Não Funcional (Restrição) |
|--------------------|------------------------------------|
| RNF1 | A aplicação deve ser responsiva em diferentes dispositivos (computadores, tablets, smartphones). |
| RNF2 | A aplicação deve apresentar interface simples e intuitiva. |
| RNF3 |	A aplicação deve suportar aumentos no volume de requisições. |
| RNF4 |	O sistema deve estar disponível 24/7. |
| RNF5 |	Os carregamentos entre páginas e módulos devem ter apenas 3seg de carregamento. |
| RNF6 |	O sistema poderá apresentar tema escuro e claro. |
| RNF7 |	O sistema deve respeitar as leis locais (LGPD). |

### 3.3.3 Usuários 

| Ator | Descrição |
|-----------------|---------------------------------------|
| Prestador de serviços |	O prestador de serviços será o usuário responsável por gerenciar as solicitações de agendamentos dos clientes, podendo aceitar ou recusar de acordo com seu interesse. Também será responsável por catalogar no sistema os produtos e serviços oferecidos em seu estabelecimento. |
| Cliente |	Caberá ao usuário cliente selecionar no sistema o prestador de seu interesse e solicitar o agendamento dos serviços. Além disso, será de sua responsabilidade avaliar os prestadores após a realização do atendimento. |

## 3.4 Modelagem do Sistema

### 3.4.1 Diagrama de Casos de Uso
Como observado no diagrama de casos de uso da Figura 1, a secretária poderá gerenciar as matrículas e professores no sistema, enquanto o coordenador, além dessas funções, poderá gerenciar os cursos de aperfeiçoamento.

#### Figura 1: Diagrama de Casos de Uso do Sistema.

![dcu](https://github.com/user-attachments/assets/41f6b731-b44e-43aa-911f-423ad6198f47)
 
### 3.4.2 Descrições de Casos de Uso

#### Solicitar Agendamento (CSU-01)

Sumário: O cliente escolhe um prestador no sistema e solicita o agendamento na data e horário de seu interesse, podendo descrever brevemente sua necessidade.

Ator Primário: Cliente

Ator Secundário: Prestador

Pré-condições: O cliente deve estar logado no sistema.

Fluxo Principal:

1) 	O cliente escolhe um prestador no sistema.
2) 	O sistema apresenta o catálogo de produtos e serviços do prestador escolhido, juntamente com as opções ‘escolher outro prestador’ e ‘solicitar agendamento’.
3) 	Caso o cliente selecione a opção ‘escolher outro prestador’, o caso de uso retorna à etapa 1; caso contrário, o caso de uso segue o fluxo.
4) 	Após a escolha da opção ‘solicitar agendamento’, o sistema apresenta um calendário com datas/horários disponibilizados pelo prestador.
5) 	O cliente seleciona a data/horário de seu interesse e o sistema apresenta as opções ‘confirmar solicitação’ e ‘escolher outra data/horário’.
6) 	Caso o cliente selecione a opção ‘escolher outra data/horário’, o caso de uso retorna à etapa 4; caso contrário, a solicitação é confirmada e o caso de uso é concluído. <br>

Pós-condições: O prestador recebe a solicitação do cliente e escolhe aceitar ou recusar, gerenciando dessa forma seus agendamentos.

#### Gerenciar agendamentos (CSU-02)

Sumário: O prestador recebe as solicitações dos clientes com informações de data/horário e uma breve descrição da demanda, podendo aceitar, recusar ou propor uma nova data/horário para realizar o atendimento.

Ator Primário: Prestador

Ator Secundário: Cliente

Pré-condições: O prestador deve estar logado no sistema.

Fluxo Principal:

1) 	O prestador recebe uma solicitação de agendamento no sistema.
2) 	O sistema apresenta as opções ‘aceitar’, ‘recusar’ e ‘propor uma nova data/horário’.
3) 	Se o prestador escolher a opção ‘aceitar’, o agendamento é confirmado e o caso de uso é concluído.
4) 	Se o prestador escolher a opção ‘recusar’, o agendamento é cancelado, o cliente é informado sobre a recusa e o caso de uso é concluído.
5) 	Se o prestador escolher a opção ‘propor uma nova data/horário’, o sistema apresenta um calendário com datas/horários.
6) 	O prestador informa a data/horário de sua disponibilidade, o sistema envia a proposta ao cliente e o caso de uso é concluído. <br>

Fluxo Alternativo (etapa 2):

1) 	O prestador não responde à solicitação do cliente e não sugere uma nova data/horário.
2) 	Após 24h da abertura da solicitação, o sistema recusa automaticamente e informa ao cliente que o prestador não respondeu.
3) 	O sistema apresenta ao cliente as opções ‘solicitar novamente ao mesmo prestador’ e ‘solicitar a outro prestador’.
4) 	Caso o cliente selecione ‘solicitar novamente ao mesmo prestador’, o caso de uso retorna à etapa 4 do CSU-01 (Solicitar agendamento).
5) 	Caso o cliente selecione ‘solicitar a outro prestador’, o caso de uso retorna ao início do CSU-01 (Solicitar agendamento). <br>

Pós-condições: O sistema informa ao prestador que ter um percentual de recusas elevado influencia na sua avaliação.


### 3.4.3 Diagrama de Classes 

A Figura 2 mostra o diagrama de classes do sistema. A Matrícula deve conter a identificação do funcionário responsável pelo registro, bem com os dados do aluno e turmas. Para uma disciplina podemos ter diversas turmas, mas apenas um professor responsável por ela.

#### Figura 2: Diagrama de Classes do Sistema.
 
![image](https://github.com/user-attachments/assets/abc7591a-b46f-4ea2-b8f0-c116b60eb24e)


### 3.4.4 Descrições das Classes 

| # | Nome | Descrição |
|--------------------|------------------------------------|----------------------------------------|
| 1	|	Aluno |	Cadastro de informações relativas aos alunos. |
| 2	| Curso |	Cadastro geral de cursos de aperfeiçoamento. |
| 3 |	Matrícula |	Cadastro de Matrículas de alunos nos cursos. |
| 4 |	Turma |	Cadastro de turmas.
| 5	|	Professor |	Cadastro geral de professores que ministram as disciplinas. |
| ... |	... |	... |
