<template>
    <!--<header style="height: 13.3vh;">-->
    <header style="height: 86px;">
        <nav class="navbar navbar-expand-lg bg-primary fixed-top" data-bs-theme="dark">
            <div class="container-fluid">
                <a class="navbar-brand" href="#">
                    <img src="/media/imagenes/logos/logo_0.png" id="logo" alt="Logo de Clinic Up" width="130vw" height="60vh" class="d-inline-block align-top" draggable="false">
                </a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarColor01" aria-controls="navbarColor01" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarColor01">
                    <ul class="navbar-nav me-auto">
                        <li class="nav-item">
                            <a class="nav-link" href="#inicio">
                                Inicio
                            </a>
                        </li>
                        <li class="nav-item dropdown">
                            <a class="nav-link dropdown-toggle" data-bs-toggle="dropdown" href="#servicios" role="button" aria-haspopup="true" aria-expanded="false">
                                Servicios
                            </a>
                            <div class="dropdown-menu">
                                <a class="dropdown-item" href="#">Amplio espectro residual</a>
                                <a class="dropdown-item" href="#">Amplio espectro residual mixta</a>
                                <a class="dropdown-item" href="#">F. residual mixta disuasivo murciélago</a>
                                <a class="dropdown-item" href="#">F. amplio espectro residual</a>
                                <a class="dropdown-item" href="#">F. cucarachas grandes</a>
                                <a class="dropdown-item" href="#">Tratamiento especial ratas</a>
                                <a class="dropdown-item" href="#">Cajas cebaderas con trampa de agua</a>
                                <a class="dropdown-item" href="#">Caja cebadera normal</a>
                                <a class="dropdown-item" href="#">F. amplio espectro residual garrapata y patacón</a>
                                <a class="dropdown-item" href="#">Pipetas para perro</a>
                                <a class="dropdown-item" href="#">F. termitas, carcoma, polilla, comejen</a>
                            </div>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link elementoCliqueable" data-bs-toggle="modal" data-bs-target="#modalNuestroEquipo">
                                Sobre Nosotros
                            </a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#galeria">
                                Galería
                            </a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#contacto">
                                Contacto
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
    </header>
    <section style="height: auto;">

        <div id="contenedorInicio" class="container-fluid pt-3 centrado" title="Inicio">
            <div>
                <div class="tituloSeccion">
                    <img class="w-100 d-block d-lg-none" src="/public/media/imagenes/titulos/fumigaciones_3.png" alt="titulo de la seccion centro especializado palabra centro" draggable="false">
                    <img class="w-75 d-none d-lg-block" src="/public/media/imagenes/titulos/fumigaciones_3.png" alt="titulo de la seccion centro especializado palabra centro" draggable="false">
                </div>
                <div class="tituloSeccion">
                    <img class="w-75 d-block d-lg-none" src="/public/media/imagenes/titulos/serviexpress_5.png" alt="titulo de la seccion centro especializado palabra especializado" draggable="false">
                    <img class="w-50 d-none d-lg-block" src="/public/media/imagenes/titulos/serviexpress_5.png" alt="titulo de la seccion centro especializado palabra especializado" draggable="false">
                </div>
                <div class="centrado mt-5 cartaAmarilla">
                    <p class="text-primary h3 text-center tipoDeFuenteDos">
                        Nos especializamos en proteger tu hogar, negocio, y seres queridos de cualquier tipo de plaga.
                    </p>
                </div>
            </div>
        </div>

        <div id="servicios" class="pt-2 bg-secondary" title="Servicios">
            <div class="tituloSeccion mb-2">
                <img class="w-50 d-block d-lg-none" src="/public/media/imagenes/titulos/servicios.png" alt="titulo de la seccion tratamientos capilares palabra tratamientos" draggable="false">
                <img class="w-50 d-none d-lg-block" src="/public/media/imagenes/titulos/servicios.png" alt="titulo de la seccion tratamientos capilares palabra tratamientos" draggable="false">
            </div>
            <div class="accordion accordion-flush" id="accordionFlushUno">
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonAmplioEspectroResidual" class="accordion-button collapsed text-primary bg-secondary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoUno" aria-expanded="false" aria-controls="colapsarFlujoUno">
                            Amplio espectro residual
                        </button>
                    </h2>
                    <div id="colapsarFlujoUno" class="accordion-collapse collapse text-dark bg-secondary" data-bs-parent="#accordionFlushUno">
                        <div class="accordion-body">
                            Es una Fumigación que incluye todos los insectos Rastreros y Voladores existentes y también roedores. Es Ideal para espacios donde queremos hacer prevenciones o correcciones y adicionalmente deseamos dejar una protección a largo plazo con una cobertura completa y general que quede matando animales a lo largo de al menos 6 meses.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonAmplioEspectroResidualMixta" class="accordion-button collapsed text-primary bg-secondary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoDos" aria-expanded="false" aria-controls="colapsarFlujoDos">
                            Amplio espectro residual mixta
                        </button>
                    </h2>
                    <div id="colapsarFlujoDos" class="accordion-collapse collapse text-dark bg-secondary" data-bs-parent="#accordionFlushUno">
                        <div class="accordion-body">
                            Fumigación de Amplio Espectro Residual Mixta se Realiza a Doble Cañón para Mayor Protección un Cañón a Propulsión y un Cañón de Humo. Incluye todos los insectos rastreros y voladores.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonFumigacionMixtaDisuasivoMurcielago" class="accordion-button collapsed text-primary bg-secondary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoTres" aria-expanded="false" aria-controls="colapsarFlujoTres">
                            F. residual mixta disuasivo murciélago
                        </button>
                    </h2>
                    <div id="colapsarFlujoTres" class="accordion-collapse collapse text-dark bg-secondary" data-bs-parent="#accordionFlushUno">
                        <div class="accordion-body">
                            Fumigación de Amplio Espectro Residual Mixta con Disuasivo para Murcielagos se Realiza a Doble Cañón para Mayor Protección un Cañón a Propulsión y un Cañón de Humo.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonFumigacionAmplioEspectroResidual" class="accordion-button collapsed text-primary bg-secondary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoCuatro" aria-expanded="false" aria-controls="colapsarFlujoCuatro">
                            F. amplio espectro residual
                        </button>
                    </h2>
                    <div id="colapsarFlujoCuatro" class="accordion-collapse collapse text-dark bg-secondary" data-bs-parent="#accordionFlushUno">
                        <div class="accordion-body">
                            Cobertura total de jates y cucarachas, todo tipo de insectos voladores y rastreros, es importante seguir una linea de procedimientos que se proponen para el antes de la fumigación que se deben seguir.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonFumigacionCurachasGrandes" class="accordion-button collapsed text-primary bg-secondary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoCinco" aria-expanded="false" aria-controls="colapsarFlujoCinco">
                            F. cucarachas grandes
                        </button>
                    </h2>
                    <div id="colapsarFlujoCinco" class="accordion-collapse collapse text-dark bg-secondary" data-bs-parent="#accordionFlushUno">
                        <div class="accordion-body">
                            Fumigación de amplia cobertura de cucarachas grandes. Hay que seguir un proceso del antes de la fumigación para una mejor efectividad.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonTratamientosEspecialRatas" class="accordion-button collapsed text-primary bg-secondary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoSeis" aria-expanded="false" aria-controls="colapsarFlujoSeis">
                            Tratamiento especial ratas
                        </button>
                    </h2>
                    <div id="colapsarFlujoSeis" class="accordion-collapse collapse text-dark bg-secondary" data-bs-parent="#accordionFlushUno">
                        <div class="accordion-body">
                            Se Realiza una supervisión de toda la casa / oficina / espacio para determinar el foco de infestación o madriguera. Areas a Tratar Sala, comedor, Pasillos, Baños, Cocina, Alacenas, 3 habitaciones, Closets en Habitaciones, Cielos Falso, Fachada, Patio Trasero, Patio Delantero, Bodeguita, Cuarto de Servidumbre, garaje o Parqueo.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonCajasCebaderasConTrampaDeAgua" class="accordion-button collapsed text-primary bg-secondary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoSiete" aria-expanded="false" aria-controls="colapsarFlujoSiete">
                            Cajas cebaderas con trampa de agua
                        </button>
                    </h2>
                    <div id="colapsarFlujoSiete" class="accordion-collapse collapse text-dark bg-secondary" data-bs-parent="#accordionFlushUno">
                        <div class="accordion-body">
                            Cajas Cebadera Retenedor de Agua Trampa de Impacto Segura Instalación Incluida en el servicio Cebo con Atrayente Especial.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonCajaCebaderaNormal" class="accordion-button collapsed text-primary bg-secondary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoOcho" aria-expanded="false" aria-controls="colapsarFlujoOcho">
                            Caja cebadera normal
                        </button>
                    </h2>
                    <div id="colapsarFlujoOcho" class="accordion-collapse collapse text-dark bg-secondary" data-bs-parent="#accordionFlushUno">
                        <div class="accordion-body">
                            Cajas Cebadera Trampa de Impacto Segura Cebo con Atrayente Especial. Fuertes, durables y confiables. Instalación y Abastecimiento Gratis.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonFumigacionAmplioEspectroResidualGarrapataYPatacon" class="accordion-button collapsed text-primary bg-secondary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoNueve" aria-expanded="false" aria-controls="colapsarFlujoNueve">
                            F. amplio espectro residual garrapata y patacón
                        </button>
                    </h2>
                    <div id="colapsarFlujoNueve" class="accordion-collapse collapse text-dark bg-secondary" data-bs-parent="#accordionFlushUno">
                        <div class="accordion-body">
                            Cobertura Total de Todos los insectos Rastreros y Voladores. En Algunos casos es necesario realizar procedimientos del antes de Fumigación en otros no, por favor consulte.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonPipetasParaPerro" class="accordion-button collapsed text-primary bg-secondary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoDiez" aria-expanded="false" aria-controls="colapsarFlujoDiez">
                            Pipetas para perro
                        </button>
                    </h2>
                    <div id="colapsarFlujoDiez" class="accordion-collapse collapse text-dark bg-secondary" data-bs-parent="#accordionFlushUno">
                        <div class="accordion-body">
                            Las Pipetas, matan todas las Pulgas, Garrapatas y Patacones que porta el animal en el momento y matan todos los huevecillos que anda la mascota a lo largo de semanas y meses eso constituye una gran protección. Se recomienda ponerle a su mascota luego de la fumigación contra pulgas y garrapatas.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonFumigacionTermitasCarcomaPolillaComejen" class="accordion-button collapsed text-primary bg-secondary" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoOnce" aria-expanded="false" aria-controls="colapsarFlujoOnce">
                            F. termitas, carcoma, polilla, comejen
                        </button>
                    </h2>
                    <div id="colapsarFlujoOnce" class="accordion-collapse collapse text-dark bg-secondary" data-bs-parent="#accordionFlushUno">
                        <div class="accordion-body">
                            Se aplica a: Puertas, Contra Marcos de puertas, Ventanas, Contra Marcos Ventanas, Cómodas de madera, Mesas De Noche, Techos, Vigas, Mesas, Sillas, Divisiones, Roperos, Closets, Muebles, De Cocina, Alacenas, Chineros, Gaveteros, Muebles, de Madera, Cielo Falso Toda la Casa, Archivadores, Libreros, y Todo lo que Este Hecho En Madera
                        </div>
                    </div>
                </div>
            </div>
        </div>

    </section>
    <footer class="bg-primary centrado" style="height:10vh;" title="© 2024 Fumigaciones Serviexpress Todos los derechos reservados.">
        <span class="text-secondary text-center tipoDeFuenteDos">
            © 2024 Fumigaciones Serviexpress Todos los derechos reservados.
        </span>
    </footer>
