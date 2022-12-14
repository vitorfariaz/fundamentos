# A base desenvolvimento do software

Esse material tem intuito de explicar de forma prática e objetiva o que uma pessoa precisa aprender para se tornar desenvolvedora de software, seja frontend ou backend.


## Qual problema esse material pretende resolver?
  
Se você...
- Não sabe por onde começar e pra onde ir
- Já começou a estudar mas as coisas não entram na sua cabeça
- Não entende o contexto todo e se sente perdido as vezes, como se não soubesse nada
- Não tem noção do que tem pela frente e o que vai precisar aprender
- Como tudo se conecta, a internet, navegador, aplicativo, frontend, backend, etc... NA PRÁTICA!
- Quer uma base sólida, na prática e resumido
- Quer entender na prática o que o dev frontend e o backend fazem e o que precisam saber
- Tá aprendendo HTML e 
  - Não sabe quem transforma o arquivo html no que vemos quando acessamos um site
  - Não sabe como isso chega no dispositivo das pessoas
  - Não sabe onde fica hospedado esse arquivo

Sem ter esse conteúdo base sólido, você não será é um profissional completo e nem vai ir muito longe na carreira
<br />

Se você vai aprender a construir coisas na internet, precisa entender como ela funciona antes
- Um encanador precisa entender como os canos funcionam e como chega a água na casa das pessoas, entre outras coisas
- O eletricista, precisa entender como a eletricidade funciona e como chega na casa das pessoas, entre outras coisas
- O carteiro, precisa entender de onde vem, onde pegar e onde entregar as cartas
- O desenvolvedor, precisa entender como funciona o computador e a internet
  
