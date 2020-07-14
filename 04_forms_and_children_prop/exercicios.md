### Refactoring

A prop **children** nos ajuda a passar uma hierarquia de componentes como propriedade para um componente em React.

- Escreva um componente que representa o bloco "Conteúdo de Página", reutilizável para todas as seções da aplicação, utilizando a prop *children*;
- Mova, para o componente, a lógica de exibição de cabeçalho da seção (por exemplo, a corta corrente);
- Utilize este componente, encapsulado o código JSX retornado em cada seção principal da aplicação (por exemplo, componentes *Home*, *Movies*, *Book*, *BookDetails*, etc.)

### Forms e Listas de Dados

Na página de detalhes de um livro:
- Crie uma lista de exibição de *reviews*;
- Crie um *form* para adicionar reviews, contendo nome do autor da review, nota e texto do comentário;
  - Valide se a nota se encaixa entre os valores 0 e 5;
  - Transforme seus inputs em **componentes controlados**, associando-os a um estado e criando os métodos de tratamento dos seus respectivos eventos;
  - Adicione os botões *Submit* e *Delete*;
  - Escreva a lógica de *submit*, integrando o formulário com a API remota;
  - Escreva a lógica de *delete*, integrando o formulário com a API remota;
  - Trate os retornos da chamada da forma devida, adicionando/removendo a *review* recém-criada à lista de *reviews*.
- Crie um botão que exibe/oculta o formulário;