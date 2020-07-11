### Integração com APIs externas

- Incremente sua camada de integração com a API, consumindo o serviço REST de atualizar (PATCH) um filme, com base na Swagger da API;
- Utilize esse serviço para persistir as mudanças dos filmes entre estantes;
- Faça a atualização da sua UI no momento oportuno, depois que os dados são gravados;
- Refatore sua aplicação, tentando reaproveitar a mesma função de update para todas as operações de mudança de estado nas listas.

### Sorting

Implemente as funcionalidades de *sorting* nas suas listas de filmes. Cada lista deve poder ser ordenada:
- por nome do filme (ordem alfabética, **crescente**);
- por quantidade de prêmios recebidos (número de Academy Awards, **decrescente**);
- uma lista deve ter ordenação independente das outras.

### React Router

- Adicione a biblioteca [React Router](https://reactrouter.com/web/guides/quick-start) no seu projeto;
- Crie suas primeiras rotas (Home e Movies), substituindo o "Router" temporário, que criamos na primeira aula.

### Desafio Bônus

Adicione à sua aplicação uma seção "Books".

- Crie o componente que consulta e exibe a lista de livros;
- Declare a rota para esse componente;
- Atualize o menu de navegação da aplicação.