# Projeto Natours sobre css e sass avançado

- 3 PILARES PARA UM BOM SITE FEITO EM HTML E CSS
  -> Design responsivo
    : Site que funcione perfeitamente em qualquer tamanho de tela
  -> Manutenibilidade e escalabilidade do codigo
    : Importante para o dev , pois posteriormente o codigo pode ser passado para outra pessoa
    : codigo legivel e entendivel pelo dev
  -> Performance do Site
    : Site rapido
    : Site menor
    : Fazer com que o usuario tabalhe com menos dados

# BEM

- Estrutura bem definida para organização das classes no CSS
- Dividida em 3 partes
  ->
  ->
  -> Modificadores

# SASS

- È um CSS pré-processador, uma extensão do css que adiciona potência e elegância a linguagem básica.
- Usado para corrigir os problemas gerados pelo CSS.
- Oferece ferramentas e recursos que o css não possui.
  ->variaveis: **para reutilizar valores como colors,fonts-sizes,espaçamento,etc.**
  ->Nesting: **para aninhar seletores dentro um do outro**
  ->Operadores: **para operações matematicas dentro do css**
  ->Imports: **nos permite escrever css em arquivos diferentes, e importa-los em um unico arquivo**
  ->Mixins: **para reescrever partes reutilizáveis do código css**
  ->Funções: **para produzir valores e reutiliza-los mais tarde, parecido com os mixins**
  ->Extends: **Faz com que diferentes seletores herdem declarações para todos eles**
  ->Control Directives: **permitem escrever condições e loops como na linguagem de programação**

  # instalando o SASS
  
  - Usando o NPM
  - Digitar no CMD : npm init
  - Digitar no CMD : npm install node-sass --save-dev
  - Digitar no CMF : npm install jquery --save
  - Desinstalar: npm uninstall jquery --save - Não vamos usar

  # usando o SASS
  - Escreva no script : "compile:sass":"node-sass sass/main.scss css/style.css -w"
  - Rode o comando : npm run compile:sass

  //  "compile:sass":"node-sass sass/main.scss css/style.css -w"

  # ESTRUTURA

  abstract - vai conter nosso css com variaveis, mixins, aninhamentos, etc.
  base - animações, tipos, utilidades, etx.
  main - todos os CSSs vão ser importados aqui
  css - contendo o css final depois de compilado.
  img - storage de imagens
  index.html - nosso arquivo principal
  componentes - são as paginas do nosso site, devem ser independentes - manutentabilidade.
  layout - vão conter os layouts globais que vão estar em todo o site, ex : cabeçalho, rodapé,etc.
  pages - aqui vai estar nossa home page.

  # trabalhando com filhos herdados.

  No css não é possivel estilizar o checkbox, logo tem-se uma maneira de estilizar outro
  elemento no lugar do checkbox e usar ele como se fosse um checkbox
    - esconde o checkbox
    - por cima coloque o elemento estilizado
    - verificar se o checkbox está checked, caso sim , use &__checkbox:checked + &__label
      e coloque como valor opacity: 1 para mostrar o elemento.

  # Ancora

  criamos uma id pra sessão e referenciamos essa id no a href que você quiser.



