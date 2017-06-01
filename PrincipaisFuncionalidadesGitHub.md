# PRINCIPAIS FUNCIONALIDADES DO GITHUB PARA GERENCIAR PROJETOS

## O que é um Issue Tracker?
Um issue tracker funciona como um fórum interno de cada projeto. Nele, podem ser feitas postagens que atendem diversas necessidades 
específicas, além de ser bastante flexível a diferentes usos. Possui suporte a labels (e filtragens pelas mesmas), 
usadas para categorizar issues. 

## O que são Issues?

Uma issue é uma "postagem" contida no issue tracker. Possui um autor, título, número, descrição 
(com suporte a imagens, trechos de código, referências a outras issues em forma de link, linguagem de marcação, etc...) e 
pode ser atribuída a um dos desenvolvedores daquele repositório (como uma forma de dizer: "ei, você cuida disso aqui!"). 
Issues podem ser usadas como uma forma de delegação de tarefas, informar bugs ou até mesmo como documentação. 
Labels são utilizadas como um indicativo visual do que se trata a issue. Podem ser usadas labels para categorizar issues como bugs, 
funcionalidades do sistema, documentação ou até mesmo dúvidas enfrentadas pelos desenvolvedores. Uma coisa que diferencia 
uma issue de uma simples postagem em algum fórum é o fato de que elas podem ser referenciadas em commits feitos ao repositório. 
Essas referências servem para você dizer que há algo naquele commit que influencia a issue em questão. Segue um exemplo de referência 
de uma issue em um commit:

     git commit -m "Resolving bug #16"

Onde #16 é uma issue cadastrada naquele repositório. Issues possuem dois estados: 
aberta e fechada! Uma issue "aberta" é aquela que ainda está em andamento ou não foi resolvida.
Uma issue fechada significa que a atividade que ela descreve já foi realizada! Pode ser uma tarefa feita ou o conserto de um bug.


#### Existem duas formas de fechar um commit: 

Indo na página dela no repositório e clicando em "Close" ou via uma mensagem de commit! 
Por exemplo, suponha que exista uma issue de número #10 e que informa que uma determinada classe de Student deve ser criada. 
O programador responsável por ela, após implementá-la e testá-la, pode fazer o seguinte commit:

      git commit -m "Implementing and testing Student class. Closes #10"
      
As palavras chave:
1.	close
1.	closes
1.	closed
1.	fix
1.	fixes
1.	fixed
1.	resolve
1.	resolves
1.	resolved

##### Issues podem ser vinculadas a milestones para organização de prazos!
 
## O que são Milestones?

Um milestone, como a tradução sugere, são "marcos" do projeto: eventos com uma data, título e descrição que podem funcionar, 
por exemplo, para definir prazos de entrega de funcionalidades. Issues podem ser vinculadas a milestones de forma a indicar que 
as mesmas devem ser fechadas até o prazo estabelecido. Milestones possuem um indicativo visual do progresso das issues nele contidas.
Um exemplo é a definição de entrega de versões do projeto para avaliação do cliente. Vinculam-se as issues referentes as funcionalidades
esperadas pelo cliente, isso serve para ter noção da evolução.

## Usando labels para categorização de issues

Labels são um ótimo indicativo visual sobre do que se trata uma issue, muitas vezes facilitando a busca do desenvolvedor 
por determinado tipo de problema que deve ser resolvido. 

#### Eis alguns exemplos:

• feature: usada em issues que descrevem uma user story ou requisitos do sistema (que não necessariamente possui uma história. 
Exemplo desse caso: "notificações automática", "Envio de e-mail de validação", entre outras). Não vem por padrão no issue tracker 
do GitHub.

•	bug: usada para reportar erros de qualquer tipo, não necessariamente algo que esteja fazendo o sistema "crashear". 
Vem por padrão no issue tracker do GitHub.

•	documentation: aplicada em issues que documentam o projeto de alguma forma. Não vem por padrão no issue tracker do GitHub.

•	front-end: Atividades relacionadas geralmente às views da aplicação ou até mesmo elaboração de mockups ou definição de layouts.
Não vem por padrão no issue tracker do GitHub.

•	test: aplicada em issues relacionadas a testes automatizados de qualquer tipo 
(seja de elaboração ou reportagem da necessidade dos mesmos). Não vem por padrão no issue tracker do GitHub.

•	duplicate: usada para informar que uma issue foi escrita duas vezes. Nesse caso, usa-se esta label em uma das duas e fecha-se a mesma.
Vem por padrão no issue tracker do GitHub.

•	low priority e high priority: reportam issues que podem ser feitas mais posteriormente (low priority) ou imediatamente (high priority).
Não vem por padrão no issue tracker do GitHub. 

##### Nada impede que outras labels sejam criadas dada uma necessidade específica de cada projeto.

## Usando Milestones

O usos deste recurso não varia muito de sua proposta. É criado um milestone para cada sprint(ciclo de desenvolvimento)
dentro do projeto e são estabelecidas que issues devem ser fechadas até o prazo do mesmo. Se porventura alguma issue do milestone 
não for fechada no prazo, ela deve ir para o próximo milestone e categorizada como high priority (tendo que ser resolvida antes de 
qualquer outra issue da sprint seguinte).

Reforça-se que cada desenvolvedor deve fechar todas as issues antes do fim de cada sprint. 
Caso não acredite que seja capaz de cumprir com o prazo, o desenvolvedor deve notificar aos outros membros da equipe o quanto antes.

