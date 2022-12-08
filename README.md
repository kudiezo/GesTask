# GesTask
 Trabalho dado pelo professor (Engenharia de Software)

[ENUNCIADO]

Engenharia de Software I 
João da Costa  
joao.costa@isptec.co.ao 
ISPTEC / DET / EINF, 2022-23 
Exercícios de Engenharia de Software I 
 
Tema II: Modelação de Sistema de Software. 
 
# Objectivo 
Analisar o problema proposto seguindo o paradigma orientado a objecto com recurso a 
linguagem UML. 
# Introdução 
Pretendemos desenvolver uma aplicação móvel multiplataforma para gestão de tarefas 
(GesTasks). Deve haver um servidor de aplicação para dar suporte a mobilidade e deve 
funcionar como mediador dos principais serviços do GesTasks. 

# LISTA DE EVENTOS 
#  Descrição  Tipo  Classificação
1  Registar utilizador  E  C 
2  Criar lista  E  D 
3  Adicionar tarefa  E  D 
4  Marcar tarefa como concluída   E  D 
 
# DETALHES DOS EVENTOS 
O registo de um utilizador requer que o mesmo tenha uma conta GMail. O utilizar ao solicitar o seu registo é reencaminhado para interface de autenticação sob domínio da empresa Google, onde lhe é solicitado a sua conta de email e a palavra-passe. Se autenticado com sucesso o 
GesTask recebe um conjunto de dados autorizados (fotografia, nome e conta de email) dos serviços Google. Estes dados são armazenados na base de dados local do cliente GesTask e na sua base de dados na nuvem gerida pelo servidor de aplicação. Se o servidor estiver indisponível, então o cliente localmente agenda o registo para, assim que tiver conectividade, 
concluir a operação (define um serviço que monitorar as comunicações, via WiFi e/ou redes móveis – LTE/3G/2G, para implementar o comportamento em background). 
Para criar uma lista, o utilizador deve estar registado no GesTask e ser apresentado as listas predefinidas ou as previamente criadas pelo próprio utilizador, seleciona a opção e, a seguir, fornece o nome da lista e um marcador (cor ou fotografia). A lista é mantida tanto no cliente móvel GesTask como no servidor GesTask. Há listas geradas automaticamente pelo sistema (O 
meu dia, Importante, Planeada e Tarefas) no momento de instalação do GesTask. Embora o utilizador tem a visão de quatro listas, em termo prático apenas existe uma lista (a lista Tarefas), as outras listas são na verdade a lista Tarefas apresentada com um determinado filtro. A lista “O meu dia” é composta pelas tarefas que têm o campo “hoje” definido com true. 
A lista “Importante” é composta pelas tarefas que têm o campo “importante” definido com true. A lista “Planeada” é composta pelas tarefas que têm o campo “prazo” definido com uma determinada data.
Uma lista é composta nenhuma ou várias tarefas. Uma tarefa é composta por um 
identificador, uma descrição, um atributo para indicar que a tarefa deve ser feita hoje ou não, pode ter um prazo, uma data de criação e tem um estado (concluída ou não concluída). 
Para adicionar uma tarefa, deve antes selecionar a lista que pretende utilizar. Ao selecionar a lista, lhe é listada todas as tarefas que pertencem a lista e o recurso para adicionar a tarefa. Ao adicionar a tarefa deve ser apresentada nas listas predefinidas. As tarefas listas na lista, podem ser marcadas como importante, concluída e/ou do dia (hoje). A tarefa pode, também, alterar/adicionar lembrete periódico ou não (em termo de data e hora), prazo, descrição e ficheiro. 
 
# EXERCÍCIOS 
 
1.  Elaborar o modelo de contexto numa perspectiva arquitectural 
a.  Arquitectura de software (utilize o diagrama de componentes) 
b.  Arquitectura de sistema (utilize o diagrama de implantação) 
2.  Elaborar o modelo de contexto numa perspectiva funcional 
a.  Diagrama de contexto (utilize o diagrama de casos de uso e modelo para 
descrever os casos de uso e os actores disponível com este enunciado). 
b.  Agrupe as funcionalidades (utilize o diagrama de pacote) 
c.  Apresente o workflow do sistema (utilize o diagrama de actividades) 
d.  Apresente, graficamente, o fluxo alternativo de cada caso de uso. 
3.  Elaborar o modelo de estrutura 
a.  Apresente o modelo de dados do sistema (utilize o diagrama de classes 
entidades) 
b.  Apresente o modelo de dados do sistema (utilize o diagrama de objectos) 
4.  Elaborar o modelo de interação 
a.  Para cada caso de uso, elabora o diagrama de sequência que descreve a 
interação entre os objectos necessários para implementar o referido caso de 
uso. 
5.  Elaborar o modelo de comportamento 
a.  Elaborar o diagrama de estado do sistema GesTask. 
 

Obs.: Dúvidas sobre o universo de discurso ou informações omitidas podem ser apresentadas ao corpo docente durante a aula. 
 
Engenharia de Software I 
João da Costa  
joao.costa@isptec.co.ao 
ISPTEC / DET / EINF, 2022-23 
