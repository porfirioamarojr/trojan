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
