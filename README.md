*,
*::before,
*::after {
    --azul-profundo: #01080E;
    --azul-escuro: #041832;
    --azul-medio: #144480;
    --azul-destaque-light: #1875E9;
    --azul-destaque-dark: #3985D8;
    --cinza-escuro: #222222;
    --cinza-medio: #C5C5C5;
    --cinza-claro: #F2F2F2;
    --branco: #FFFFFF;
    box-sizing: border-box;
}

body {
    font-family: Roboto, Arial, Helvetica, sans-serif;
    background-color: var(--branco);
    position: relative;
    width: 100%;
    height: 100vh;
    overflow: auto;
    font-size: 14px;
    color: var(--cinza-escuro);                                                            
    box-sizing: border-box;
    text-align: center;
}

/* CABEÇALHO */

.cabecalho__container {
    background-color: var(--branco);
    height: 80px;
    width: 100%;
    padding: 0 25px;
}

.logo__item {
    padding: 15px 0px;
    cursor: pointer;
}

.pesquisar__input {
    padding: 8px;
    border: 2px solid var(--cinza-claro);
    border-radius: 32px 0px 0px 32px;
    font-size: 16px;
}

.pesquisar__input-teclado{
    position: absolute;
    right: 16%;
    top: 30%;
}

.pesquisar__btn {
    background-color: var(--cinza-claro);
    border: 0px;
    border-radius: 0px 32px 32px 0px;
    padding: 8px;
    padding-right: 15px;
    border-left: none;
    cursor: pointer;
}

.cabecalho__audio {
    border: 0px;
    background-color: var(--branco);
}

.cabecalho__videos {
    background-image: url(../img/topbar/video_call.png);
    background-repeat: no-repeat;
    background-position: center;
    padding: 20px;
}

.cabecalho__apps {
    background-image: url(../img/topbar/apps.png);
    background-repeat: no-repeat;
    background-position: center;
    padding: 13px 30px 13px 13px;
}

.cabecalho__notificacoes {
    background-image: url(../img/topbar/notifications.png);
    background-repeat: no-repeat;
    background-position: center;
    padding: 13px 30px 13px 13px;
}

.cabecalho__avatar {
    background-image: url(../img/topbar/Avatar.png);
    background-repeat: no-repeat;
    background-position: center;
    padding: 13px 30px 13px 33px;
}

.cabecalho__switch {
    position: relative;
    display: inline-block;
    padding: 13px 30px 13px 13px;
    width: 60px;
    height: 34px;
  }
  
  .cabecalho__switch-input{
    opacity: 0;
    width: 0;
    height: 0;
  }
  
  .cabecalho__switch-slider {
    position: absolute;
    cursor: pointer;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-color: var(--cinza-claro);
    -webkit-transition: .4s;
    transition: .4s;
    border-radius: 34px;
  }
  
  .cabecalho__switch-slider:before {
    position: absolute;
    content: "";
    height: 26px;
    width: 26px;
    left: 4px;
    bottom: 4px;
    background-color: var(--branco);
    -webkit-transition: .4s;
    transition: .4s;
    border-radius: 50%;
  }
  
  .cabecalho__switch-input:checked + .cabecalho__switch-slider {
    background-color: var(--azul-destaque-light);
  }
  
  .cabecalho__switch-input:focus + .cabecalho__switch-slider {
    box-shadow: 0 0 1px var(--cinza-claro);
  }
  
  .cabecalho__switch-input:checked + .cabecalho__switch-slider:before {
    -webkit-transform: translateX(26px);
    -ms-transform: translateX(26px);
    transform: translateX(26px);
  }


/* MENU LATERAL */

.menu__container {
    font-size: 14px;
    background-color: var(--branco);
}

.icone__inicio::before {
    content: url(../img/sidebar/home.png);
}

.icone__explorar::before {
    content: url(../img/sidebar/explore.png);
}

.icone__shorts::before {
    content: url(../img/sidebar/airplay.png);
}

.icone__inscricoes::before {
    content: url(../img/sidebar/subscriptions.png);
}