</template>

<script>
    export default {
        
    }
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Rammetto+One&display=swap');

    .navbar-toggler
    {
        color: rgba(255, 0, 0, 0.266);
        border:solid rgb(54, 54, 54);
        line-height: 1;
    }
    [data-bs-theme=dark] .navbar-toggler-icon 
    {
        --bs-navbar-toggler-icon-bg: url(/media/imagenes/iconos/icono_toggler_navbar.svg);
    }
    .nav-link
    {
        color: rgba(0, 0, 0);
    }
    .nav-link:hover, .nav-link:focus {
        color:  rgba(255, 0, 0);
    }
    .navbar-nav .nav-link.active, .navbar-nav .nav-link.show
    {
        color: rgba(255, 0, 0);
    }
    #contenedorInicio
    {
        background-image: url('/media/imagenes/gifs/fumigacion_0.gif');
        background-size: cover;
        background-position: center;

        height: 86.6vh;
        /*height:563px;*/
    }
    .tituloSeccion
    {
        display:flex;
        justify-content: center;
    }
    .centrado
    {
        display:flex;
        align-items: center;
        justify-content: center;
    }
    .tipoDeFuenteDos
    {
        font-family: "Rammetto One", sans-serif;
    }
    .cartaAmarilla
    {
        /*background-color: rgba(242, 255, 0, 0.518);*/
        background-color:   rgba(255, 0, 0, 0.518);
    }
    .elementoCliqueable
    {
        cursor: pointer;
    }
</style>