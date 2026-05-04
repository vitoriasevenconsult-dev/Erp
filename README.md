# Erp
Documentação Grupo 2
FLOWDOC
Gestão de Equipes
1
São Paulo
2026
UNIVERSIDADE CIDADE DE SÃO PAULO
SUMÁRIO
1. INTRODUÇÃO ...............................................................................................3
1.1 FUNCIONALIDADES....................................................................3 – 4
1.2 REGRAS DE NEGÓCIO ...............................................................4 - 5
2. METODOLOGIA DE DESENVOLVIMENTO .............................................5 - 6
3. PÚBLICO- ALVO..............................................................................................6
4. FERRAMENTAS E METODOLOGIAS UTILIZADAS ......................................7
5. ESPECTRO DE ATUAÇÃO.............................................................................7
6. RESULTADOS ESPERADOS..........................................................................8
7. RESULTADO DISC EQUIPE....................................................................9 - 10
8. MODELAGEM DO APLICATIVO ..................................................................10
8.1 ABAS E TABELAS .......................................................................10 - 11
8.2 TIPAGEM DE ATRIBUTOS.................................................................12
9. APRESENTAÇÃO..................................................................................13 – 15
2
São Paulo
2026
UNIVERSIDADE CIDADE DE SÃO PAULO
INTRODUÇÃO
Atualmente, a gestão eficiente de demandas internas tornou-se um fator
fundamental para garantir produtividade, organização e qualidade na execução
de tarefas.
Diante desse cenário, o FLOWDOC é um sistema inteligente produzido com o
objetivo de otimizar o gerenciamento de demandas organizacionais,
aumentando controle de prazos, produtividade, evitar perda de informações
devido à falta de documentações e facilitar a comunicação entre equipe.
O FLOWDOC foi produzido para atender às necessidades de equipes que
buscam organização, eficiência e otimização de tempo em suas atividades,
oferecendo funcionalidades como cadastro e autenticação de usuários, criação
e gerenciamento de demandas, definição de prioridades por meio de
indicadores visuais, atribuição de responsáveis e acompanhamento dos status
das tarefas.
Além disso, o sistema incorpora um mecanismo de documentação obrigatória
das demandas, no qual o usuário só poderá realizar alterações em uma
atividade mediante o registro de informações descritivas sobre a ação
executada. Caso essa documentação não seja realizada, o usuário permanece
com permissões restritas, atuando apenas como leitor. Essa funcionalidade foi
criada como o intuito de garantir rastreabilidade e controle de atividades,
incentivando boas práticas de registro. Dessa forma, o sistema não apenas
gerencia tarefas, mas também assegura formalização das ações realizadas,
contribuindo para melhoria contínua dos processos.
Este trabalho temo como objetivo apresentar o desenvolvimento do sistema
FLOWDOC, abordando os conceitos, funcionalidades e metodologias aplicadas
a sua relevância no contexto das necessidades em um ambiente corporativo.
FUNCIONALIDADES
Autenticação de usuários
O FLOWDOC permite o cadastro e autenticação de usuários por meio de login
e senha, garantindo que apenas pessoas autorizadas tenham acesso às
informações e funcionalidades.
Gerenciamento de demandas
O usuário pode criar, editar e visualizar demandas, permitindo o controle
completo de atividades. As demandas devem obter informações detalhadas,
como responsável, prazo, descrição, e data das últimas atualizações.
3
São Paulo
2026
UNIVERSIDADE CIDADE DE SÃO PAULO
Definição de prioridades
As demandas podem ser classificadas por níveis de prioridade (baixa, média e
alta), utilizando cores como indicadores visuais para facilitar a identificação de
tarefas mais urgentes, ajudando na tomada de decisões.
Controle de prazos
O sistema permite a definição de prazos para cada demanda, permitindo o
acompanhamento de tempo de execução e contribuindo para o cumprimento
de metas e entregas antes do vencimento.
Atribuição de responsáveis
É possível denominar pessoas responsáveis para cada demanda, promovendo
organização e clareza na distribuição das atividades entre as pessoas.
Acompanhamento de status
Além dos indicadores visuais, as demandas podem ser organizadas por status,
como “pendente”, “em andamento”, e “concluído”.
Documentação obrigatória das demandas
O sistema exige documentação para realização de alterações nas demandas.
Para que o usuário possa editar uma tarefa, é preciso registrar informações
descritivas sobre a ação executada, fornecendo evidências com anexos,
descrição da ação, horário e nome do usuário que realizou a edição.
Histórico de alterações
O sistema mantém um registro de alterações realizadas nas demandas,
permitindo o acompanhamento o histórico de modificações.
Comunicação entre equipe
Os usuários poderão entrar em contato uns com os outros através da aba
“mensagens”, podendo referir-se a uma demanda específica na mensagem
enviada.
Agenda
reuniões.
O usuário pode registrar todos os seus prazos de entregas, lembretes e
Reunião
O usuário pode registrar os horários, participantes e links de reuniões.
REGRAS DE NEGÓCIO
RN01: O acesso ao sistema só será permitido mediante login e senha válidos.
4
São Paulo
2026
UNIVERSIDADE CIDADE DE SÃO PAULO
RN02: Toda demanda deve ter título, descrição, data e prazo no momento de
criação.
RN03: Cada demanda deve possuir um identificador único no sistema (#).
RN04: A edição de uma demanda só pode ser realizada com o registro de uma
documentação descritiva da alteração.
RN05: Se o usuário não registrar a documentação exigida, ele terá acesso
apenas de visualização.
RN06: Toda documentação inserida deve ser armazenada e vinculada á
respectiva demanda, compondo o histórico de alterações.
RN07: Toda demanda deve possuir um nível de prioridade definido.
RN08: As demandas devem obter um status que represente seu andamento.
RN09: Toda demanda deve possuir uma data limite para conclusão.
RN10: Cada demanda deve obter ao menos um usuário responsável.

RN11: A exclusão de demandas poderá ser restrita a usuários com permissão
administrativa.

METODOLOGIA DE DESENVOLVIMENTO
Esse projeto foi desenvolvido baseado na metologia ágil SCRUM, com
organização das atividades em sprints (divisão do projeto). As principais
funcionalidades (demanda, documentação e trabalho em equipe) foram
definidas no início do projeto, e as demais funcionalidades foram
implementadas de forma incremental, permitindo um planejamento flexível.
Sprint 1: Planejamento geral.
Sprint 2: Listar funcionalidades e regras de negócio.
Sprint 3: Início da realização do protótipo.
Sprint 4: Teste.
Sprint 5: Organização de ideias para apresentações.
Sprint 6: Início da realização do projeto final.
A metodologia Scrum foi escolhida por permitir flexibilidade no
desenvolvimento, possibilitando a construção incremental do sistema e
facilitando a adaptação a mudanças durante o projeto.
5
São Paulo
2026
UNIVERSIDADE CIDADE DE SÃO PAULO
SPRINT PERÍODO ATIVIDADES ENTREGA
1 Primeira semana 2 Segunda semana 3 Terceira á quarta
semana
Organização da equipe,
definição do escopo,
planejamento do sistema.
Listar funcionalidades de
cada aba específica,
regras de negócio,
restrições do sistema,
detalhamento de
descrição das abas do
sistema, definição do
logo, cores e fontes.
Iniciação do protótipo
pela ferramenta FIGMA,
utilizando a
documentação inicial do
projeto.
Definição da
estrutura inicial
do projeto.
Estrutura
aprofundada que
seja
minimamente
funcional
Protótipo
visualmente
claro, funcional e
ideal para
realização de
testes.
4 Quarta semana Realização de testes das
abas, logins, segurança
dos dados.
5 Quinta a sexta
semana
Definição de modelo,
dinâmica, materiais e
responsabilidades para
apresentação.
Testes claros
para alterações
no projeto final.
Definição da
apresentação
final.
6 Sexta semana Início do
desenvolvimento do
projeto final, 100%
funcional
Entrega do
produto.
PÚBLICO- ALVO
O sistema é especialmente indicado para ambientes que exigem controle
rigoroso das atividades e registro formal das alterações realizadas.
Entre os principais usuários do sistema, destacam-se:
• Equipes administrativas, que necessitam organizar demandas operacionais
e acompanhar prazos;
• Setores de Tecnologia da Informação (TI), responsáveis pelo gerenciamento
de chamados, tarefas técnicas e suporte interno;
• Pequenas e médias empresas, que buscam uma solução prática para
organizar seus processos internos;
6
São Paulo
2026
UNIVERSIDADE CIDADE DE SÃO PAULO
• Equipes de projetos, que necessitam de controle sobre atividades, status e
progresso das entregas.
FERRAMENTAS E METODOLOGIAS
UTILIZADAS
O desenvolvimento do FLOWDOC foi baseado em uma abordagem ágil,
utilizando princípios do Scrum. As atividades foram organizadas em etapas
incrementais, permitindo a construção gradual das funcionalidades, como
controle de demandas, autenticação de usuários e organização por prioridades.
As tarefas foram divididas em pequenas entregas semanais, priorizadas
conforme a necessidade do sistema. Foram realizados testes contínuos
durante o desenvolvimento, garantindo a validação das funcionalidades
implementadas.
As ferramentas utilizadas foram:
• Google docs: Documentação geral do projeto;
• Word: Formatação de documentos para entrega;
• Figma: Desenvolvimento do protótipo e projeto final;
• Miro: Diagramação visual e planejamento.
ESPECTRO DE ATUAÇÃO
Seu uso é voltado para equipes corporativas que necessitam organizar
atividades internas de forma eficiente. O sistema contempla funcionalidades
como criação de demandas, categorização por prioridade, controle de usuários
e acompanhamento do fluxo de execução.
Não fazem parte do escopo do sistema funcionalidades como integração com
sistemas externos, automação avançada de processos, análise preditiva de
dados, não utiliza inteligência artificial e não substitui sistemas ERP.
7
São Paulo
2026
UNIVERSIDADE CIDADE DE SÃO PAULO
RESULTADOS ESPERADOS
Com a implementação do sistema FLOWDOC, espera-se promover melhorias
significativas na gestão de demandas organizacionais, proporcionando maior
controle, organização e eficiência na execução das atividades.
Entre os principais resultados esperados, destacam-se:
• Melhoria na organização das demandas: O sistema permitirá a
centralização das tarefas em um único ambiente, facilitando o acesso às
informações e reduzindo a desorganização causada por controles manuais
ou descentralizados.
• Aumento da produtividade: Com a definição clara de prazos, prioridades e
responsáveis, espera-se uma execução mais eficiente das atividades,
reduzindo atrasos.
• Melhor distribuição de responsabilidades: A atribuição de responsáveis por
demanda proporcionará maior clareza na divisão das tarefas, evitando
falhas de comunicação.
• Maior controle e rastreabilidade: Espera-se garantir um histórico detalhado
de todas as alterações realizadas em um projeto, promovendo,
responsabilidade e controle das ações.
• Fortalecimento da governança e auditoria: O registro das atividades
permitirá auditorias mais eficazes, contribuindo para a padronização dos
processos e melhoria contínua das operações.
• Redução de erros e retrabalho: A padronização do fluxo de trabalho e o
controle das alterações tendem a diminuir inconsistências e falhas na
execução das tarefas.
DISC DA EQUIPE
Emilly Carvalho de Oliveira
Resultado: D – Dominante
Gustavo Fernandes de Oliveira
Resultado: S – Estabilidade
Heberty Alexandre Da Silva
Resultado: C - Conformidade
Izadora Lima Santos
8
São Paulo
2026
UNIVERSIDADE CIDADE DE SÃO PAULO
Resultado: D – Dominante
Marcela Monteiro Ferreira
Resultado: C - Conformidade
Michael Moisés Alves de Moura
Resultado: C – Conformidade
Pedro Henrique Marcandelle
Resultado: S – Estabilidade
Rafael Marconi Navas Titonele
Resultado: C - Conformidade
Rafael Romanato Cordeiro
Resultado: C - Conformidade
Raíssa Buytar
Resultado: C - Conformidade
Victor Manoel Pereira dos Reis
Resultado: C - Conformidade
Vitória Alves da Silva
Resultado: C - Conformidade
Willian Biapino Souza Rodrigues
Resultado: I – Influência
Dominância: Assertivos, competitivos e orientados a resultados. Gostam de
desafios e tomam decisões rápidas.
Influência: Sociáveis, otimistas e persuasivos. Comunicáveis colaborativos.
Estabilidade: Calmos, pacientes e consistentes. Valorizam a harmonia e o
ambiente acolhedor.
Conformidade: Detalhistas, técnicos, precisos. Valorizam regras, qualidade e
análise detalhada.
9
São Paulo
2026
UNIVERSIDADE CIDADE DE SÃO PAULO
DISC
Conformidade Dominancia Estabilidade Influência
MODELAGEM DO APLICATIVO
ABAS E TABELAS
Demandas
• Criar, editar e acompanhar demandas
• Definir prioridade, prazo e status
Dados necessários:
• Cliente
• Tipo da demanda
• Descrição
• Status (pendente, em andamento, concluído)
• Data de criação e prazo
• Responsável (Admin)
Tabela: Request
Aba: Clientes (Customer)
• Cadastro de clientes
• Consulta de demandas por cliente
Dados necessários:
• Nome
10
São Paulo
2026
UNIVERSIDADE CIDADE DE SÃO PAULO
• Contato
• E-mail
Tabela: Admin
Aba: Administração (Admin)
• Login no sistema
• Controle de usuários
• Responsáveis pelas demandas
Dados necessários:
• Nome
• Senha
Tabela: Admin
Aba: Administração (Admin)
• Login no sistema
• Controle de usuários
• Responsáveis pelas demandas
Dados necessários:
• Nome
• Senha
Aba: Documentação
• Registrar tudo que foi feito
• Guardar conhecimento da equipe
• Evitar perda de informação
Funcionalidades:
• Anexar descrição detalhada
• Histórico de alterações
• Relacionar com demandas
11
São Paulo
2026
UNIVERSIDADE CIDADE DE SÃO PAULO
TIPAGEM DE ATRIBUTOS
Usuário
CAMPO TIPO
Usuário (PK) Nome INT
VARCHAR
Email VARCHAR
Senha VARCHAR
Perfil
Campo Tipo
Perfil (PK) Nome INT
VARCHAR
Descrição TEXT
Equipe
Campo Tipo
Equipe (PK) Nome INT
VARCHAR
Usuário Equipe
Campo Tipo
ID (PK) Usuário (FK) EquipeID (FK) INT
INT
INT
Demanda
Campo Tipo
DemandaID (PK) Titulo INT
VARCHAR
Descrição TEXT
Comentário Demanda
Campo Tipo
ComentarioID (PK) DemandaID (FK) UsuarioID (FK) Conteudo INT
INT
INT
Text
Data DATETIME
12
São Paulo
2026
UNIVERSIDADE CIDADE DE SÃO PAULO
Anexo
Campo Tipo
Anexo (PK) DemandaID (FK) Arquivo INT
INT
VARCHAR
Notificação
Campo Tipo
NotificaçãoID (PK) DocumentoID (FK) Mensagem INT
INT
TEXT
Data DATETIME

APRESENTAÇÃO
A apresentação será realizada em formato de gincana temática, com o objetivo de
tornar o conteúdo mais dinâmico, interativo e envolvente para os participantes.

A gincana será composta por 6 rodadas de perguntas, organizadas por nível de
dificuldade, conforme descrito abaixo:
• 3 rodadas de perguntas fáceis, totalizando 15 perguntas
• 2 rodadas de perguntas médias, totalizando 10 perguntas
• 1 rodada de pergunta difícil, contendo 8 perguntas

Em cada rodada, cada participante responderá uma pergunta, garantindo
participação equilibrada entre todos.
Com base na quantidade total de perguntas disponíveis por rodada, foi definido
que poderão participar até 5 pessoas, permitindo que todas as rodadas sejam
realizadas sem repetição de perguntas.
Regras

• Cada participante terá 10 segundos para responder cada pergunta, caso
passe do tempo, será desclassificado.

• O vencedor receberá 1 caixa de bombom, uma agenda e uma caneta.

• Os participantes que ocuparam o 2º e 3º lugar receberão uma agenda, uma
caneta e um bombom.
____
