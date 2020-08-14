## Iniciando a versão 2.0

Chegou a hora de reorganizarmos nosso projeto, nos preparando para grandes mudanças que virão na versão 2.0! Para isso, temos que considerar alguns aspectos.

### Gerência de Configuração

- Integre, se ainda não o fez, todas as mudanças feitas até agora no *branch* principal (**master**) do seu repositório;
  - \[**OPCIONAL**\] Marque uma tag para a versão 1.0 que concluímos.
- Crie um *branch* dedicado para o desenvolvimento da versão 2.0. Não se esqueça ade usar um nome que tenha significado para o que estará sendo desenvolvido. Por exemplo, **v2_material_ui**.
- Faça o *checkout* local do *branch* recém criado. Seguiremos nele até o final do módulo.
- Apesar de estar em um *branch* à parte do principal, siga as mesmas boas práticas de GC durante o desenvolvimento:
  - *Commits* atômicos e concisos;
  - Mensagens não muito longas, mas com bom significado;
  - Código no repositório remoto sempre testado e estável.

### Estrutura de pastas do projeto

Hora da faxina!

- Remova pastas e arquivos que são particulares da primeira versão:
  - Arquivos CSS;
  - Actions;
  - Reducers;
  - Componentes das "páginas" da aplicação;
  - Componentes auxiliares ou de seções de página da aplicação;
- Remova referências aos arquivos e pastas apagados no seu código;
- Remova configurações referentes a estes arquivos;

Você pode manter pedaços que são uma espécie de *standard* para aplicações do tipo, como: configuração da Redux Store, configuração de ferramentas auxiliares (ex. Axios) e camada de integração com a API.

Feita a limpeza, faça um *commit* das mudanças, demarcando o ponto inicial dos trabalhos.

### Configuração da biblioteca Material-UI
- Siga os [passos de instalação](https://material-ui.com/getting-started/installation/) da bibliotecas de componentes **Material-UI**;
  - Prefira adicionar as fontes pelo [método do CDN](https://material-ui.com/components/typography/#general);
  - Prefira instalar [ícones SVG](https://material-ui.com/components/icons/#installation);
- [Faça o teste](https://material-ui.com/components/icons/#installation), utilizando um simples componente e garantindo que a sua configuração funciona.

### \[BÔNUS\] Primeiras funcionalidades do projeto

- Crie as rotas da sua aplicação, com base no que já tínhamos na primeira versão;
- Experimente criar menus com botões, barra de título e [usar estilos](https://material-ui.com/styles/api/#examples-3).

A documentação da biblioteca é muito rica, com extensa descrição da API dos componentes e um *showcase* muito completo. Acostume-se a consultá-la, ela será sua melhor amiga durante o desenvolvimento do projeto.