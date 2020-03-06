# TROJAN | ENADE SIMULATION
## DOCUMENTO DE VISÃO

![trojan](https://user-images.githubusercontent.com/29488124/75595041-a8e70600-5a69-11ea-8285-30abaa72f7f2.png)

## Histórico de revisões
Data | Versão | Descrição | Autor
--------- | ------ | --------- | ------
28/02/2020   | 1.0 | Documento inicial | José Erildo Medeiros Ramos
28/02/2020   | 1.1 | Documento inicial | Jhonatas I. C. Laurentino
06/03/2020 | 1.2 | Incremento de Requisitos | José Erildo M. Ramos

## Equipe e Definição de Papéis
    
Equipe | Papel | E-mail 
--------- | ------ | ---------
Porfirio Amaro  | Gerente | porfirioamarojr@gmail.com
Jhonatas Laurentino | Analista/Gerente | costajhonatas9@gmail.com
José Erildo | Analista | joseerildo007@gmail.com

### Matriz de Competências

Equipe | Competências
--------- | --------
Porfirio Amaro | HTML,CSS,Javascript, C, UML, Arduino, Scrath;
Jhonatas Laurentino | HTML, CSS, javascript, Bootstrap, Java, C, PHP, Marketing, Gerência de Projetos, entre outras habilidades...
José Erildo | HTML, CSS, Javascript, C, Arduino;

## Descrição do Projeto
O  sistema Trojan tem como propósito incentivar alunos a testarem seus conhecimentos tecnológicos e matemáticos sobre a prova do ENADE, de forma a prepará-los para o exame, agregando influência e especialização pela área. O sistema é composto por questões relacionadas à àrea de Tecnologia da Informação e contará com mecanismos de pontos para classificar jogadores em escala pessoal e ranking geral, instigando-os a melhorar cada vez mais.

## Requisitos Funcionais
------------------------------------------------------------------
Correspondente à usuários:
        
        RF01 - CRUD perfis usuário (professor, aluno e administrador)
    
    RF02 - Ver histórico de questões - Deve conter o nome da questão, data e hora da tentativa;

------------------------------------------------------------------
Correspondente à administradorRF03 - CRUD questão
    
--------------------------------------------------------------------
Correspondente ao perfil professor
    RF04 - Crud Turma
    RF05 - Crud Aluno
    RF06 - Selecionar questões para a turma
   
------------------------------------------------------------------
Correspondente às questões:
    RF07 - CRUD questão
    RF08 - 2 Sessões de questões divididas entre: selecionar categoria e nivel da questão;
    RF09 - A sessão anterior correspondente a nivelamente deve conter uma opção de níveis aleatórios;
    RF10 - O professor e aluno podem selecionar a resposta
    RF11 - O professor e aluno detêm X tempo para completar a questão
    
------------------------------------------------------------------
Correspondente às estatísticas:
    RF12 - Ver ranking geral
    RF13 - Ver ranking por categoria
    RF14 - Progresso de questões referentes a cada categoria - Ex de progresso:  45 de 115;
    RF15 - Progresso de questões referentes a todas as questões
    RF16 - Estatística de resoluções do usuário dos úçtimos 6 meses
    RF17 - Estatística de resoluções do usuário de 1 ano atrás
    RF18 - Gráfico pizza referente às questões respondidas de cada categoria
    RF19 - Ver outros jogadores
    RF20 - Mostrar questões resolvidas    
    RF21 - Top 20 maiores pontuações 
    RF22 - Sessão de Ajuda
    RF23 - Sessão de Contato
    
--------------------------------------------------------------------
Correspondente a outras sessões
    RF24 - Sessão de perguntas frequentes
    RF25 - Sessão sobre o site
    RF26 - Sessão desafio
    
--------------------------------------------------------------------
Correspondente a sessão desafio
    RF27 - Uma sessão destinada a questões lançadas em períodos específicos. Tais perguntas são elaboradas por professores de X área e somente o administrador tem permissão para publicá-las.
    RF28 - A(s) questão(ões)devem conter um período global para ser respondida
    

## Requisitos não-Funcionais

    RNF01 - Servidor web
    RNF02 - facilidade de acesso
    RNF03 - Ambiente atrativo
    RNF04 - Utilizar de uma base de dados para armazenar informações dos jogadores 
    RNF05 - Confiabilidade quanto às informações dos usuários
    RNF06 - Facilidade de Uso

## Perfis dos Usuários
**Jogador:** aquele que participa do quiz e interage com outros jogadores;

**Professor:** criar um grupo de turma e inserir alunos, criando rankings, fazendo atividades e interagindo com eles.

**Administrador:** cadastrar questões, gerar enquetes globais e publicar notícias;


## Riscos

Preencher na tabela os riscos identificados para o início do projeto. Essa tabela deve ser atualizada ao final de cada iteração na reunião de acompanhamento.
- Não entrar o sistema no prazo
- Expor os dados do usuário
- O sistema não ser funcional
- O sistema não atingir os requisitos estabelecidos
- Não agradar o cliente


Data | Risco | Prioridade | Responsável | Status | Providência/Solução
--------- | ------ |  -------- | --------- |  --------- | ------
28/02/2020 | Não entregar o sistema no prazo | Alta | Todos |Vigente | Manter-se fiel aos prazos do cronograma.
28/02/2020 | Expor os dados do usuário | Alta | Desenvolvedor | Vigente | Fazer verificações de segurança quanto ao acesso de terceiros ao banco de dados
28/02/2020 |Erros de funcionalidade no sistema | Alta | Desenvolvedor | Vigente | Aplicar vários testes em todo o site
28/02/2020 | Não atingir os requisitos estabelecidos | Alta | Desenvolvedor e Analista | Vigente | Verificar se todos os requisitos estão contidos na aplicação
28/02/20 | Não agradar o cliente | Alta | Todos | Vigente |  Manter contato e sempre notificar e receber feedbacks



[link drive](https://docs.google.com/document/d/1LRq87qfWPJkKeYejZEAmTLUfaU4A5eqDhHBc5BNnLJE/edit#heading=h.xsipevjb5rla) | 
[link github](https://github.com/AmaroJunior98/trojan.git) 
