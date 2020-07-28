## Redux

Chegou a hora de adicionar Redux à nossa aplicação!

### Instalação das dependências no projeto

- Instale a biblioteca principal [redux](https://redux.js.org/introduction/installation#redux-core);
- Instale a biblioteca utilitária [react-redux](https://react-redux.js.org/introduction/quick-start#installation).

### Configuração Inicial da Store
- Crie sua [**Redux Store**](https://redux.js.org/recipes/configuring-your-store#creating-the-store);
- Utilize o [**Provider**](https://redux.js.org/recipes/configuring-your-store#creating-the-store), fornecido por *react-redux* para permitir que qualquer componente da sua aplicação se conecte à *store*;
- Utilize a função [**combineReducers**](https://redux.js.org/api/combinereducers#reducersindexjs) para ajudar a montar (arquitetar) o formato da sua *Redux Store*.

**Dica**: Você pode, por enquanto, passar um objeto vazio `{}` para *combineReducers*, **pois ainda não escreveu nenhum reducer**.

### Actions e Reducers
- Escreva um **Action Creator** para o carregamento (*LOAD*) de um novo estado global da lista de livros (*books*);
  - Extraia o *type* da Action para uma constante, para que possa ser compartilhado para outros arquivos;
- Escreva seu primeiro **Reducer** (books), tratando adequadamente o disparo da *action* acima;
  - Lembre-se: Reducers devem ser funções puras, recebem uma fatia do estado atual e uma action, e retornam **uma cópia modificada ou um novo estado inteiro**;
  - Mantenha a coerência de tipos entre o estado retornado e o estado inicial declarado;
- Adicione uma referência a seu novo reducer ao objeto passado para *combineReducers*.

### Carregando dados
- Utilize o *hook* **useDispatch** para obter uma referência à função *dispatch* da sua Redux Store dentro do componente **App.js**;
- Dentro de um *effect* de inicialização do componente, consulte os dados remotos referentes aos livros e, em seguida, dispare a *action* que carrega os dadosna sua *store*;
  - Lembre-se de que a chamada remota continua assíncrona e precisa ser tradada!

### Conectando Componentes
- Remova os estados locais dos componentes que guardavam as listas de livros;
  - Por enquanto, atenha-se aos componentes de lista exibidos em *Home* e *Books*;
- Remova os *hooks* de carregamento dos dados nas seções dedicadas;
- Remova as passagens, agora desnecessárias e quebradas, de *props* que se referiam ao estado local e funções que o alteravam;
- Conecte o seu componente principal (**App.js**) à store, utilizando o *hook* [**useSelector**](https://react-redux.js.org/7.1/api/hooks#useselector-examples);
  - Lembre-se de que, diferentemente de dentro dos *reducers*, o **state** aqui se refere ao **estado global completo da aplicação**, não à uma fatia dele;
- Utilize o valor obtido da *store* para renderizar os dados no seu componente;
- Filtre e ordene os dados obtidos normalmente;
- Lembre-se de garantir que o componente não quebre, quando os dados ainda não estiverem carregados na *store* (estado inicial vazio).

### Bônus: Alterando dados na *store*
Caso se sinta confiante com Redux, experimente ir além, criando sua primeira *action* de **alteração parcial de estado** na sua *store*.
- Mude o componente de detalhes de um livro (Book Details) para se conectar à *store*, obtendo a lista e extraindo o livro desejado pelo ID;
- Utilize esse dado para renderizar os retalhes de livros e a lista de *reviews*;
  - Você pode obter a lista de *reviews* independentemente, no seu próprio componente, se quiser. É decisão sua repassar a lista para baixo via *props* ou não;
- Ao adicionar uma nova *review* ao livro, dispare a *action* enviando a nova *review* (e o ID do livro) à store;
- Adicione um *case* no seu *reducer* de livros, que **cirurgicamente** adiciona a review **sem alterar o estado atual diretamente**.