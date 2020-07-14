### *Refactoring*

A prop **children** nos ajuda a passar uma hierarquia de componentes como propriedade para um componente em React.

- Escreva um componente que representa o bloco "Conteúdo de Página", reutilizável para todas as seções da aplicação, utilizando a prop *children*;
- Mova, para o componente, a lógica de exibição de cabeçalho da seção (por exemplo, a rota corrente);
- Utilize o componente em cada seção principal da aplicação (por exemplo, componentes *Home*, *Movies*, *Book*, *BookDetails*, etc.), encapsulado o código JSX retornado.

### *Forms* e Listas de dados

Na página de detalhes de um livro:
- Crie uma lista de exibição de *reviews*;
- Crie um *form* para adicionar reviews:
  - Adicione o nome do autor (da *review*), a nota e o texto do comentário ao formulário;
  - Valide se a nota se encaixa entre os valores 0 e 5;
  - Transforme seus inputs em **componentes controlados**, associando-os a um estado e criando os métodos de tratamento dos seus respectivos eventos;
  - Adicione os botões *Submit* e *Delete*;
  - Escreva a lógica de *submit*, integrando o formulário com a API remota;
  - Escreva a lógica de *delete*, integrando o formulário com a API remota;
  - Trate os retornos das chamadas remotas da forma devida, adicionando/removendo a *review* recém-criada/apagada na lista de *reviews*.
- Crie um botão parar exibir/ocultar o formulário;