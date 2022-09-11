# lading-page-jquery
## Índice
<!--ts-->
* [Descrição do Projeto](#descrição-do-projeto-)
* [Função](#função-)
* [Tecnologias Utilizadas](#tecnologias-utilizadas-)
* [Como acessar](#como-acessar-)
* [Conhecimentos jQuery](#conhecimentos-jquery-)
* [Autor](#autor-)
<!--te-->
<img src="https://img.shields.io/badge/status-completo-green"><br>

# Descrição do projeto <br>
Uma landing page e compartilhando conhecimentos em jQuery. Na página usei o método `ready()` que disponibiliza uma função depois que o documento for carregado totalmente, fazendo com que a função `slideToggle()` deslize o menu mobile.<br><br>

# Função <br>
![mobile (2)](https://user-images.githubusercontent.com/109925535/189507685-d21cfc7c-eabe-4028-a865-42f4edaa193f.gif)


# Tecnologias Utilizadas <br>
Javascript(jQuery), CSS, HTML.</br>

Note: Media Queries 📲

# Como acessar <br>
<a href="https://maurilosantos.github.io/lading-page-jquery/">Acesse aqui</a>

# Conhecimentos jQuery <br>
É uma biblioteca JavaScript criada por John Resig em 2006. Suas linhas de código simplificam os scripts interpretados pelo navegador do client-side e por esse motivo era uma das bibliotecas mais populares na comunidade de desenvolvedores. Embora haja bibliotecas mais modernas, é bom ter conhecimento caso apareça alguma aplicação web que a utilize.<br><br>
$ —> Símbolo do jQuery. Usado pra selecionar elementos e fazer uma ação;<br>
Biblioteca: `<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.1/jquery.min.js"></script>`<br><br>

Eventos praticados: <br>
```$(".título").hide( );

$(".título").click( );

$(".título").mouseenter( );

$(".título").mouseleave( );

$(".título").dblclick( );
```

Animações:<br>
```$(”#button”).click( ( ) ⇒{ 

$(”#square”).fadeIn( ); 

$(”#square”).faeOut( );

$(”#square”).fadeTo( );

$(”#square”).slideDown( );

$(”#square”).SlideUp( );

$(”#square”).fadeToggle( );

$(”#square”).stop( );
```

Utilizando Callback:<br>
```$("#button").click( () => {
    $("#green").hide(2000, function callback() {
       $("#green").show(2000);
     })
})
```
Selecionando elementos Filhos:<br>
```let lista1 = $("#lista1");
lista1.find().fadeOut() //filtra todos os filhos

lista1.children().fadeOut() // filtra o filho mais direto
```
Encadeamento (chaining):<br>
```let jQ = $("#lista1").slideUp(2000).slideDown(1000).fadeOut(1000);
// as funções executadas em jQ retornam o próprio objeto.
```
Lendo o conteúdo de um elemento:<br>
```$("#lista1").text(); // exibe o conteúdo display
$("#lista1").html(); // exibe o conteúdo com as tags
$("#lista1").val(); // exibe o conteúdo atribuído ao valor
$("#lista1").attr("name"); // exibe o conteúdo do atributo "name" 
```
Selecionando Elementos por Atrbutos:<br>
```// colocamos a [ key ] de um ítem para realizar a ação
$("#lista1").find("[key = 2]").remove()
```
Removendo Elementos:<br>
```$("#lista1").remove(); //remove toda a lista1 inclusive
$("#lista1").empty(); // remove todos os ítens da lista1
$("li").remove(".item1, .item2"); // remove os ítens selcionados
```
Inserino Elementos:<br>
```let lista1 = $("#lista1");

lista1.append("<li>novo elemento</li>"); // adiciona ao fim da lista
lista1.prepend("li>novo elemento</li>"); // adiciona no começo da lista
lista1.after("li>novo elemento</li>"); // adiciona depois da div da lista
lista1.before("li>novo elemento</li>"); // adiciona antes da div da lista
```
Modificando o CSS:<br>
```$("h1").addClass("bg-blue"); // adiciona uma Class
$("h1").removeClass("bg-blue"); // remove a Class
$("h1").css("background-color", "blue") // colocanod fundo azul
$("h1").css({"background-color":"blue", "font-size": "25px"}) // coloca o fundo azul e muda o tamanho da fonte
```
Dimensões:<br>
```let box = $(".box");
box.width();// largura
box.innerWidth(); // largura + padding
box.outerWidth(); // largura + padding + borda
box.outerWidth(true); // largura + padding + borda + margem
```
Elementos Irmãos (Siblings):<br>
```$("#div1").siblings(); // pega todos os elementos irmãos (mesmo nível) da div1
$("#div1").siblings("#div4"); // pega todos com essa id = div4
$("#div1").nextAll(); // pega todos os elementos irmãos declarados depois da div1
$("#div1").next(); // pega o único elemento próximo a div1
$("#div3").prevAll(); // pega todos os elementos antes do div3
$("#div3").prev(); // pega o único elemento anterior a div3
$("#div1").nextUntil("#div4"); //pwga todos os elementos próximo até o div4
$("#div5").prevUntil("#div2"); // pega todos os elementos anteriores até div2
```
Filter, Last, First, e Eq:<br>
```$("div").filter(".div1"); // seleção da div e filtrar apenas quem é div1
$("#container").children().first(); // pegar apenas o primeiro elemento
$("#container").children().last(); // pegar o último elemento
$("#container").children().not("#div8"); // pega todos os elementos menos o div8
$("#container").children().eq(2); // pega o elemento com o índice 2
```


# Autor <br>

[<img src="https://avatars.githubusercontent.com/u/109925535?v=4" width=115><br><sub>Maurilo Santos</sub>](https://github.com/maurilosantos) 



