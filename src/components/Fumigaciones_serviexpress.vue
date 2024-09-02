<template>
    <header style="height: 86px;">
        <nav class="navbar navbar-expand-lg bg-primary fixed-top" data-bs-theme="dark">
            <div class="container-fluid">
                <a class="navbar-brand" href="#">
                    <img src="/media/imagenes/logos/logo_0.png" id="Logo de Fumigaciones Serviexpress" alt="Logo de Clinic Up" width="130vw" height="60vh" class="d-inline-block align-top" draggable="false">
                </a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarColor01" aria-controls="navbarColor01" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarColor01">
                    <ul class="navbar-nav me-auto">
                        <li class="nav-item">
                            <a class="nav-link fw-bold" href="#inicio">
                                Inicio
                            </a>
                        </li>
                        <li class="nav-item dropdown">
                            <a class="nav-link dropdown-toggle fw-bold" data-bs-toggle="dropdown" href="#servicios" role="button" aria-haspopup="true" aria-expanded="false">
                                Servicios
                            </a>
                            <div class="dropdown-menu" style="height: 29vh; overflow-y: scroll">
                                <a class="dropdown-item fw-bold" href="#" @click="abrirServicio('AmplioEspectroResidual')">
                                    <small>
                                        AMPLIO ESPECTRO RESIDUAL
                                    </small>
                                </a>
                                <a class="dropdown-item fw-bold" href="#" @click="abrirServicio('AmplioEspectroResidualMixta')">
                                    <small>
                                        AMPLIO ESPECTRO RESIDUAL MIXTA
                                    </small>
                                </a>
                                <a class="dropdown-item fw-bold" href="#" @click="abrirServicio('FumigacionResidualMixtaDisuasivoMurcielago')">
                                    <small>
                                        MIXTA DISUASIVO MURCIÉLAGO
                                    </small>
                                </a>
                                <a class="dropdown-item fw-bold" href="#" @click="abrirServicio('FumigacionAmplioEspectroResidualTipoJatesYCucarachas')">
                                    <small style="white-space: nowrap; overflow-x: auto;">
                                        JATES Y CUCARACHAS
                                    </small>
                                </a>
                                <a class="dropdown-item fw-bold" href="#" @click="abrirServicio('FumigacionAmplioEspectroResidualTipoJatesYCucarachasConTratamientoRatas')">
                                    <small style="white-space: nowrap; overflow-x: auto;">
                                        JATES Y CUCARACHAS (RATAS)
                                    </small>
                                </a>
                                <a class="dropdown-item fw-bold" href="#" @click="abrirServicio('FumigacionCucarachasGrandes')">
                                    <small>
                                        CUCARACHAS GRANDES
                                    </small>
                                </a>
                                <a class="dropdown-item fw-bold" href="#" @click="abrirServicio('TratamientoEspecialRatas')">
                                    <small>
                                        TRATAMIENTO ESPECIAL RATAS
                                    </small>
                                </a>
                                <a class="dropdown-item fw-bold" href="#" @click="abrirServicio('FumigacionAmplioEspectroResidualTipoEspecialRatonesYRatas')">
                                    <small>
                                        RESIDUAL (RATONES Y RATAS)
                                    </small>
                                </a>
                                <a class="dropdown-item fw-bold" href="#" @click="abrirServicio('FumigacionAmplioEspectroResidualTipoPulgasYRatas')">
                                    <small>
                                        RESIDUAL (PULGAS Y RATAS)
                                    </small>
                                </a>
                                <a class="dropdown-item fw-bold" href="#" @click="abrirServicio('CajasCebaderasConTrampaDeAgua')">
                                    <small>
                                        CAJA CEBADERA (TRAMPA DE AGUA)
                                    </small>
                                </a>
                                <a class="dropdown-item fw-bold" href="#" @click="abrirServicio('CajaCebaderaNormal')">
                                    <small>
                                        CAJA CEBADERA NORMAL
                                    </small>
                                </a>
                                <a class="dropdown-item fw-bold" href="#" @click="abrirServicio('FumigacionAmplioEspectroResidualGarrapataYPatacon')">
                                    <small>
                                        RESIDUAL GARRAPATA Y PATACÓN
                                    </small>
                                </a>
                                <a class="dropdown-item fw-bold" href="#" @click="abrirServicio('PipetasParaPerro')">
                                    <small>
                                        PIPETAS PARA PERRO
                                    </small>
                                </a>
                                <a class="dropdown-item fw-bold" href="#" @click="abrirServicio('FumigacionTermitasCarcomaPolillaComejen')">
                                    <small>
                                        TERMITAS, CARCOMA, COMEJÉN
                                    </small>
                                </a>
                            </div>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link elementoCliqueable fw-bold" data-bs-toggle="modal" data-bs-target="#modalNuestroEquipo">
                                Sobre Nosotros
                            </a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link fw-bold" href="#galeria">
                                Galería
                            </a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link fw-bold" href="#contacto">
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
                    <img class="w-100 d-block d-lg-none" src="/public/media/imagenes/titulos/fumigaciones_3.png" alt="titulo de la seccion inicio, palabra fumigaciones" draggable="false">
                    <img class="w-75 d-none d-lg-block" src="/public/media/imagenes/titulos/fumigaciones_3.png" alt="titulo de la seccion inicio, palabra fumigaciones" draggable="false">
                </div>
                <div class="tituloSeccion">
                    <img class="w-100 d-block d-lg-none" src="/public/media/imagenes/titulos/serviexpress_5.png" alt="titulo de la seccion inicio, palabra serviexpress" draggable="false">
                    <img class="w-75 d-none d-lg-block" src="/public/media/imagenes/titulos/serviexpress_5.png" alt="titulo de la seccion inicio, palabra serviexpress" draggable="false">
                </div>
                <div class="centrado mt-5">
                    <p class="text-primary h3 text-center tipoDeFuenteDos cartaAmarilla">
                        Entorno sano, mente sana.
                    </p>
                </div>
            </div>
        </div>

        <div id="servicios" class="pt-2 bg-secondary" title="Servicios">
            <div class="tituloSeccion mb-2">
                <img class="w-50 d-block d-lg-none" src="/public/media/imagenes/titulos/servicios.png" alt="titulo de la seccion servicios" draggable="false">
                <img class="w-50 d-none d-lg-block" src="/public/media/imagenes/titulos/servicios.png" alt="titulo de la seccion servicios" draggable="false">
            </div>
            <div class="accordion accordion-flush" id="accordionFlushUno">
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonAmplioEspectroResidual" class="accordion-button collapsed text-primary bg-secondary fw-bold" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoUno" aria-expanded="false" aria-controls="colapsarFlujoUno">
                            AMPLIO ESPECTRO RESIDUAL
                        </button>
                    </h2>
                    <div id="colapsarFlujoUno" class="accordion-collapse collapse text-secondary bg-primary fw-bold" data-bs-parent="#accordionFlushUno">
                        <div class="container-fluid">
                            <div class="row">
                                <div class="col-sm-12 pt-2">
                                    <div class="centrado">
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_rastreros.png" alt="Imagen de prohibido insectos rastreros" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_voladores.png" alt="Imagen de prohibido insectos voladores" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_rastreros.png" alt="Imagen de prohibido insectos rastreros" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_voladores.png" alt="Imagen de prohibido insectos voladores" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/roedores.png" alt="Imagen de prohibido roedoeres" draggable="false">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-sm-12 d-block d-md-none pt-2">
                                    <div class="centrado">
                                        <div class="w-50 centrado">
                                            <img class="w-75" src="/public/media/imagenes/plagas/roedores.png" alt="Imagen de prohibido roedores" draggable="false">
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="accordion-body text-center">
                            Es una Fumigación que incluye todos los insectos Rastreros y Voladores existentes y también roedores. Es Ideal para espacios donde queremos hacer prevenciones o correcciones y adicionalmente deseamos dejar una protección a largo plazo con una cobertura completa y general que quede matando animales a lo largo de al menos 6 meses.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonAmplioEspectroResidualMixta" class="accordion-button collapsed text-primary bg-secondary fw-bold" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoDos" aria-expanded="false" aria-controls="colapsarFlujoDos">
                            AMPLIO ESPECTRO RESIDUAL MIXTA
                        </button>
                    </h2>
                    <div id="colapsarFlujoDos" class="accordion-collapse collapse text-secondary bg-primary fw-bold" data-bs-parent="#accordionFlushUno">
                        <div class="container-fluid">
                            <div class="row">
                                <div class="col-sm-12 pt-2">
                                    <div class="centrado">
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_rastreros.png" alt="Imagen de prohibido insectos rastreros" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_voladores.png" alt="Imagen de prohibido insectos voladores" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_rastreros.png" alt="Imagen de prohibido insectos rastreros" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_voladores.png" alt="Imagen de prohibido insectos voladores" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/roedores.png" alt="Imagen de prohibido roedores" draggable="false">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-sm-12 d-block d-md-none pt-2">
                                    <div class="centrado">
                                        <div class="w-50 centrado">
                                            <img class="w-75 d-block d-lg-none" src="/public/media/imagenes/plagas/roedores.png" alt="Imagen de prohibido roedores" draggable="false">
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="accordion-body text-center">
                            Fumigación de Amplio Espectro Residual Mixta se Realiza a Doble Cañón para Mayor Protección un Cañón a Propulsión y un Cañón de Humo. Incluye todos los insectos rastreros y voladores.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonFumigacionResidualMixtaDisuasivoMurcielago" class="accordion-button collapsed text-primary bg-secondary fw-bold" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoTres" aria-expanded="false" aria-controls="colapsarFlujoTres">
                            F. RESIDUAL MIXTA DISUASIVO MURCIÉLAGO
                        </button>
                    </h2>
                    <div id="colapsarFlujoTres" class="accordion-collapse collapse text-secondary bg-primary fw-bold" data-bs-parent="#accordionFlushUno">
                        <div class="container-fluid">
                            <div class="row">
                                <div class="col-sm-12 pt-2">
                                    <div class="centrado">
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/murcielagos.png" alt="Silueta de un murcielago dentro de un circulo rojo" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_rastreros.png" alt="Imagen de prohibido insectos rastreros" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/murcielagos.png" alt="Silueta de un murcielago dentro de un circulo rojo" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_rastreros.png" alt="Imagen de prohibido insectos rastreros" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_voladores.png" alt="Imagen de prohibido insectos voladores" draggable="false">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-sm-12 d-block d-md-none pt-2">
                                    <div class="centrado">
                                        <div class="w-50 centrado">
                                            <img class="w-75 d-block d-lg-none" src="/public/media/imagenes/plagas/insectos_voladores.png" alt="Imagen de prohibido insectos voladores" draggable="false">
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="accordion-body text-center">
                            Fumigación de Amplio Espectro Residual Mixta con Disuasivo para Murcielagos se Realiza a Doble Cañón para Mayor Protección un Cañón a Propulsión y un Cañón de Humo.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonFumigacionAmplioEspectroResidualTipoJatesYCucarachas" class="accordion-button collapsed text-primary bg-secondary fw-bold" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoCuatro" aria-expanded="false" aria-controls="colapsarFlujoCuatro">
                            F. AMPLIO ESPECTRO RESIDUAL (JATES Y CUCARACHAS)
                        </button>
                    </h2>
                    <div id="colapsarFlujoCuatro" class="accordion-collapse collapse text-secondary bg-primary fw-bold" data-bs-parent="#accordionFlushUno">
                        <div class="container-fluid">
                            <div class="row">
                                <div class="col-sm-12 pt-2">
                                    <div class="centrado">
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/jates.png" alt="Imagen de prohibido jates" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/cucarachas.png" alt="Imagen de prohibido cucarachas" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/jates.png" alt="Imagen de prohibido jates" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/cucarachas.png" alt="Imagen de prohibido cucarachas" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_voladores.png" alt="Imagen de prohibido insectos voladores" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_rastreros.png" alt="Imagen de prohibido insectos rastreros" draggable="false">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-sm-12 d-block d-md-none pt-2">
                                    <div class="centrado">
                                        <div class="w-50">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_voladores.png" alt="Imagen de prohibido insectos voladores" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-50">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_rastreros.png" alt="Imagen de prohibido insectos rastreros" draggable="false">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="accordion-body text-center">
                            Cobertura total de jates y cucarachas, todo tipo de insectos voladores y rastreros, es importante seguir una linea de procedimientos que se proponen para el antes de la fumigación que se deben seguir.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonFumigacionAmplioEspectroResidualTipoJatesYCucarachasConTratamientoRatas" class="accordion-button collapsed text-primary bg-secondary fw-bold" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoCinco" aria-expanded="false" aria-controls="colapsarFlujoCinco">
                            F. AMPLIO ESPECTRO RESIDUAL (JATES Y CUCARACHAS ADEMAS INCLUYE TRATAMIENTO ESPECIAL DE RATAS)
                        </button>
                    </h2>
                    <div id="colapsarFlujoCinco" class="accordion-collapse collapse text-secondary bg-primary fw-bold" data-bs-parent="#accordionFlushUno">
                        <div class="container-fluid">
                            <div class="row">
                                <div class="col-sm-12 pt-2">
                                    <div class="centrado">
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/jates.png" alt="Imagen de prohibido jates" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/cucarachas.png" alt="Imagen de prohibido cucarachas" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/jates.png" alt="Imagen de prohibido jates" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/cucarachas.png" alt="Imagen de prohibido cucarachas" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_voladores.png" alt="Imagen de prohibido insectos voladores" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_rastreros.png" alt="Imagen de prohibido insectos rastreros" draggable="false">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-sm-12 d-block d-md-none pt-2">
                                    <div class="centrado">
                                        <div class="w-50">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_voladores.png" alt="Imagen de prohibido insectos voladores" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-50">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_rastreros.png" alt="Imagen de prohibido insectos rastreros" draggable="false">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-sm-12 d-block d-md-none pt-2">
                                    <div class="centrado">
                                        <div class="w-50 centrado">
                                            <img class="w-75 d-block d-lg-none" src="/public/media/imagenes/plagas/roedores.png" alt="Imagen de prohibido roedores" draggable="false">
                                        </div>
                                    </div>
                                </div>
                                <div class="col-sm-12 pt-2">
                                    <div class="centrado">
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/roedores.png" alt="Imagen de prohibido roedores" draggable="false">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="accordion-body text-center">
                            Fumigación de Amplio Espectro Residual Tipo: Jates, Zancudos, Chinches y Alacranes con Tratamiento Especial de Ratas Y Ratones.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonFumigacionCucarachasGrandes" class="accordion-button collapsed text-primary bg-secondary fw-bold" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoSeis" aria-expanded="false" aria-controls="colapsarFlujoSeis">
                            F. CUCARACHAS GRANDES
                        </button>
                    </h2>
                    <div id="colapsarFlujoSeis" class="accordion-collapse collapse text-secondary bg-primary fw-bold" data-bs-parent="#accordionFlushUno">
                        <div class="container-fluid">
                            <div class="row">
                                <div class="col-sm-12 pt-2">
                                    <div class="centrado">
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/cucarachas.png" alt="Imagen de prohibido cucarachas" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/cucarachas.png" alt="Imagen de prohibido cucarachas" draggable="false">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="accordion-body text-center">
                            Fumigación de amplia cobertura de cucarachas grandes. Hay que seguir un proceso del antes de la fumigación para una mejor efectividad.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonTratamientoEspecialRatas" class="accordion-button collapsed text-primary bg-secondary fw-bold" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoSiete" aria-expanded="false" aria-controls="colapsarFlujoSiete">
                            TRATAMIENTO ESPECIAL RATAS
                        </button>
                    </h2>
                    <div id="colapsarFlujoSiete" class="accordion-collapse collapse text-secondary bg-primary fw-bold" data-bs-parent="#accordionFlushUno">
                        <div class="container-fluid">
                            <div class="row">
                                <div class="col-sm-12 pt-2">
                                    <div class="centrado">
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/roedores.png" alt="Imagen de prohibido roedores" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/roedores.png" alt="Imagen de prohibido roedores" draggable="false">
                                            </div>
                                        </div>
                                    </div>
                                </div>  
                            </div>
                        </div>
                        <div class="accordion-body text-center">
                            Se Realiza una supervisión de toda la casa / oficina / espacio para determinar el foco de infestación o madriguera. Areas a Tratar Sala, comedor, Pasillos, Baños, Cocina, Alacenas, 3 habitaciones, Closets en Habitaciones, Cielos Falso, Fachada, Patio Trasero, Patio Delantero, Bodeguita, Cuarto de Servidumbre, garaje o Parqueo.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonFumigacionAmplioEspectroResidualTipoEspecialRatonesYRatas" class="accordion-button collapsed text-primary bg-secondary fw-bold" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoOcho" aria-expanded="false" aria-controls="colapsarFlujoOcho">
                            F. AMPLIO ESPECTRO RESIDUAL (ESPECIAL RATAS Y RATONES)
                        </button>
                    </h2>
                    <div id="colapsarFlujoOcho" class="accordion-collapse collapse text-secondary bg-primary fw-bold" data-bs-parent="#accordionFlushUno">
                        <div class="container-fluid">
                            <div class="row">
                                <div class="col-sm-12 pt-2">
                                    <div class="centrado">
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_rastreros.png" alt="Imagen de prohibido insectos rastreros" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_voladores.png" alt="Imagen de prohibido insectos voladores" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_rastreros.png" alt="Imagen de prohibido insectos rastreros" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_voladores.png" alt="Imagen de prohibido insectos voladores" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/roedores.png" alt="Imagen de prohibido roedores" draggable="false">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-sm-12 d-block d-md-none pt-2">
                                    <div class="centrado">
                                        <div class="w-50 centrado">
                                            <img class="w-75" src="/public/media/imagenes/plagas/roedores.png" alt="Imagen de prohibido roedores" draggable="false">
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="accordion-body text-center">
                            Fumigación de Amplio Espectro Residual con cobertura para todos insectos que existen rastreros y voladores y 4 Rondas de Tratamiento Especial de Ratas y Ratones. Es necesario realizar procesos del antes de la fumigación.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonFumigacionAmplioEspectroResidualTipoPulgasYRatas" class="accordion-button collapsed text-primary bg-secondary fw-bold" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoNueve" aria-expanded="false" aria-controls="colapsarFlujoNueve">
                            F. AMPLIO ESPECTRO RESIDUAL (PULGAS Y RATAS)
                        </button>
                    </h2>
                    <div id="colapsarFlujoNueve" class="accordion-collapse collapse text-secondary bg-primary fw-bold" data-bs-parent="#accordionFlushUno">
                        <div class="container-fluid">
                            <div class="row">
                                <div class="col-sm-12 pt-2">
                                    <div class="centrado">
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/pulgas.png" alt="Imagen de prohibido pulgas" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_rastreros.png" alt="Imagen de prohibido insectos rastreros" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/pulgas.png" alt="Imagen de prohibido pulgas" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_rastreros.png" alt="Imagen de prohibido insectos rastreros" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_voladores.png" alt="Imagen de prohibido insectos voladores" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/roedores.png" alt="Imagen de prohibido roedores" draggable="false">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-sm-12 d-block d-md-none pt-2">
                                    <div class="centrado">
                                        <div class="w-50">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_voladores.png" alt="Imagen de prohibido insectos voladores" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-50">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/roedores.png" alt="Imagen de prohibido roedores" draggable="false">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="accordion-body text-center">
                            Fumigación de Amplio Espectro Residual Tipo Pulgas con cobertura para todos los insectos rastreros y volares que existen Y 4 Rondas de Tratamiento Especial Ratas y Ratones. Cobertura Completa
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonCajasCebaderasConTrampaDeAgua" class="accordion-button collapsed text-primary bg-secondary fw-bold" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoDiez" aria-expanded="false" aria-controls="colapsarFlujoDiez">
                            CAJAS CEBADERAS CON TRAMPA DE AGUA
                        </button>
                    </h2>
                    <div id="colapsarFlujoDiez" class="accordion-collapse collapse text-secondary bg-primary fw-bold" data-bs-parent="#accordionFlushUno">
                        <div class="container-fluid">
                            <div class="row">
                                <div class="col-sm-12 pt-2">
                                    <div class="centrado">
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/roedores.png" alt="Imagen de prohibido roedores" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/roedores.png" alt="Imagen de prohibido roedores" draggable="false">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="accordion-body text-center">
                            Cajas Cebadera Retenedor de Agua Trampa de Impacto Segura Instalación Incluida en el servicio Cebo con Atrayente Especial.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonCajaCebaderaNormal" class="accordion-button collapsed text-primary bg-secondary fw-bold" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoOnce" aria-expanded="false" aria-controls="colapsarFlujoOnce">
                            CAJA CEBADERA NORMAL
                        </button>
                    </h2>
                    <div id="colapsarFlujoOnce" class="accordion-collapse collapse text-secondary bg-primary fw-bold" data-bs-parent="#accordionFlushUno">
                        <div class="container-fluid">
                            <div class="row">
                                <div class="col-sm-12 pt-2">
                                    <div class="centrado">
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/roedores.png" alt="Imagen de prohibido roedores" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/roedores.png" alt="Imagen de prohibido roedores" draggable="false">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="accordion-body text-center">
                            Cajas Cebadera Trampa de Impacto Segura Cebo con Atrayente Especial. Fuertes, durables y confiables. Instalación y Abastecimiento Gratis.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonFumigacionAmplioEspectroResidualGarrapataYPatacon" class="accordion-button collapsed text-primary bg-secondary fw-bold" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoDoce" aria-expanded="false" aria-controls="colapsarFlujoDoce">
                            F. AMPLIO ESPECTRO RESIDUAL GARRAPATA Y PATACÓN
                        </button>
                    </h2>
                    <div id="colapsarFlujoDoce" class="accordion-collapse collapse text-secondary bg-primary fw-bold" data-bs-parent="#accordionFlushUno">
                        <div class="container-fluid">
                            <div class="row">
                                <div class="col-sm-12 pt-2">
                                    <div class="centrado">
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_rastreros.png" alt="Imagen de prohibido insectos rastreros" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_voladores.png" alt="Imagen de prohibido insectos voladores" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_rastreros.png" alt="Imagen de prohibido insectos rastreros" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/insectos_voladores.png" alt="Imagen de prohibido insectos voladores" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/garrapatas.png" alt="Imagen de prohibido garrapatas" draggable="false">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-sm-12 d-block d-md-none pt-2">
                                    <div class="centrado">
                                        <div class="w-50 centrado">
                                            <img class="w-75" src="/public/media/imagenes/plagas/garrapatas.png" alt="Imagen de prohibido garrapatas" draggable="false">
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="accordion-body text-center">
                            Cobertura Total de Todos los insectos Rastreros y Voladores. En Algunos casos es necesario realizar procedimientos del antes de Fumigación en otros no, por favor consulte.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonPipetasParaPerro" class="accordion-button collapsed text-primary bg-secondary fw-bold" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoTrece" aria-expanded="false" aria-controls="colapsarFlujoTrece">
                            PIPETAS PARA PERRO
                        </button>
                    </h2>
                    <div id="colapsarFlujoTrece" class="accordion-collapse collapse text-secondary bg-primary fw-bold" data-bs-parent="#accordionFlushUno">
                        <div class="container-fluid">
                            <div class="row">
                                <div class="col-sm-12 pt-2">
                                    <div class="centrado">
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/pulgas.png" alt="Imagen de prohibido pulgas" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/garrapatas.png" alt="Imagen de prohibido garrapatas" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/pulgas.png" alt="Imagen de prohibido pulgas" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/garrapatas.png" alt="Imagen de prohibido garrapatas" draggable="false">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="accordion-body text-center">
                            Las Pipetas, matan todas las Pulgas, Garrapatas y Patacones que porta el animal en el momento y matan todos los huevecillos que anda la mascota a lo largo de semanas y meses eso constituye una gran protección. Se recomienda ponerle a su mascota luego de la fumigación contra pulgas y garrapatas.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button id="botonFumigacionTermitasCarcomaPolillaComejen" class="accordion-button collapsed text-primary bg-secondary fw-bold" type="button" data-bs-toggle="collapse" data-bs-target="#colapsarFlujoCatorce" aria-expanded="false" aria-controls="colapsarFlujoCatorce">
                            F. TERMITAS, CARCOMA, POLILLA, COMEJÉN
                        </button>
                    </h2>
                    <div id="colapsarFlujoCatorce" class="accordion-collapse collapse text-secondary bg-primary fw-bold" data-bs-parent="#accordionFlushUno">
                        <div class="container-fluid">
                            <div class="row">
                                <div class="col-sm-12 pt-2">
                                    <div class="centrado">
                                        <div class="w-50 d-block d-md-none">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/termitas.png" alt="Imagen de prohibido termitas" draggable="false">
                                            </div>
                                        </div>
                                        <div class="w-25 d-none d-md-block">
                                            <div class="centrado">
                                                <img class="w-75" src="/public/media/imagenes/plagas/termitas.png" alt="Imagen de prohibido termitas" draggable="false">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="accordion-body text-center">
                            Se aplica a: Puertas, Contra Marcos de puertas, Ventanas, Contra Marcos Ventanas, Cómodas de madera, Mesas De Noche, Techos, Vigas, Mesas, Sillas, Divisiones, Roperos, Closets, Muebles, De Cocina, Alacenas, Chineros, Gaveteros, Muebles, de Madera, Cielo Falso Toda la Casa, Archivadores, Libreros, y Todo lo que Este Hecho En Madera
                        </div>
                    </div>
                </div>
            </div>
        </div>

    </section>
    <footer class="bg-primary centrado" style="height:10vh;" title="© Fumigaciones Serviexpress Todos los derechos reservados.">
        <span class="text-secondary text-center tipoDeFuenteDos">
            © {{anioActual}} Fumigaciones Serviexpress Todos los derechos reservados.
        </span>
    </footer>