Recomendação:
[3 técnicas para aprender a programar](https://www.youtube.com/watch?v=ZtMzB5CoekE&ab_channel=FilipeDeschamps)
  
## Qual o resultado esperado ao final desse material

 - Caminho claro do que estudar até saber criar um software e disponibiliza-lo na internet

Obs.: É isso que importa para você conseguir um emprego e não diplomas ou outras coisas...
<br />

Desmistificando algumas coisas
- Você **vai** achar que é burro durante os 6 primeiros meses de estudo.
- Você **vai achar muito difícil** tudo nesses 6 primeiros meses
- Você **vai** achar que precisa de **algo que você não tem** para aprender
- Foi assim com tudo mundo, você não é especial e nem burro
- Não precisa dominar tudo pra: conseguir criar software e disponibiliza-lo na internet e conseguir un emprego, mas é dominar BEM o básico. <br />
- Não é em 1 semana e nem em 12 meses que tu vai dominar tudo. <br />
- Você pode criar um site em 2 dias e disponiza-lo na internet. Mas... Entender o processo inteiro e dominar com confiança, **leva mais de 12 meses estudando 2 horas por dia!** E tá tudo bem... <br />
- Você terá que criar e disponibilizar na internet algumas dezenas de sites até ter confiança e "decorar" o necessário.


# Fundamentos da computação 
O que é um computador? Ou dispositivo celular? <br />
É uma Caixa preta que resolve problemas. <br />

Ele representa e interpreta dados do mundo real, você insere uma informação, ele interpreta, resolve seu problema e retorna uma saída. <br />
![image](https://user-images.githubusercontent.com/40611760/185723359-3d215465-07e6-43b3-b15a-634f43a1bffe.png)

<br />

Como o computador representa, trafega, calcula dados e gera informações?<br />
Com o sistema Binário. <br />

Com binário ele consegue representar números, cor, som, letras, etc... <br />
- Caracteres: ASCII, unicode
- Cores: RGB
- Etc..

Binário é a "linguagem da máquina" pois lida diretamente com as peças físicas do computador. <br />
Nós não precisamos saber disso, pois nós programamos mais "alto nível". A linguagem que usamos para programar 
sabe como traduzir o nosso código "alto nível" em linguagem de máquina. <br />

Exemplo: imagine que você tem o bloco alto nível de código abaixo
```
escreva(''Digite 2 números para que o sistema faca a multipicaçã de um pelo outro)
leia(valor1)
leia(valor2)
real resultado = valor1 * valor2
escreva(''O resultado é: '' resultado)
```

Esse bloco só está criando 3 variáveis e fazendo uma multiplicação. <br />

Isso é o que chamamos de código alto nível pq não precisamos nos preocupar em como o computador(parte física) está guardando esses valores
 na memória, como o computador está mostrando os pixels da mensagem na tela, etc... Pois isso é trabalho da própria linguagem fazer em tempo de execução ou compilação. <br />

Compilação: é quando a linguagem transforma o seu código alto nível em código baixo nível(que será executado pela sua máquina/pc, nesse caso o binário) <br />

Que tipo de problemas um computador pode resolver? <br />
Coisas que exigem grande quantidade de cálculos <br />
Exemplo: imagina que tu tem que procurar um número numa lista telefônica ordenada alfabeticamente com 1 milhão de valores. <br />

Se vc fosse procurar isso manualmente, provavelmente levaria alguns minutos, mesmo com a lista ordenada por ordem alfabética. <br />
Mas se essa lista estivesse reprentada dentro de um computador, ele poderia achar um número em menos de 1 segundo. Esse é o poder da computação. <br />

E como o computador faz isso? ALGORITMOS. <br />

Assim como na vida real, na computação também tem formas eficientes de resolver um problema. <br />
Por exemplo: se você procurar na lista telefônica página por página, vai levar muito até achar, mas se você vai direto na letra que está procurando, vai ser mais rápido... <br />

[Aqui](https://github.com/vitorfariaz/guia-web-developer/blob/main/public/estagio-estudos.md) tem um material com tudo que podemos fazer com algoritmos
<br />

IDE's online:
- https://portugol-webstudio.cubos.io/ide
- https://dgadelha.github.io/tcc-webstudio/

PRÁTICA:
Algoritmo pra calcular o imposto de renda
Usuário digita o salário, e o sistema calcula qual deve ser o descontos de: imposto de renda

```
programa {
    inclua biblioteca Matematica 
    
	funcao inicio() {

		real salario = 0
		real impostoRenda = 0
		real baseSalario1 = 1903.98
		real baseSalario2 = 2826.65
		real baseSalario3 = 3751.05
		real baseSalario4 = 4664.68
		real aliquota1 = 7.5
		real aliquota2 = 15
		real aliquota3 = 22.5
		real aliquota4 = 27.5
		real parcelaDeducao1 = 142.80
		real parcelaDeducao2 = 354.80
		real parcelaDeducao3 = 636.13
		real parcelaDeducao4 = 869.36

		escreva("Digite seu salario: ")
		leia(salario)

		se (salario <= baseSalario1){
		    impostoRenda = 0
		    
		} senao se(salario > baseSalario1 e salario <= baseSalario2 ){
		    impostoRenda = (salario * (aliquota1/100)) - parcelaDeducao1
		    
		} senao se (salario > baseSalario2 e salario <= baseSalario3 ){
		    impostoRenda = (salario * (aliquota2/100)) - parcelaDeducao2
		    
		} senao se(salario > baseSalario3 e salario <= baseSalario4){
		    impostoRenda = (salario * (aliquota3/100)) - parcelaDeducao3
		    
		} senao se(salario > baseSalario4){
		    impostoRenda = (salario * (aliquota4/100)) - parcelaDeducao4
		}
        
                real salarioLimpo = salario - impostoRenda
		escreva("\nSeu salario é: R$", salario)
		escreva("\nDescontos")
		escreva("\nImposto de renda: R$", Matematica.arredondar(impostoRenda, 2))
		escreva("\nSalário limpo: R$",  Matematica.arredondar(salarioLimpo, 2)
	}
		
}


programa {
    inclua biblioteca Matematica 
    
	funcao inicio() {

        inteiro contador = 0
        enquanto (contador < 100){
          escreva("\nContando: ", contador)
          
          contador++;
        }
	}
		
}

```

Isso que passei aqui é a introdução da introdução... Você precisa aprender bem algoritmos, esse é deve ser seu foco. <br />
Quando eu sei que estou bom para ir para o próximo tópico?<br />
Quando vc conseguir resolver exercícios como esses de cor, sem "colar": 
- https://www.inf.pucrs.br/~pinho/LaproI/Exercicios/SeqDecisao/lista1.htm
- https://www.cursoemvideo.com/wp-content/uploads/2020/10/Exerci%CC%81cios-de-Algoritmos-1-100.pdf
Obs.: caso comece a achar os exercícios fáceis(provavelmente vai demorar) ou repetidos, avance para os últimos das listas pois são um pouco mais difíceis
<br />

Cursos sobre algoritmos e fundamentos da computação <br />
[Curso de fundamentos da computação](https://github.com/vitorfariaz/guia-web-developer) 


# Fundamentos da internet 
O que é a Internet? É uma rede de redes.

Tem alguns conceitos que é importante saber
- TCP/IP: é uma Convenção/protocolo: como um computador encontra outro na rede. 
 - Ele lida com o endereço, nome, e pacote de informações trafegadas pela rede
 - Exemplo: Pra enviar uma carta vc precisa de nome, endereço, origem e destino, só que na internet como é muita informação trafegada muito rápida, as vezes não cabe numa carta só, então a informação tem que ir em 4 cartas ou caso a informação se perca no meio do caminho, o protocol TCP resolve

- DNS(lista telefonica): Um computador tem o seu IP, porém nós nos comunicamos pelo nome de um site, o DNS é quem faz essa "tradução".
- PC passa a informação(binário) através de cabo ou wireless de um pc para outro. A informação é passada pro eletricidade pelos cabos, como e binário, um sinal de luz representa 1 e sem sinal de luz representa 0. A informação é enviada em conjunto de binários (algo como código [mors](https://www.youtube.com/watch?v=EvAp7zTjGXo&ab_channel=MarksTuto))
- HTTP: Hyper Text Transfer protocol. É texto/binário que passa de um lado pra outro. mas ele tem um padrão.
  - Cabeçalho. (tipo da request/response, etc..)
  - Corpo
  - Método http 
  - Exemplo: http request é o que vai dentro da carta. Como se tu tivesse que passar o "idioma" do texto da carta, o que tu quer, se vai esperar uma resposta de volta ou se só está "enviando" informações, etc... É a forma como os binários estã organizados dentro de cada envio de informação. O TCP/IP é a parte de fora do envolope e HTTP a parte de dentro.
- HTTP: pq é importante? backend lida bastante com http, pq é basicamente através dele que passamos informações para o frontend
 - Example: http request GET pcdovitor.com/fotodonaruto.jpg. Retorna http status 200 e a cópia de uma foto do naruto do meu PC
- Browser: lida/monta/faz a http request pra nós e interpreta o html para transformar nas coisas que vemos num "site"
 - F12 numa página, aba "network" > recarrega a página. Verá as request http que o browser faz "por baixo dos panos"
- Qual a diferença entre  
 - Internet 
 - Browser
 - Google(motor de busca)
 - Sites
 - Metafora: imagina que seu carro é o computador
   - Internet: é o mundo, tudo que se conecta 
   - Browser: são as estradas, permitem que chegamos de um lugar ao outro
   - Google: é o GPS do seu carro. Ele pesquisa de forma ultra eficiente todas as possíveis rotas de acordo com onde você "quer ir"
   - Sites: são as casas
- Curl: fazendo request http sem o browser
 - Http POST


PRÁTICA: <br />
Retorna valores das açoes na bolsa. (Não oficial)

- Busca cotações histórico por id: GET https://api-cotacao-b3.labdo.it/api/empresa/5/cotacoes/02  
- Busca id das empresas: GET: https://api-cotacao-b3.labdo.it/api/empresa
- Busca cotações do mesmo ativo, para hoje: GET: https://api-cotacao-b3.labdo.it/api/empresa/5/cotacoes
- `curl https://api-cotacao-b3.labdo.it/api/empresa/5/cotacoes/02`
- Pegar o html retorno e criar um arquivo `curl GET http://www.google.com/`


### Resumo até aqui

- Computador só entende binário
- Na rede é passado código binário mas tem um protocolo pra definir como vai ser o padrão desse código: TCP/IP
- DNS traduz a url para o IP do computador na rede
- Quando acessamos algum site nosso navegador está fazendo uma request http para um servidor, passando pelo DNS
- Navegador recebe a resposta do servidor e sabe interpretar o código, se for um arquivo html ele apresenta o site da forma que vemos

![image](https://user-images.githubusercontent.com/40611760/186545862-82d140ea-74d4-4278-929a-1e88b4e8e546.png)
<br />

Isso é so uma introdução, abaixo tem cursos de fundamentos da internet <br />
[Curso de fundamentos da internet](https://github.com/vitorfariaz/guia-web-developer) 


# Frontend

- HTML
  - Não é uma linguagem de programação!
  - É uma estrutura de dados
![image](https://user-images.githubusercontent.com/40611760/185725617-650e16e7-489a-40ba-8f36-2e0968d255bf.png)
  - Quem "entrega" o HTML é um server. Seu computador pode ser um fácilmente. (Várias IDE's disponibilizam um botão para vc habilitar o server no seu pc)
- CSS
  - Aplica propriedades/estilo nos elementos
  - Cor, fonte, tamanho
  - Tabela de propriedade e valor

Exemplo: HTML
```html
<html>
  <head>
    <title>Simple html</title>
  </head>
  <body>
    <h1>This webpage</h1>
  </body>
</html>
```

Exemplo: HTML + CSS
```html
<html>
  <head>
    <title>Body bgcolor Attribute example</title>
  </head>
  <body bgcolor="#afafaf">
    <h1>This webpage has colored background.</h1>
  </body>
</html>
```

Com HTML, podemos fazer várias coisas, foi inovador, foi inventado em 1989 e a última atualização HTML 5 em 2009. (E dizem que dev precisa se atualizar todo dia)

- Javascript
 - NÃO é Java!
 - É uma linguagem de programação
 - Deixa dinamico

Pra que quero deixar minha página HTML dinâmica? <br />
- Pegar/salvar/atualizar uma informação de um banco de dados e na tela
- Aplicar alguma lógica pra processar alguma coisa como:
  - Procurar um nome numa lista
  - Calcular percentual
- Aplicar lógica na interface(se uma pessoa tiver online, um botão fique verde)
- Etc...

Exemplo: HTML + CSS + javascript
```html
<html>

<head>
  <title>Body bgcolor Attribute example</title>
</head>
<script>

  function criaElemento(content) {
    let novaDiv = document.createElement("div"); //button, 
    novaDiv.textContent = content

    let div1 = document.getElementById("div1");
    document.body.insertBefore(novaDiv, div1);

  }

  function criaElementoViaJs() {

    let contador = 0;

    while (contador < 100) {
      criaElemento("Contador: " + contador);
      contador++;
    }
  }

  function getDatatual() {
    var today = new Date();
    var dd = String(today.getDate()).padStart(2, '0');
    var mm = String(today.getMonth() + 1).padStart(2, '0');
    var yyyy = today.getFullYear();
    today = yyyy + mm + dd
    return parseInt(today, 10);
  }

  function buscaIdEmpresa(empresas, codigoAcao) {

    for (var i = 0; i < empresas.length; i++) {
      if (empresas[i].cd_acao_rdz.toLowerCase() == codigoAcao.toLowerCase()) {
        console.log("ACHOU O ID DA AÇÃO: " + empresas[i].id)
        return empresas[i].id
      }
    }
  }

  function encontrarCotacaoDoDia(cotacoes) {

    for (var i = 0; i < cotacoes.length; i++) {

      if (cotacoes[i].cd_bdi == "02" &&
          cotacoes[i].dt_pregao == getDatatual()) {
        console.log("ACHOU A COTAÇÃO DO DIA: " + cotacoes[i].id)
        return cotacoes[i]
      }
    }
  }

  function pesquisarTodasEmpresas() {
    let urlTodasEmpresas = "https://api-cotacao-b3.labdo.it/api/empresa";
    let acao = "petr"

    fetch(urlTodasEmpresas)
      .then(response => response.json())
      .then(empresas => {

        console.log("Busca todas empresas response: ", empresas)

        let id = buscaIdEmpresa(empresas, acao)
        const urlCotacao = `https://api-cotacao-b3.labdo.it/api/empresa/${id}/cotacoes`;

        console.log(urlCotacao)

        return fetch(urlCotacao);
      })
      .then(response => response.json())
      .then(cotacoes => {
        console.log(cotacoes)

        let cotacaoDia = encontrarCotacaoDoDia(cotacoes)

        criaElemento("Código ação: " + cotacaoDia.cd_acao);
        criaElemento("Valor ação: R$" + cotacaoDia.vl_fechamento);

      })
      .catch(function () {
        criaElemento("Deu ruim na busca de todas empresas!")
      });
  }


</script>

<body bgcolor="#afafaf">
  <h1>This webpage has colored background</h1>

  <button style="width: 100px; height: 100px;" onClick="criaElementoViaJs()">
    Botao
  </button>

  <button id="botaoCotacao" style="width: 100px; height: 100px;" onClick="pesquisarTodasEmpresas()">
    BuscaAcao
  </button>

  <div id="div1">
</body>

</html>

```
