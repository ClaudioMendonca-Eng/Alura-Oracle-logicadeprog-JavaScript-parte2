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
- [Funções com retorno](#funcoes-com-retorno)
- [Tipo booleano](#tipo-booleano)
- [Verificando o chute](#verificando-o-chute)
- [Contando tentativas](#contando-tentativas)
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

## <a name="funcoes-com-retorno"> Funções com retorno </a>

Estou introduzindo a criação de funções com retorno para gerar um número aleatório em nosso código. Começo definindo uma função chamada gerarNumeroAleatorio, utilizando Math.random() para gerar um número entre 1 e 10. Destaco a importância da palavra-chave return para indicar que a função deve nos devolver esse número.

Demonstro como armazenar o resultado da função (o número gerado) em uma variável chamada numeroSecreto. Explico que essa função é diferente das anteriores, pois ela retorna uma informação que queremos armazenar.

Mostro que existem diferentes modelos de funções: aquelas sem parâmetros e sem retorno (como verificarChute()), aquelas com parâmetros e sem retorno (como exibirTextoNaTela(tag, texto)), e finalmente, aquelas sem parâmetros e com retorno (como gerarNumeroAleatorio()).

Testo a função, imprimindo o número secreto no console quando o botão "Chutar" é clicado. Observo que o número é gerado apenas na primeira vez que a função é chamada, e subsequentes chamadas apenas imprimem o mesmo número. Destaco a necessidade de entender quando e como invocar funções para obter resultados desejados.

Concluo destacando que agora estamos atribuindo funções a variáveis, uma nova abordagem em relação às variáveis que antes armazenavam apenas strings ou números.

## <a name="tipo-booleano"> Tipo booleano </a>

Agora estou lidando com a interação do usuário no campo de entrada do HTML, onde ele insere um número entre 1 e 10. Ao clicar no botão "Chutar", quero capturar o valor inserido nesse campo e compará-lo com o número aleatório gerado. Começo selecionando o campo input usando document.querySelector('input') e obtendo o valor inserido usando .value. Faço uma comparação, verificando se o valor inserido (chute) é igual ao número secreto (numeroSecreto), e imprimo o resultado no console.

Explico a razão de usar .value em vez de simplesmente armazenar o campo como fizemos com o título e o parágrafo. Destaco a diferença entre = (atribuição) e == (comparação) em JavaScript.

Testo a comparação no console, e como resultado obtenho false, que é um valor booleano indicando que o chute não é igual ao número secreto.

Demonstro que o tipo booleano (verdadeiro ou falso) é comum na programação, explicando como o JavaScript interpreta esses valores. Faço uma manipulação temporária para atribuir um número específico (5) à variável numeroSecreto e, ao inserir 5 no campo de input, obtenho true no console, indicando uma correspondência verdadeira.

Concluo ressaltando a aprendizagem contínua sobre tipos de dados, como string, número e booleano. A seguir, sugiro a possibilidade de usar uma alternativa ao console para exibir uma resposta mais compreensível na tela.

## <a name="verificando-o-chute"> Verificando o chute </a>

Agora, estou implementando a lógica de jogo para fornecer feedback ao usuário após inserir um número no campo de input e clicar no botão "Chutar". Uso estruturas condicionais if() e else() para verificar se o chute é igual ao número secreto ou não.

Explico que ao acertar, exibo mensagens no console e na tela usando a função exibirTextoNaTela(). Testo essa funcionalidade e ajusto as mensagens para indicar que a pessoa acertou e descobriu o número secreto.

Introduzo uma lógica para mensagens de erro, onde informo se o número é maior ou menor que o número secreto. Uso o número gerado aleatoriamente como número secreto e testo o jogo.

Destaco que, mesmo sem alertas e prompts, conseguimos entender a dinâmica do jogo, criar funções e usar retornos. Destaco que há desafios a serem enfrentados nas etapas subsequentes.

## <a name="contando-tentativas"> Contando tentativas </a>

Estou adicionando a funcionalidade de exibir o número de tentativas no jogo que desenvolvemos. Introduzo uma variável chamada tentativas na linha 2 e inicializo com o valor 1, considerando que a primeira tentativa já ocorre no início do jogo.

Atualizo o texto da tag p para incluir a informação sobre o número de tentativas. Utilizo uma template string e a variável tentativas para exibir a mensagem adequada, levando em consideração a conjugação correta da palavra "tentativas" no plural ou singular.

Introduzo uma lógica para determinar se devo usar "tentativas" ou "tentativa" com base no valor de tentativas. Crio a variável palavraTentativa na linha 17 e a utilizo na mensagem exibida.

Ajusto a contagem de tentativas no código, incrementando a variável tentativas sempre que o chute é errado.

Testo o jogo, verificando se as mensagens são exibidas corretamente para diferentes situações, incluindo acertos e erros. Destaco que a contagem considera apenas tentativas erradas, não contabilizando acertos subsequentes.

Ao final, restauro a geração aleatória do número secreto para manter a dinâmica do jogo.




