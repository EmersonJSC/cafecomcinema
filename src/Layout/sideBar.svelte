<script>
    import logo from '../assets/img/Logo.png'
</script>

<div class="sidebar is-flex is-flex-direction-column is-align-items-center">
    <div class="">
        <img class="logo px-4 py-4" src={logo} />
    </div>
    <div class="menu is-flex is-align-items-start py-2">
        <ul>
            <ui class="menu-item mx-4">Home</ui>
        </ul>
    </div>
</div>

<style>
    :global(body){
        background: url("https://img.freepik.com/vetores-gratis/cartaz-de-tempo-de-filme-de-cinema-horizontal-realista-com-carretel-de-badalo-de-bilhetes-de-lanches-de-oculos-3d-em-fundo-azul-com-ilustracao-vetorial-bokeh_1284-77013.jpg");
    }
    .sidebar{
        z-index: 1000;
        background-color: #e326ab;
        height: 100vh;
        width: 20vh;
        background-color: rgba(20, 20, 20, 0.4);
        backdrop-filter: blur(10px);
    }

    .logo{

    }
    .menu{
        /* background-color: aqua; */
        width: 100%;
        /* background-color: rgb(198 198 198 / 0.4); */
        background: linear-gradient(to right, rgb(99 0 0 / 0.4) 90%, rgb(255 255 255 / 0.1) 30%);
    }

    .menu-item{
        font-family: 'Roboto', sans-serif;
        font-weight: bold;
        color: #fff;
    }
</style>