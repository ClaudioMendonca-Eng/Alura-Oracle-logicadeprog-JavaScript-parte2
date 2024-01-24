# Alura - ONE Oracle Next Education T6
# Lógica de programação: explore funções e listas - 2º PARTE

Atualmente, estou participando ativamente do programa ONE Oracle Next Education T6, uma colaboração entre a Oracle e a Alura. Estou genuinamente desfrutando da experiência educacional oferecida por este curso, que está focado no aprendizado de Lógica de Programação e na exploração dos fundamentos da programação com JavaScript.
#oraclenexteducation #alura #HelloONET6 #aluracursos #aluraonline #aluraone #aluraoneoracle #aluraoneoracleeducation #aluraoneoracleeducationt6 #aluraoneoracleeducationt6claudiomendon

![](img/imagemgamer.png)

## Índice

- [Instrutores](#instrutor)
- [Apresentação](#apresentacao)
- [Manipulando textos](#manipulando-textos)
- [Criando uma função](#criando-uma-funcao)
- [Funções com parâmetros](#funcoes-com-parametros)
- [Conclusão](#conclusao)
- [Licença](#licença)

## <a name="instrutor"> Instrutores </a>

[Mônica Hillman](https://github.com/MonicaHillman) - Desenvolvedora de software há mais de 20 anos, com experiência em diversas linguagens e tecnologias. Atualmente, trabalha como desenvolvedora e consultora independente, além de ser instrutora na Alura.

[Guilherme Lima](https://github.com/guilhermeonrails) - Desenvolvedor de software há mais de 10 anos, com experiência em diversas linguagens e tecnologias. Atualmente, trabalha como desenvolvedor e consultor independente, além de ser instrutor na Alura.

A lógica de programação nada mais é do que uma sequência de passos para resolver um problema. Quem vai resolver o problema, nesse caso, é o computador, baseado nas instruções que passamos para ele. Então, precisamos saber quais tipos de instruções o computador entende e qual a melhor forma de passarmos os comandos para nos comunicarmos com ele.

## <a name="apresentacao"> Apresentação </a>

No primeiro curso, utilizamos bastante alert e prompt para interação. Entretanto, ao acessar um e-commerce ou site, não é comum que essas janelas fiquem surgindo na tela, concorda?

Neste curso, nosso objetivo principal é explorar como podemos usar o JavaScript para interagir com a tela de maneira mais sofisticada, semelhante às ferramentas que encontramos no dia a dia. Além disso, vamos consolidar os conhecimentos de lógica de programação e aprimorar nosso projeto do número secreto, incorporando novas funcionalidades e tornando-o visualmente mais atraente. Vamos lá!

## <a name="manipulando-textos"> Manipulando textos </a>


Vamos iniciar nossos estudos analisando o projeto baixado para este treinamento. No Visual Studio, abrimos o projeto, composto pelos arquivos index.html, style.css e app.js, sendo este último o foco do desenvolvimento.

Apesar de semelhante ao curso anterior, há diferenças notáveis. Ao clicar com o botão direito no index.html, optamos por "Open with Live Server" para visualizar o projeto no navegador. A aparência é agora mais próxima de um site real.

A tela mostra uma caixa de texto para inserir o número secreto, botões "Chutar" e "Novo Jogo", e um personagem à direita. O uso do alert prompt foi substituído, destacando a interação direta com o HTML.

A manipulação visual com JavaScript torna o projeto mais dinâmico. Exploramos a seleção de elementos HTML, exemplificada com h1 e p. A tag h1, representando o título principal, é acessada no JavaScript por meio de document.querySelector('h1').

Ao criar a variável "titulo", aplicamos titulo.innerHTML para modificar o conteúdo da tag h1, exibindo "Jogo do número secreto". Similarmente, selecionamos e alteramos o conteúdo do parágrafo (tag p) usando paragrafo.innerHTML.

Essa dinâmica proporciona uma experiência mais realista, evitando prompts invasivos. As alterações feitas refletem um título "Jogo do número secreto" e um parágrafo com "Escolha um número entre 1 e 10" acima da caixa de texto.

## <a name="criando-uma-funcao"> Criando uma função </a>

Estou enfrentando o desafio de reconhecer e implementar a funcionalidade dos botões "Chutar" e "Novo jogo" no projeto. O botão "Novo jogo" está atualmente desabilitado, focando no jogo atual. Nosso objetivo é criar uma ação ao clicar em "Chutar".

Para isso, inspecionamos o botão "Chutar" no HTML, adicionando um elemento onclick com a função "verificarChute()" para indicar que algo deve acontecer no JavaScript quando o botão for clicado.

A função "verificarChute()" é então implementada no arquivo app.js. No HTML, usamos onclick para referenciar a função JavaScript com o mesmo nome. A função JavaScript é introduzida com a palavra-chave "function".

Dentro da função "verificarChute()", definimos o escopo com chaves, onde realizaremos as verificações. Lembre-se da importância de dar nomes descritivos a funções.

A função atual exibe a mensagem "O botão foi clicado!" no console, marcando o funcionamento correto do botão "Chutar". Essa ação é um passo inicial para a implementação mais detalhada do jogo.

## <a name="funcoes-com-parametros"> Funções com parâmetros </a>

Estou explorando a criação e uso de funções, focando em funções com parâmetros. Ao revisar o código, percebo que mesmo para ações diferentes, como manipular elementos distintos (h1 e p), as estruturas são semelhantes. Criamos variáveis para armazenar seleções de elementos e as utilizamos para alterar seus textos.

Embora os campos (título, parágrafo) e tags (h1, p) variem, a lógica subjacente é a mesma. Destaco a possibilidade de aprimorar a eficiência e clareza do código usando funções.

Então, introduzo a função exibirTextoNaTela(tag, texto), que recebe uma tag e um texto como parâmetros. Dentro da função, selecionamos o elemento com a tag fornecida e atualizamos seu conteúdo com o texto.

Demonstro como chamar essa função para manipular tanto o h1 quanto o parágrafo, fornecendo as tags 'h1' e 'p' como argumentos, respectivamente. Além disso, especifico os textos desejados, como 'Jogo do número secreto' e 'Escolha um número entre 1 e 10'.

Exploro a flexibilidade do JavaScript, mostrando que a ordem de declaração e chamada de funções não é restrita. Comento sobre a importância de nomear funções de forma descritiva e explico como as funções com parâmetros podem ser poderosas para tornar o código mais dinâmico e reutilizável.


