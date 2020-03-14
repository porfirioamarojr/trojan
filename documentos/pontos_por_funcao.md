Análise de Pontos de Função para o Sistema APF

Análise de Pontos de Função para o Sistema APF    1
Descrição do Projeto    1
Siglas    1
Lista de User Stories - US    1
US01 - Cadastro de Projetos    1
US02 - Cadastro de Usuários    2
US03 - Cadastro de Membros/Equipe    2
US04 - Cadastro de User Stories    2
US05 - Cadastro de Funções do Tipo Dado    2
US06 - Cadastro de Funções do Tipo Transação    2
Tipos de Contagem    2
Contagem Indicativa (Ci)    2
Contagem Estimativa (Ce)    3
Contagem Detalhada (Cd)    3


Descrição do Projeto
    O projeto consiste de um sistema para auxiliar o analista de sistemas ou engenheiro de software à realizar uma contagem por ponto de função. O sistema permitirá o cadastro de informações da base de dados e das telas das funcionalidade para gerar informações para os conceitos da análise de ponto de função. Os conceitos relacionados com dados são os Arquivos de Lógica Interna (ALI) e os Arquivos de Interface Externa (AIE), e os conceitos relacionados com operações externas a fronteira do sistema são: Entrada Externa (EE), Consulta Externa (CE) e Saída Externa (SE).
Siglas
    PF - Pontos de Função
    APF - Análise de Pontos de Função
    ALI - Arquivos Lógicos Internos
Lista de User Stories - US
    Lista de User Stories e os requisitos que estão associados.
US01 - Cadastro de Projetos

    RF01 - Cadastro de Projetos;
US02 - Cadastro de Usuários

    RF13 - Cadastro e Gerenciamento de Usuários;
US03 - Cadastro de Membros/Equipe

    RF03 - Incluir membros da equipe do projeto;
    RF04 - Alterar membro da equipe do projeto;
US04 - Cadastro de User Stories

    RF05 - Cadastro de User Stories;
US05 - Cadastro de Funções do Tipo Dado

    RF06 - Cadastro de Funções do Tipo Dado;
        RF06.1 - Cadastro de ALI (ILFs);
        RF06.2 - Cadastro de AIE (EIFs);

US06 - Cadastro de Funções do Tipo Transação

    RF07 - Cadastro de Funções do Tipo Dados;
        RF07.1 - Cadastro de Entrada Externa - EE (EI - External Inputs);
        RF07.2 - Cadastro de Consulta Externa - CE (EQ - External Inquiry);
        RF07.3 - Cadastro de Saída Externa - SE (EO - External Outputs);
                Às saídas externas devem gerar dados derivados.

Tipos de Contagem
Contagem Indicativa (Ci)

    Na contagem indicativa só é necessário analisar os ALIs (Arquivos Lógicos Internos) com o valor de 35 PF cada e os AIE (Arquivos de Interface Externa) com o valor de 15 PF cada.