.icone__biblioteca::before {
    content: url(../img/sidebar/video_library.png);
}

.icone__historico::before {
    content: url(../img/sidebar/history.png);
}

.icone__relogio::before {
    content: url(../img/sidebar/history_toggle_off.png);
}

.icone__like::before {
    content: url(../img/sidebar/thumb_up_alt.png);
}

.icone__alura::before {
    content: url(../img/sidebar/Avatar_Alura.png);
}

.icone__gaveta::before {
    content: url(../img/sidebar/Avatar_Gaveta.png);
}

.icone__ballerini::before {
    content: url(../img/sidebar/Avatar_Rafa.png);
}

.icone__iamarino::before {
    content: url(../img/sidebar/Avatar_Atila.png);
}

.icone__souto::before {
    content: url(../img/sidebar/Avatar_Souto.png);
}

.icone__nerd::before {
    content: url(../img/sidebar/Avatar_Jovem_Nerd.png);
}

.icone__deschamps::before {
    content: url(../img/sidebar/Avatar_Deschamps.png);
}

.icone__mostrar::before {
    content: url(../img/sidebar/keyboard_arrow_down.png);
}

.icone__videos::before {
    content: url(../img/sidebar/ondemand_video.png);
}

.icone__filmes::before {
    content: url(../img/sidebar/movie.png);
}

.icone__jogos::before {
    content: url(../img/sidebar/sports_esports.png);
}

/* SECAO SUPERIOR */

.superior__secao__container {
    height: 63px;
    color: var(--branco);
    font-size: 16px;
    background-color: var(--branco);
    padding: 0 20px;
    position: fixed;
    top: 80px;
    right: 0;
    left: 0;
    /* transition: transform 0.5s ease-in-out;
    transform: translateX(0); */
}

.superior__secao__container-wrapper{
    position: relative;
}

.superior__item {
    color: var(--cinza-escuro);
    font-size: 16px;
    background-color: var(--cinza-claro);
    border-radius: 20px;
    padding: 8px 20px;
    cursor: pointer;
    width: 200px;
}

.superior__item:hover {
    color: var(--branco);
    background-color: var(--azul-destaque-light);
    transition: .5s;
}

.superior__slider{
    position: absolute;
    right: 0%;
    width: 4%;
    height: 100%;
    background-color: var(--branco);
}

/* SEÇÃO VÍDEOS */

.videos__container {
    color: black;
    padding: 153px 20px 10px 20px;
}

iframe{
    border-radius: 10px;
    width: 100%;
    height: 62%;
}

.descricao-video .img-canal{
    border-radius: 100%;
    width: 40px;
    height: 40px;
}

.descricao-video .titulo-video {
    font-weight: 700;
    color: var(--cinza-escuro);
}

.descricao-video .titulo-canal {
    font-size: 14px;
    color: var(--cinza-escuro);
}  

::-webkit-scrollbar{
    width: 0px;
    height: 0px;
}

@media(min-width: 834px) {

    body {
        height: 100vh;
    }

    /* ESTILOS DO MENU LATERAL */

    .menu__container {
        font-size: 16px;
    }

    .menu__lista {
        padding-top: 15px;
    }

    .menu__lista li {
        width: 100%;
    }

    /* ESTILOS DA SECAO SUPERIOR */

    .superior__secao__container {
        border-top: var(--azul-medio) 1px solid;
        border-bottom: var(--azul-medio) 1px solid;
        width: auto;
        left: 82px;
    }

    /*ESTILOS SEÇÃO VÍDEOS */

    .videos__container {
        padding-left: 90px;
        padding-right: 17px;
    }

}

@media(min-width: 1440px) {

    /* SEÇÃO SUPERIOR */

    .superior__secao__container {
        left: 247px;
    }

    /* ESTILOS DO MENU LATERAL */

    .menu__lista {
        border-bottom: 1.5px solid var(--azul-medio);
    }

    /* ESTILOS VIDEOS */

    .videos__container {
        padding-right: 10px;
        padding-left: 248px;
    }

}