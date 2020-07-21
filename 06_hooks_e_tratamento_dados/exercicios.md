### React Hooks

- Converta os componentes de classe para componentes do tipo **função**;
- Utilize *hooks* demonstrados na aula para substituir a variável *state* e os métodos de ciclo de vida do componente;
- Utilize *hooks* do React Router, substituindo as funcionalidades parecidas já utilizadas.

**Dica**: Diferentemente do `this.setState` nas classes, a função de *set* retornada pelo *useState* **não faz um merging** de propriedades do objeto recebido como parâmetro. O valor passado será o novo valor do estado declarado.

Sendo assim, prefira uma estrutura mais *flat* para o estado do seu componente, chamando *useState* quantas vezes precisar.

### Characters

- Seguindo com as funcionalidades sobre personagens, crie um *Link* no nome de cada personagem listado na busca já implementada, que leva para a página de detalhes desse personagem;
- Crie a página de detalhes de personagem, realizando a busca por ID, quando essa página carrega;
- Trate adequadamente os dados no retorno da consulta:
  - Exiba uma mensagem que informa que o personagem não existe para determinado ID, se for o caso;
  - Implemente um comportamento de loading, para evitar um carregamento precoce da mensagem errada;
  - Formate os dados do personagem de forma amigável. Exiba de forma condicional os dados que julgar não obrigatórios.