# Website-acess-vel
Protótipo de um website em construção com interface, pluggins e softwares woltados para atender as demandas das pessoas com deficiência, especialmente pessoas com daltonismo, baixa visão, visão monocular. Por isso, você conseguirá ver a codificação para pluggins de leitores de tela e leitura em LIBRAS.
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="author" content="Nayara dos Santos ">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Projeto 1</title>

    <style>

        h1{
            text-align: center;
        }
        body {
			padding:0px;
			margin:0px;
            text-align: justify;
            font-family: Arial;
		}
 
		#menu ul {
			padding:0px;
			margin:0px;
			float: left;
			width: 100%;
			background-color:#EDEDED;
			list-style:none;
			font:80% Tahoma;
		}
 
		#menu ul li { display: inline; }
 
		#menu ul li a {
			background-color:#EDEDED;
			color: #333;
			text-decoration: none;
			border-bottom:3px solid #EDEDED;
			padding: 2px 10px;
			float:left;
		}
 
		#menu ul li a:hover {
			background-color:#D6D6D6;
			color: #6D6D6D;
			border-bottom:3px solid #221d1d;
		}
	
       div{
           text-align: center;
       }
   
        .destaque{
           text-align: justify;
           font-family: 'Times New Roman', Times, serif;
           font-size: 14px;
           margin-left: 400px;
           margin-right: 400px;
       }
       .formulário{
           text-align: left;
       }

       .contrast h1, .contrast h2,.contrast p, .contrast label,
       .contrast i, .contrast b, .contrast u,.contrast span {
            color: white !important;
        }

       .contrast,.contrast nav,.contrast div,.contrast li,.contrast ol,
       .contrast header,.contrast footer,.contrast main,
       .contrast aside {
            background: black !important;
            color: white !important;
        }
        .contrast a{
            color: yellow !important;
        }

    .contrast button, .contrast input[type=button], .contrast input[type=reset],
    .contrast input[type=submit] {
        background: black !important;
        color: yellow !important;
        border: none !important;
    }

    .contrast img.on-contrast-force-gray {
        filter: grayscale(100%) contrast(120%);
    }

    .contrast img.on-contrast-force-white {
        filter: brightness(0) invert(1);
    }

    .contrast img.on-contrast-force-gray {
        filter: grayscale(100%) contrast(120%);
    }

    .contrast img.on-contrast-force-white {
        filter: brightness(0) invert(1);
    }

    .gif{
        text-align: center;
    }
    
    </style>

    <!--Função alto contraste no site -->
    <link rel="stylesheet" href="./css/contrast.css">

    <script type="text/javascript">
        $(document).ready(function() {
            $("#menu li a").click(function() {
                $("link").attr("href",$(this).attr('rel'));
                return false;
            });
        
            $(".iautocontraste a").click(function() {
                $("link").attr("href",$(this).attr('rel'));
                $(this).attr('rel',($(this).attr('rel')=="autocontraste.css") ? "style.css" : "autocontraste.css");
                return false;
            });
        });
    </script>

</head>
<body>
    <!-- Inserção do plugin de tradutor de LIBRAS no site -->
    <ui-view></ui-view>
 
   <script src="https://plugin.handtalk.me/web/latest/handtalk.min.js"></script>
   <script>
     var ht = new HT({
       token: "..."
     });
   </script>
 
    
    <!-- Inserção de formulário -->
        <link rel="stylesheet" type="text/css" href="css/estilo.css">
        <!--[if IE]>
        <link rel="stylesheet" type="text/css" href="css/estiloie.css">
        <![endif]-->

</body>

<!-- Inserção de Menu Horizontal -->
    <div id="menu">
    <ul>
        <li><a href="">Home</a></li>
        <li><a href="">Sobre</a></li>
        <li><a href="">Artigos</a></li>
        <li><a href="">Diretório</a></li>
        <li><a href="">Links</a></li>
        <li><a href="">Contato</a></li>
    </ul>

    <div class="acessibilidade-exemplo"><ul>  
        <li class="iaumentar"><a class="aumentar" href="#" title="Aumentar fonte">Aumentar Fonte</a></li>  
        <li class="inormal"><a class="normal" href="#" title="Tamanho normal da fonte">Tamanho Normal</a></li>  
        <li class="idiminuir"><a class="diminuir" href="#" title="Diminuir fonte">Diminuir Fonte</a></li>  
        <li class="iautocontraste"><a class="autocontraste" href="#" rel="autocontraste.css" title="Alto Contraste">Alto Contraste</a></li>  
        </ul>  
        </div> 

    </div>

     <!-- Conteúdo -->

     <h1><b>Projeto de Teste 1</b></h1>
     <div>
        <img src="diversidade e inclusão.jpg"></imgsrc>
        <p class="destaque"><i><smal>
            #PraCegoVer:</i> Imagem em formato retangular com fundo escuro e rústico.
            No centro da imagem há uma placa azul com o conteúdo: diversidade e inclusão no idioma inglês.
            Ao redor da placa há bonecos coloridos no formato do corpo humano.
        </smal></p>
    </div> 

    <h2>Mercado de trabalho após 40 anos</h2>
    <p>É comum nos sentirmos sozinhos e com baixa autoestima nesse momento. As pessoas que estão trabalhando e vivendo suas rotinas parecem viver em outra dimensão, enquanto as que estão na busca por um caminho enfrentam uma ansiedade muito grande, afinal, procurar trabalho pode ser, muitas vezes, o pior trabalho do mundo.</p>

    <h2>Mercado de trabalho para pessoas com deficiência</h2>
    <p>Segundo o educador Marcos José da Silveira Mazzotta, pode-se dizer que a questão da pessoa com deficiência passou, ao longo da história, da ‘marginalização’ para o assistencialismo e deste para a educação, reabilitação, integração social e, mais recentemente, para a inclusão social.</p>
    
    <h2>Formulários para pessoas com daltonismo, baixa visão ou hipersensibilidade</h2>
    <p>Uma das formas de se promover a acessibilidade é a utilização de diretórios e/ou seções que se adequem
        à deficiência ou dificuldade visual da pessoa, como por exemplo, evitar usar muitas cores em formulários 
        no site ou possibilitar a alteração e adequação da cor do formulário à necessidade da pessoa que está preenchendo. Por exemplo:
    </p>
    <section>
        <figure class="gif">
            <img src="form.gif">
        </figure>
    </section>

    <!-- Inserção de formulário -->
   <div>
    <div id="area">
        <form id="formulario" autocomplete="off">
          <fieldset>
            <legend>Formulário</legend>
            <label>Nome:</label><input class="campo_nome" type="text"><br>
            <label>Email:</label><input class="campo_email" type="password"><br>
            <label>Mensagem:</label><br><textarea class="msg" cols="35" rows="8"></textarea><br>
            <input class="btn_submit" type="submit" value="Enviar">
          </fieldset>
        </form>
      </div>
     </div>
   

</html>