</template>

<script>
    export default {
        data(){
            return {
                fechaActual:"",
                anioActual:"",
            }
        },
        methods:{
            obtenerAnioActual() {
                this.fechaActual = new Date(); // Obtiene la fecha actual
                this.anioActual = this.fechaActual.getFullYear(); // Extrae el año de la fecha actual
            },
            abrirServicio(servicio){
                let boton="boton"+servicio;
                let botonServicio=document.getElementById(boton);                
                botonServicio.click();
            }
        },
        components: {

        },
        props: {

        },
        created() {
            this.obtenerAnioActual();
        },
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
        --bs-navbar-toggler-icon-bg: url('/media/imagenes/iconos/icono_toggler_navbar.svg');
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
    .accordion
    {
        --bs-accordion-btn-icon: url('/media/imagenes/iconos/flecha_hacia_abajo_acordeon.svg');
    }
    .enUnaSolaLinea
    {
        white-space: nowrap;            /* Mantiene el texto en una sola línea */
        overflow-x: auto;               /* Habilita la barra de desplazamiento horizontal si es necesario */
        /*width: 300vw;*/               /* Ajusta el ancho del contenedor */
        /*border: 1vw solid #ccc;*/     /* Opcional: Añade un borde para ver el área del contenedor */
        /*padding: 5vw;*/               /* Opcional: Añade un poco de padding */
    }
    .dropdown-menu
    {
        --bs-dropdown-bg: rgba(255, 0, 0);
        --bs-dropdown-link-hover-bg: rgb(242, 255, 0);
        border: 2px solid rgba(0, 0, 0);
        --bs-dropdown-link-hover-color: rgba(255, 0, 0);
    }
    .dropdown-item
    {
        color:rgb(242, 255, 0);
    }
    .contenedorFlexible
    {
        display:flex;
    }
    .centrado
    {
        display:flex;
        align-items: center;
        justify-content: center;
    }
</style>