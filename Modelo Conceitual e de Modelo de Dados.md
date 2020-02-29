#### UNIVERSIDADE FEDERAL DO RIO GRANDE DO NORTE CENTRO DE ENSINO SUPERIOR DO SERIDÓ DEPARTAMENTO DE CIÊNCIAS EXATAS E APLICADAS PROGRAMA DE GRADUAÇÃO EM SISTEMAS DE INFORMAÇÃO

# Modelo Conceitual e de Dados
![trojan](https://user-images.githubusercontent.com/29488124/75595041-a8e70600-5a69-11ea-8285-30abaa72f7f2.png)


# Descrição
### O referido documento representa de maneira abstrata as interações, relacionamentos e atribuições entre os artefatos que compõeem o sistema.

# Histórico de Revisões

| Data | Versão | Descrição | Autor |
| ---- |---- | ---- | ---- |
|29/02/2020| 1.0 | Inicio da documentação | José Erildo |

#Modelo Coneitual

![modelo conceitual](https://i.pinimg.com/564x/c1/af/93/c1af93176c451d06d8157e556a5222bb.jpg)

#Dicionário de Dados

### Tabela 1
| Tabela |	Relacionamento |	Nome do Relacionamento |	Descrição |
|--|--|--|--|
| Usuário|	Aluno | é |	Tabela correspondente aos perfis dos usuários |
|| Administrador|	é   
||	Professor|	é	
|Aluno	|Usuário	|é	|Tabela correspondente a interação com o perfil aluno|
||	Professor|	adiciona/remove|
|Administrador|	Usuário|	é	|Administrador  interage com os perfis usuário e questão|
|| Usuário	| remove	|
|| Questão	| adiciona |
|Professor	|Aluno	|adiciona/remove	|Professor interage com aluno e turma
||	Turma	|cria|	
|Turma	|Professor	|cria	|Tabela de dados da turma
|Questão	|Administrador		|Tabela correspondente aos dados de uma questão

### Tabela 2

| Tabela	| Nome da Coluna | Tipo de Dados	| Comprimento	| Restrições	| Valor Padrão |	Descrição |
|--|--|--|--|--|--|--|
| Usuário |	id	| int	| 4 bytes	| PK, NOT NULL, AUTO_INCREMENT|	N/D	| Nº  identificação do usuário|
||	universidade|	Varchar(100)|	800 bytes	| NOT NULL |	N/D	|Nome da universidade|
||	e-mail	| varchar(50)	| 400 bytes	| NOT NULL |	N/D	| Email do usuário|
||	senha	| int	| 4 bytes	| NOT NULL	| N/D	| Senha do usuário|
||	username | varchar(15) |	120 bytes	| NOT NULL	| N/D	| Login do usuário| 
||	nascimento	| date	| 3 bytes	| NOT NULL	| N/D	| Data de nascimento do usuário
||	sexo	| varchar(9)	| 72 bytes | NOT NULL	| N/D	| Gênero do usuário
||	nome	| Varchar(100) |	800 bytes	| NOT NULL | N/D	| Nome do usuário

### Tabela 3

|Tabela	| Nome da Coluna	| Tipo de Dados	| Comprimento	| Restrições | Valor Padrão	| Descrição|
|--|--|--|--|--|--|--|
|Aluno	|pontuação	|double	|8 bytes	|N/D	|0	|Total de pontos atingidos pelo usuário respondendo questões|

### Tabela 4

|Tabela	| Nome da Coluna	| Tipo de Dados	| Comprimento	| Restrições | Valor Padrão	| Descrição|
|--|--|--|--|--|--|--|
| Professor	| pontuação	| double	| 8 bytes	| N/D	| 0	| Total de pontos atingidos pelo usuário respondendo questões|

### Tabela 5

|Tabela	| Nome da Coluna	| Tipo de Dados	| Comprimento	| Restrições | Valor Padrão	| Descrição|
|--|--|--|--|--|--|--|
| Questão	| id	| int	| 4 bytes	| PK, NOT NULL, AUTO_INCREMENT	| N/D	| Identificador da questão |
|| título	| text	| Sem límíte específico	| NOT NULL	|N/D	|Título da questão
||subtítulo	|text	|Sem límíte específico	| N/D	| N/D	| Subtítulo da questão
||alternativa1	| text	| Sem límíte específico	| NOT NULL	| N/D	|Conteúdo da alternativa 1
||alternativa2	| text	| Sem límíte específico	| NOT NULL	| N/D	|Conteúdo da alternativa 2
||alternativa3	| text	| Sem límíte específico	| NOT NULL	| N/D	|Conteúdo da alternativa 3
||alternativa4	| text	| Sem límíte específico	| NOT NULL	| N/D	|Conteúdo da alternativa 4

### Tabela 6

|Tabela	| Nome da Coluna	| Tipo de Dados	| Comprimento	| Restrições | Valor Padrão	| Descrição|
|--|--|--|--|--|--|--|
| Turma	| id	| int	| 4 bytes	| PK, NOT NULL, AUTO_INCREMENT	| N/D	| Identificador da Turma|
||	quantMembros	|int	| 4 bytes	| NOT NULL	|0	| Quantidade de membros do grupo da turma
