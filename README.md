# Projeto 1A - FirstCRUD

## Sistema de mini-posts

#### Descrição
O projeto consiste em um sistema de posts, em que o usuário pode ver, postar, apagar e editar tarefas.


#### Como usar?
Para começar, você pode rodar o projeto no Eclipse ou acessar pelo URL: http://localhost:8080/Projeto1A/

Se já possuir um cadastro, pode começar entrando diretamente pela página de login. Caso contrário, clique na opção para fazer um cadastro e faça login após essa etapa ser concluída.

A página principal contém a listagem das tarefas criadas. Caso deseje criar uma nova, é só clicar em "Nova Tarefa", no menu. 
Você também pode atualizar ou deletar as tarefas, clicando nos ícones correspondentes (ao lado da lista).

Em meio a tantas tarefas, está perdido para encontrar uma específica? Sem problemas! Você pode procurar pelo nome da tarefa na barra de busca. Caso não se lembre do nome, pode ainda filtrar a lista por categorias. Ou se preferir, pode ordenar a disposição das tarefas por data de entrega ou por ordem afabética!

Quando tiver acabado sua consulta, você pode fazer logout pelo menu.


#### Estrutura
O sistema foi elaborado de acordo com a arquitetura MVC (Model-View-Controller). Dentro do pacote criado, a pasta *Model* contém o DAO (Data Access Object), em que o acesso ao banco de dados é centralizado. A mesma pasta contém os JavaBeans, com os métodos de acesso aos atributos dos objetos (Tarefas e Usuário). Dentro de WEB-INF, a pasta *view* contém os arquivos JSP responsáveis por exibir informações ao usuário. Por fim, na pasta *Controller*, estão os Servlets, cuja função é atuar como um meio de campo entre Model e View.


#### Banco de dados - SQL
Para o projeto, foi criado um database - *projetoum*. Nele, foram criadas duas tabelas: *Tarefas e Usuario*

A tabela Tarefas contém as colunas:
 - id, nome_tarefa, conteudo, data, categoria, nome_usuario
 
A tabela Usuario contém as colunas: 
- id, nome, senha
