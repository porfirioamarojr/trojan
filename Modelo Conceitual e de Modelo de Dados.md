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
