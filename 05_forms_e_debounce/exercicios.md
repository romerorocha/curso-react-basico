### *Forms*

Na lista de *reviews* de um livro (seção de detalhe do livro), implemente o evento de clique do botão "Edit", presente em cada item, observando que:
- Quando o usuário clica no botão, os dados da *review* selecionada devem preencher os campos do mesmo *form* de "Add Review";
- O clique, simultaneamente, deve fazer o *form* aparecer (este estava oculto); 
- Se o usuário clicar no botão "edit" de um item, quando outro já estiver sendo exibido para edição, os dados devem ser devidamente substituídos, enquanto que o *form* deve permanecer ativo;
- Utilize o mesmo botão do *form* para as operações "adicionar" e "editar";
- Atualize os dados da UI de forma síncrona com a atualização do servidor;
- Limpe os campos do *form* após edição e faça com que seja ocultado.

**Dica**: Preocupe-se em fazer o comportamento da edição funcionar de ponta a ponta, UI e *server*. Depois, você poderá melhorar a forma como escreve a lógica do *submit*, diminuindo a quantidade de código repetido e "fugindo" (quando possível) da programação imperativa. Lembre-se: o paradigma **declarativo** é um dos seus melhores amigos em React.

### *Debounce*

- Crie uma nova seção (e o seu respectivo menu) para sua aplicação: Characters (personagens);
- Comece com uma busca **por nome** de personagens. Note que podem existir vários personagens para cada nome ou prefixo;
- Exiba os resultados em uma lista, abaixo do campo de busca;
- Trate adequadamente o evento de busca:
  - Evite buscas inúteis, como com nome em branco: limpe a lista, quando isso ocorrer;
  - Evite disparar sucessivos requests, quando somente um é necessário: instale uma biblioteca que implementa *debounce* e configure esse comportamento.

Não deixe de visitar a seção [links úteis](links_uteis.md) desta aula :exclamation: