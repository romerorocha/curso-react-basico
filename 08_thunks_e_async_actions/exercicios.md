## Middleware

- Instale a biblioteca [*redux-thunk*](redux-thunk);
- Configure um *middleware* de thunks para sua aplicação.

**Dica**: A documentação da extensão **Redux DevTools** tem uma [solução elegante](https://github.com/zalmoxisus/redux-devtools-extension#12-advanced-store-setup) para combinar as duas configurações.

## Software

- Evolua a implementação da sua lógica de *actions*, criando *thunks* que tratam chamadas de API e disparam *actions* oportunamente;
- Dispare seus *thunks* nos componentes, substituindo todas as chamadas de API espalhadas pelo código.
- Compare o conteúdo pré e pós modificação (use o **diff do git**!). Responda: O quanto a configuração de um *middleware* de *thunks* pode melhorar a qualidade do seu código de Redux e Integração com APIs?