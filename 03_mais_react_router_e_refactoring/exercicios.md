### Refactoring

Refatoração contínua é uma prática saudável e encorajada em times de desenvolvimento profissionais. Neste exercício, procure pontos de melhoria, nos componentes que você construiu enquanto aprendia os assuntos passados. Tente pensar em termos de:
- Melhor legibilidade;
- Componentes pequenos, genéricos e reutilizáveis;
- Melhor colocação do estado e diminuição do tráfego de props entre múltiplas camadas;
- Formas elegantes, porém mais simples e diretas, de resolver problemas como *sorting* e *filtering*.

**Dica**: Aprenda as particularidades de JavaScript, principalmente se estiver migrando de outra linguagem.

### React Router

Agora que criamos nossas primeiras rotas, vamos nos aprofundar na biblioteca que é o core das SPA React.

- Se ainda não o fez, crie a rota (e o componente) para listar os "Books" fornecidos pela API;
- Exiba a lista de livros, com *nome* e *review count*;
- Crie a rota de "Book Details", para exibir as informações detalhadas de um livro;
- Crie um Link no título de cada Book, levando-o para sua página de detalhes;
- Consulte os detalhes, obtendo o *id* do Book dos parâmetros da rota;
  
A seção de "Book Details" será incrementada nas próximas aulas. Por enquanto, nosso foco será o trabalho com as rotas, navegação e obtenção de parâmetros.

**Cuidados**:
- Trate possíveis pontos problemáticos na renderização de dados obtidos na API;
- Previna-se de possíveis erros: IDs de livros inexistentes, renderização de dados iniciais e null pointers.


