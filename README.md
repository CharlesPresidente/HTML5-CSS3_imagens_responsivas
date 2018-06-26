# HTML5/CSS3 - Imagens Responsivas

Deixa as imagens com responsividade, se adequando ao tamanho da tela e resolução.

## Arquivos

### .html

	<!DOCTYPE html>
    <html lang="pt">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <meta http-equiv="X-UA-Compatible" content="ie=edge">
        <link rel="stylesheet" href="style.css">
        <title>Imagens Responsivas</title>
    </head>

    <body>
        <header>
            <div>
                <img src="img/img1.jpg" alt="imagem">
            </div>
            <div>
                <img src="img/img2.jpg" alt="imagem">
            </div>
            <div>
                <img src="img/img3.jpg" alt="imagem">
            </div>
            <div>
                <img src="img/img4.jpg" alt="imagem">
            </div>
            <div>
                <img src="img/img5.jpg" alt="imagem">
            </div>
        </header>
    </body>

    </html>

### .css
Destaque para os elementos sinalizados com as setas:

	body {
        background-color: #0b0b0b;
        margin: 0;
    }

    header {
        margin: 0.5vw;
        font-size: 0;
        display: -ms-flexbox; <--
        -ms-flexbox-wrap: wrap; <--
        -ms-flexbox-direction: column; <--
        -webkit-flex-flow: row wrap; <--
        flex-flow: row wrap; <--
        display: -webkit-box; <--
        display: flex; <--
    }

    header div {
        -webkit-box-flex: auto; <--
        -ms-flex: auto; <--
        flex: auto; <--
        width: 200px;
        margin: 0.5vw;
    }

    header div img {
        width: 100%;
        height: 85%;
    }

    @media screen and (max-width: 400px) { <--
        header {
            padding: 0;
        }
        header div {
            margin: 0;
        }
    }
