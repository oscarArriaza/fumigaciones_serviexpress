<template>
    <div class="modal fade" id="modalProcesoAntesDeLaFumigacion" data-bs-backdrop="static" data-bs-keyboard="false" tabindex="-1" aria-labelledby="modalProcesoAntesDeLaFumigacionLabel" aria-hidden="true">
        <Proceso_antes_de_la_fumigacion></Proceso_antes_de_la_fumigacion>
    </div>
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
                                Sobre nosotros
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
                            Fumigación de Amplio Espectro Residual con cobertura para todos insectos que existen rastreros y voladores y 4 Rondas de Tratamiento Especial de Ratas y Ratones. Es necesario realizar este proceso 🡺<a class="elementoCliqueable bg-secondary text-primary elementoSinSubrayado" title="Proceso antes de la fumigacion." data-bs-toggle="modal" data-bs-target="#modalProcesoAntesDeLaFumigacion">proceso antes de la fumigación</a>🢀
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
                            Cobertura Total de Todos los insectos Rastreros y Voladores. En Algunos casos es necesario realizar este proceso 🡺<a class="elementoCliqueable bg-secondary text-primary elementoSinSubrayado" title="Proceso antes de la fumigacion." data-bs-toggle="modal" data-bs-target="#modalProcesoAntesDeLaFumigacion">proceso antes de la fumigación</a>🢀 en otros no, por favor consulte.
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
                        <div class="bg-secondary" style="height: 9vh;"></div>
                    </div>
                </div>
            </div>
        </div>

        <div id="sobreNosotros" class="pt-2 pb-3 bg-primary" title="Sobre nosotros">
            <div class="tituloSeccion mb-2">
                <img class="w-75 d-block d-lg-none" src="/public/media/imagenes/titulos/sobre_nosotros.png" alt="titulo de la seccion sobre nosotros" draggable="false">
                <img class="w-50 d-none d-lg-block" src="/public/media/imagenes/titulos/sobre_nosotros.png" alt="titulo de la seccion sobre nosotros" draggable="false">
            </div>
            <div class="container-fluid">
                <div class="row">
                    <div class="col-sm-12 col-md-6 centrado">
                        <img class="w-100 d-block d-lg-none" src="/public/media/imagenes/equipo_de_fumigaciones_serviexpress/0.jpg" alt="Equipo de fumigaciones serviexpress" title="Equipo de fumigaciones serviexpress" draggable="false">
                        <img class="w-75 d-none d-lg-block" src="/public/media/imagenes/equipo_de_fumigaciones_serviexpress/0.jpg" alt="Equipo de fumigaciones serviexpress" title="Equipo de fumigaciones serviexpress" draggable="false">
                    </div>
                    <div class="col-sm-12 col-md-6 centrado">
                        <span class="text-secondary fw-bold text-center">
                            Fumigaciones ServiExpress es una Empresa dedicada a las Fumigaciones para Exterminio de Plagas Rastreras, Voladores, Tratamientos Especiales de Roedores y Sanitización de Espacios.
                            <br>
                            <br>
                            Brindamos Atención Online y el Servicio es a Domicilio, es rápido, confiable, seguro y garantizado.
                            <br>
                            <br>
                            Somos una Empresa capaz de Realizarle una Revisión y Diagnóstico de su Espacio Gratis, Sin costo y Sin compromiso, todo con el objetivo de brindarle un servicio de calidad.
                        </span>
                    </div>
                </div>
            </div>
        </div>

        <div class="pt-1 bg-secondary" title="Galería">
            <div class="tituloSeccion mb-2">
                <img class="w-50 d-block d-lg-none" src="/public/media/imagenes/titulos/galeria.png" alt="titulo de la seccion galería" draggable="false">
                <img class="w-25 d-none d-lg-block" src="/public/media/imagenes/titulos/galeria.png" alt="titulo de la seccion galería" draggable="false">
            </div>
            <div id="carrusel" class="carousel slide">
                <div class="carousel-indicators">
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="1" aria-label="Slide 2"></button>
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="2" aria-label="Slide 3"></button>
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="3" aria-label="Slide 4"></button>
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="4" aria-label="Slide 5"></button>
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="5" aria-label="Slide 6"></button>
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="6" aria-label="Slide 7"></button>
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="7" aria-label="Slide 8"></button>
                </div>
                <div class="carousel-inner">
                    <div class="carousel-item active">
                        <img src="/public/media/imagenes/fumigaciones/01.jpg" class="d-block w-100" alt="..." dragable="false">
                        <div class="carousel-caption d-none d-md-block">
                            <h5></h5>
                            <p></p>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <img src="/public/media/imagenes/fumigaciones/02.jpg" class="d-block w-100" alt="..." draggable="false">
                        <div class="carousel-caption d-none d-md-block">
                            <h5></h5>
                            <p></p>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <img src="/public/media/imagenes/fumigaciones/03.jpg" class="d-block w-100" alt="..." draggable="false">
                        <div class="carousel-caption d-none d-md-block">
                            <h5></h5>
                            <p></p>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <img src="/public/media/imagenes/fumigaciones/04.jpg" class="d-block w-100" alt="..." draggable="false">
                        <div class="carousel-caption d-none d-md-block">
                            <h5></h5>
                            <p></p>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <img src="/public/media/imagenes/fumigaciones/05.jpg" class="d-block w-100" alt="..." draggable="false">
                        <div class="carousel-caption d-none d-md-block">
                            <h5></h5>
                            <p></p>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <img src="/public/media/imagenes/fumigaciones/06.jpg" class="d-block w-100" alt="..." draggable="false">
                        <div class="carousel-caption d-none d-md-block">
                            <h5></h5>
                            <p></p>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <img src="/public/media/imagenes/fumigaciones/07.jpg" class="d-block w-100" alt="..." draggable="false">
                        <div class="carousel-caption d-none d-md-block">
                            <h5></h5>
                            <p></p>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <img src="/public/media/imagenes/fumigaciones/08.jpg" class="d-block w-100" alt="..." draggable="false">
                        <div class="carousel-caption d-none d-md-block">
                            <h5></h5>
                            <p></p>
                        </div>
                    </div>
                </div>
                <button class="carousel-control-prev" type="button" data-bs-target="#carrusel" data-bs-slide="prev">
                    <span class="carousel-control-prev-icon bg-secondary" aria-hidden="true"></span>
                    <span class="visually-hidden">Previous</span>
                </button>
                <button class="carousel-control-next" type="button" data-bs-target="#carrusel" data-bs-slide="next">
                    <span class="carousel-control-next-icon bg-secondary" aria-hidden="true"></span>
                    <span class="visually-hidden">Next</span>
                </button>
            </div>
            <div class="bg-secondary" style="height: 9vh;"></div>
        </div>

    </section>
    <footer class="bg-primary centrado" style="height: auto;" title="© Fumigaciones Serviexpress Todos los derechos reservados.">
        <span class="text-secondary text-center tipoDeFuenteDos">
            © {{anioActual}} Fumigaciones Serviexpress Todos los derechos reservados.
        </span>
        <div style="height: 25vh"></div>
        <nav class="navbar navbar-expand-lg fixed-bottom transparente" data-bs-theme="dark">
            <div class="container-fluid">
                <div></div>
                <div>
                    <a href="https://www.facebook.com/FumigacionesServiExpress" target="_blank" title="Facebook">
                        <img src="/public/media/imagenes/logos_empresas_de_terceros/facebook.png" alt="Logo de" width="50vw" height="50vh" draggable="false">
                    </a>
                    <a href="https://www.instagram.com/fumigaciones_serviexpress" target="_blank" title="Instagram">
                        <img src="/public/media/imagenes/logos_empresas_de_terceros/instagram.png" alt="Logo de" width="50vw" height="50vh" draggable="false">
                    </a>
                    <a href="https://wa.me/c/50498573914" target="_blank" title="Whatsapp">
                        <img src="/public/media/imagenes/logos_empresas_de_terceros/whatsapp.png" alt="Logo de" width="50vw" height="50vh" draggable="false">
                    </a>
                </div>
            </div>
        </nav>
    </footer>
</template>

<script>
    import Proceso_antes_de_la_fumigacion from './Proceso_antes_de_la_fumigacion.vue'

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
            Proceso_antes_de_la_fumigacion
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
    .elementoSinSubrayado
    {
        text-decoration: none;
    }
    .transparente
    {
        background-color: rgba(255, 255, 255, 0);
    }
</style>