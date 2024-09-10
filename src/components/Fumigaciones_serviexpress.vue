<template>
    <div class="modal fade" id="modalProcesoAntesDeLaFumigacion" data-bs-backdrop="static" data-bs-keyboard="false" tabindex="-1" aria-labelledby="modalProcesoAntesDeLaFumigacionLabel" aria-hidden="true">
        <Proceso_antes_de_la_fumigacion></Proceso_antes_de_la_fumigacion>
    </div>
    <header style="height: 86px;">
        <nav class="navbar navbar-expand-lg bg-primary fixed-top" data-bs-theme="dark">
            <div class="container-fluid">
                <a class="navbar-brand">
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
                            <a class="nav-link fw-bold" href="#sobreNosotros">
                                Sobre nosotros
                            </a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link fw-bold" href="#galeria">
                                Galería
                            </a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link fw-bold" href="#horarios">
                                Horarios
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
                    <span class="text-primary h3 text-center tipoDeFuenteDos cartaAmarilla">
                        <i>
                            "Entorno sano, mente sana"
                        </i>
                    </span>
                </div>
            </div>
        </div>

        <div id="contenedorServicios" class="pt-2 bg-secondary" title="Servicios">
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

        <div id="contenedorSobreNosotros" class="pt-2 pb-3 bg-primary" title="Sobre nosotros">
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

        <div id="contendorGaleria" class="pt-1 bg-secondary" title="Galería">
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
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="8" aria-label="Slide 9"></button>
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="9" aria-label="Slide 10"></button>
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="10" aria-label="Slide 11"></button>
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="11" aria-label="Slide 12"></button>
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="12" aria-label="Slide 13"></button>
                    <button type="button" data-bs-target="#carrusel" data-bs-slide-to="13" aria-label="Slide 14"></button>
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
                    <div class="carousel-item">
                        <img src="/public/media/imagenes/fumigaciones/09.jpg" class="d-block w-100" alt="..." draggable="false">
                        <div class="carousel-caption d-none d-md-block">
                            <h5></h5>
                            <p></p>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <img src="/public/media/imagenes/fumigaciones/10.jpg" class="d-block w-100" alt="..." draggable="false">
                        <div class="carousel-caption d-none d-md-block">
                            <h5></h5>
                            <p></p>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <img src="/public/media/imagenes/fumigaciones/11.jpg" class="d-block w-100" alt="..." draggable="false">
                        <div class="carousel-caption d-none d-md-block">
                            <h5></h5>
                            <p></p>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <img src="/public/media/imagenes/fumigaciones/12.jpg" class="d-block w-100" alt="..." draggable="false">
                        <div class="carousel-caption d-none d-md-block">
                            <h5></h5>
                            <p></p>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <img src="/public/media/imagenes/fumigaciones/13.jpg" class="d-block w-100" alt="..." draggable="false">
                        <div class="carousel-caption d-none d-md-block">
                            <h5></h5>
                            <p></p>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <img src="/public/media/imagenes/fumigaciones/14.jpg" class="d-block w-100" alt="..." draggable="false">
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

        <div id="contenedorHorarios" class="container-fluid pt-2 pb-3 bg-primary" title="Horarios">
            <div class="tituloSeccion mb-2">
                <img class="w-100 d-block d-lg-none" src="/public/media/imagenes/titulos/horarios_disponibles.png" alt="titulo de la seccion galería" draggable="false">
                <img class="w-75 d-none d-lg-block" src="/public/media/imagenes/titulos/horarios_disponibles.png" alt="titulo de la seccion galería" draggable="false">
            </div>
            <div class="d-block d-md-none">
                <div class="centrado">
                    <span class="text-secondary fw-bold text-center">
                        Aplica a Revisiones e Inspecciones, Ejecuciones de Fumigaciones y Tratamientos especiales.
                        <br>
                        <br>
                        *De Lunes a Domingo *
                        <br>
                        <br>
                        - [ ] 06:30 Am a 07:30 Am
                        <br>
                        - [ ] 08:00 Am a 09:30 Am
                        <br>
                        - [ ] 10:00 Am a 11:30 Am
                        <br>
                        - [ ] 01:00 Pm a 02:30 Pm
                        <br> 
                        - [ ] 03:00 Pm a 04:30 Pm
                        <br>
                        - [ ] 05:00 Pm a 06:30 Pm
                        <br>
                        - [ ] 07:00 Pm a 08:30 Pm
                        <br>
                        - [ ] 09:00 Pm a 10:30 Pm
                        <br>
                        <br>
                        <span class="text-dark">
                            Si usted requiere algún horario especial que no aparece por favor consulte y seguro le podemos ayudar.
                        </span>
                        <br>
                        <br>
                        Todas la Fumigaciones, Tratamientos especiales e Inspecciones se programan con anticipación para no fallarle, no olvide seguir los pasos del Antes de la Fumigación que son suministrados por nuestros asesores de servicio al cliente.
                        <br>
                        <br>
                        <i>
                            “Entorno Sano, Mente Sana”
                        </i>
                    </span>
                </div>
            </div>
            <div class="d-none d-md-block">
                <div class="centrado">
                    <div class="w-50">
                        <div class="centrado">
                            <span class="text-secondary fw-bold text-center">
                                Aplica a Revisiones e Inspecciones, Ejecuciones de Fumigaciones y Tratamientos especiales.
                                <br>
                                <br>
                                *De Lunes a Domingo *
                                <br>
                                <br>
                                - [ ] 06:30 Am a 07:30 Am
                                <br>
                                - [ ] 08:00 Am a 09:30 Am
                                <br>
                                - [ ] 10:00 Am a 11:30 Am
                                <br>
                                - [ ] 01:00 Pm a 02:30 Pm
                                <br> 
                                - [ ] 03:00 Pm a 04:30 Pm
                                <br>
                                - [ ] 05:00 Pm a 06:30 Pm
                                <br>
                                - [ ] 07:00 Pm a 08:30 Pm
                                <br>
                                - [ ] 09:00 Pm a 10:30 Pm
                                <br>
                                <br>
                                <span class="text-dark">
                                    Si usted requiere algún horario especial que no aparece por favor consulte y seguro le podemos ayudar.
                                </span>
                                <br>
                                <br>
                                Todas la Fumigaciones, Tratamientos especiales e Inspecciones se programan con anticipación para no fallarle, no olvide seguir los pasos del Antes de la Fumigación que son suministrados por nuestros asesores de servicio al cliente.
                                <br>
                                <br>
                                <i>
                                    “Entorno Sano, Mente Sana”
                                </i>
                            </span>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div id="contenedorContacto" class="container-fluid pt-2 pb-3 bg-secondary" title="Contacto">
            <div class="tituloSeccion mb-2">
                <img class="w-50 d-block d-lg-none" src="/public/media/imagenes/titulos/contacto.png" alt="titulo de la seccion galería" draggable="false">
                <img class="w-50 d-none d-lg-block" src="/public/media/imagenes/titulos/contacto.png" alt="titulo de la seccion galería" draggable="false">
            </div>
            <div class="d-block d-md-none">
                <form action="https://formspree.io/f/xdknjqbb" method="POST">
                    <label class="col-sm-12 text-primary fw-bold" for="nombreCero">
                        Nombre:
                    </label>
                    <div class="col-sm-12 mb-3">
                        <input type="text" class="form-control" id="nombreCero" name="NombreCero" title="Nombre" style="background-color: rgba(242, 255, 0, 0.618); border:solid  rgba(242, 255, 0) 4px; color:rgba(255, 0, 0); font-weight: bold;">
                        <small class="bg-primary text-secondary fw-bold" id="mensajeValidacionNombreCero"></small>
                    </div>

                    <label class="col-sm-12 text-primary fw-bold" for="primerApellidoCero">
                        Primer apellido:
                    </label>
                    <div class="col-sm-12 mb-3">
                        <input type="text" class="form-control" id="primerApellidoCero" name="PrimerApellidoCero" title="Primer apellido" style="background-color: rgba(242, 255, 0, 0.618); border:solid  rgba(242, 255, 0) 4px; color:rgba(255, 0, 0); font-weight: bold;">
                        <small class="bg-primary text-secondary fw-bold" id="mensajeValidacionPrimerApellidoCero"></small>
                    </div>

                    <label class="col-sm-12 text-primary fw-bold" for="segundoApellidoCero">
                        Segundo apellido:
                    </label>
                    <div class="col-sm-12 mb-3">
                        <input type="text" class="form-control" id="segundoApellidoCero" name="SegundoApellidoCero" title="Segundo apellido" style="background-color: rgba(242, 255, 0, 0.618); border:solid  rgba(242, 255, 0) 4px; color:rgba(255, 0, 0); font-weight: bold;">
                        <small class="bg-primary text-secondary fw-bold" id="mensajeValidacionSegundoApellidoCero"></small>
                    </div>

                    <label class="col-sm-12 text-primary fw-bold" for="correoElectronicoCero">
                        Correo electrónico:
                    </label>
                    <div class="col-sm-12 mb-3">
                        <input type="email" class="form-control" id="correoElectronicoCero" name="CorreoElectronicoCero" title="Correo electrónico" style="background-color: rgba(242, 255, 0, 0.618); border:solid  rgba(242, 255, 0) 4px; color:rgba(255, 0, 0); font-weight: bold;">
                        <small class="bg-primary text-secondary fw-bold" id="mensajeValidacionCorreoElectronicoCero"></small>
                    </div>

                    <label class="col-sm-12 text-primary fw-bold" for="mensajeCero">
                        Mensaje:
                    </label>
                    <div class="col-sm-12 mb-3">
                        <textarea class="form-control" id="mensajeCero" Name="MensajeCero" rows="3" title="Mensaje" style="background-color: rgba(242, 255, 0, 0.618); border:solid  rgba(242, 255, 0) 4px; color:rgba(255, 0, 0); font-weight: bold;"></textarea>
                        <small class="bg-primary text-secondary fw-bold" id="mensajeValidacionMensajeCero"></small>
                    </div>

                    <div class="col-sm-12 text-end">
                        <button type="reset" class="btn btn-dark fw-bold">
                            Resetear
                        </button>
                        <button type="submit" id="botonSubmitCero" class="btn btn-primary fw-bold" @click="validarFormulario($event.target.id)">
                            Enviar
                        </button>
                    </div>
                </form>
            </div>
            <div class="d-none d-md-block">
                <div class="centrado">
                    <div class="w-50">
                        <form action="https://formspree.io/f/xdknjqbb" method="POST">
                            <label class="col-sm-12 text-primary fw-bold" for="nombreUno">
                                Nombre:
                            </label>
                            <div class="col-sm-12 mb-3">
                                <input type="text" class="form-control" id="nombreUno" name="NombreUno" title="Nombre" style="background-color: rgba(242, 255, 0, 0.618); border:solid  rgba(242, 255, 0) 4px; color:rgba(255, 0, 0); font-weight: bold;">
                                <small class="bg-primary text-secondary fw-bold" id="mensajeValidacionNombreUno"></small>
                            </div>

                            <label class="col-sm-12 text-primary fw-bold" for="primerApellidoUno">
                                Primer apellido:
                            </label>
                            <div class="col-sm-12 mb-3">
                                <input type="text" class="form-control" id="primerApellidoUno" name="PrimerApellidoUno" title="Primer apellido" style="background-color: rgba(242, 255, 0, 0.618); border:solid  rgba(242, 255, 0) 4px; color:rgba(255, 0, 0); font-weight: bold;">
                                <small class="bg-primary text-secondary fw-bold" id="mensajeValidacionPrimerApellidoUno"></small>
                            </div>

                            <label class="col-sm-12 text-primary fw-bold" for="segundoApellidoUno">
                                Segundo apellido:
                            </label>
                            <div class="col-sm-12 mb-3">
                                <input type="text" class="form-control" id="segundoApellidoUno" name="SegundoApellidoUno" title="Segundo apellido" style="background-color: rgba(242, 255, 0, 0.618); border:solid  rgba(242, 255, 0) 4px; color:rgba(255, 0, 0); font-weight: bold;">
                                <small class="bg-primary text-secondary fw-bold" id="mensajeValidacionSegundoApellidoUno"></small>
                            </div>

                            <label class="col-sm-12 text-primary fw-bold" for="correoElectronicoUno">
                                Correo electrónico:
                            </label>
                            <div class="col-sm-12 mb-3">
                                <input type="email" class="form-control" id="correoElectronicoUno" name="CorreoElectronicoUno" title="Correo electrónico" style="background-color: rgba(242, 255, 0, 0.618); border:solid  rgba(242, 255, 0) 4px; color:rgba(255, 0, 0); font-weight: bold;">
                                <small class="bg-primary text-secondary fw-bold" id="mensajeValidacionCorreoElectronicoUno"></small>
                            </div>

                            <label class="col-sm-12 text-primary fw-bold" for="mensajeUno">
                                Mensaje:
                            </label>
                            <div class="col-sm-12 mb-3">
                                <textarea class="form-control" id="mensajeUno" Name="MensajeUno" rows="3" title="Mensaje" style="background-color: rgba(242, 255, 0, 0.618); border:solid  rgba(242, 255, 0) 4px; color:rgba(255, 0, 0); font-weight: bold;"></textarea>
                                <small class="bg-primary text-secondary fw-bold" id="mensajeValidacionMensajeUno"></small>
                            </div>

                            <div class="col-sm-12 text-end">
                                <button type="reset" class="btn btn-dark fw-bold">
                                    Resetear
                                </button>
                                <button type="submit" id="botonSubmitUno" class="btn btn-primary fw-bold" @click="validarFormulario($event.target.id)">
                                    Enviar
                                </button>
                            </div>
                        </form>
                    </div>
                </div>
            </div>
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
            },
            validarFormulario(idFormulario)
            {
                if(!this.validaciones(idFormulario))
                {
                    event.preventDefault();
                }
            },
            validaciones(idFormulario) {

                let nombre;
                let primerApellido;
                let segundoApellido;
                let correoElectronico;
                let mensaje;

                if(idFormulario==="botonSubmitCero")
                {
                    nombre=document.getElementById("nombreCero");
                    primerApellido=document.getElementById("primerApellidoCero");
                    segundoApellido=document.getElementById("segundoApellidoCero");
                    correoElectronico=document.getElementById("correoElectronicoCero");
                    mensaje=document.getElementById("mensajeCero");
                }
                else
                {
                    nombre=document.getElementById("nombreUno");
                    primerApellido=document.getElementById("primerApellidoUno");
                    segundoApellido=document.getElementById("segundoApellidoUno");
                    correoElectronico=document.getElementById("correoElectronicoUno");
                    mensaje=document.getElementById("mensajeUno");
                }

                let laTareaPasoTodasLasValidaciones=false;
                principal();
                function principal()
                {
                    let validacionCampoVacioNombre=false;
                    let validacionCaracteresExtraniosNombre=false;
                    let validacionLongitudNombre=false;
                    let campoNombrePasoTodasLasValidaciones=false;
                    validacionCampoVacioNombre=verificarQueElCampoNoEsteVacio(validacionCampoVacioNombre,nombre);
                    validacionCaracteresExtraniosNombre=verificarQueElCampoNoContengaCaracteresExtranios(validacionCaracteresExtraniosNombre,nombre);
                    validacionLongitudNombre=verificarLongitud(validacionLongitudNombre,nombre,2,30);

                    let validacionCampoVacioPrimerApellido=false;
                    let validacionCaracteresExtraniosPrimerApellido=false;
                    let validacionLongitudPrimerApellido=false;
                    let campoPrimerApellidoPasoTodasLasValidaciones=false;
                    validacionCampoVacioPrimerApellido=verificarQueElCampoNoEsteVacio(validacionCampoVacioPrimerApellido,primerApellido);
                    validacionCaracteresExtraniosPrimerApellido=verificarQueElCampoNoContengaCaracteresExtranios(validacionCaracteresExtraniosPrimerApellido,primerApellido);
                    validacionLongitudPrimerApellido=verificarLongitud(validacionLongitudPrimerApellido,primerApellido,2,30);

                    let validacionCampoVacioSegundoApellido=false;
                    let validacionCaracteresExtraniosSegundoApellido=false;
                    let validacionLongitudSegundoApellido=false;
                    let campoSegundoApellidoPasoTodasLasValidaciones=false;
                    validacionCampoVacioSegundoApellido=verificarQueElCampoNoEsteVacio(validacionCampoVacioSegundoApellido,segundoApellido);
                    validacionCaracteresExtraniosSegundoApellido=verificarQueElCampoNoContengaCaracteresExtranios(validacionCaracteresExtraniosSegundoApellido,segundoApellido);
                    validacionLongitudSegundoApellido=verificarLongitud(validacionLongitudSegundoApellido,segundoApellido,2,30);

                    let validacionCorreoElectronico=false;
                    let campoCorreoElectronicoPasoTodasLasValidaciones=false;
                    validacionCorreoElectronico=verificarSintaxisCorreo(validacionCorreoElectronico,correoElectronico);

                    let validacionCampoVacioMensaje=false;
                    let validacionLongitudMensaje=false;
                    let campoMensajePasoTodasLasValidaciones=false;
                    validacionCampoVacioMensaje=verificarQueElCampoNoEsteVacio(validacionCampoVacioMensaje,mensaje);
                    validacionLongitudMensaje=verificarLongitud(validacionLongitudMensaje,mensaje,2,280);

                    if(validacionCampoVacioNombre&&validacionCaracteresExtraniosNombre&&validacionLongitudNombre)
                    {
                        if(idFormulario==="botonSubmitCero")
                        {
                            let mensajeError = document.getElementById("mensajeValidacionNombreCero");
                            mensajeError.textContent = "";
                        }
                        else
                        {
                            let mensajeError = document.getElementById("mensajeValidacionNombreUno");
                            mensajeError.textContent = "";
                        }
                        campoNombrePasoTodasLasValidaciones=true;
                    }
                    
                    if(validacionCampoVacioPrimerApellido&&validacionCaracteresExtraniosPrimerApellido&&validacionLongitudPrimerApellido)
                    {
                        if(idFormulario==="botonSubmitCero")
                        {
                            let mensajeError = document.getElementById("mensajeValidacionPrimerApellidoCero");
                            mensajeError.textContent = "";
                        }
                        else
                        {
                            let mensajeError = document.getElementById("mensajeValidacionPrimerApellidoUno");
                            mensajeError.textContent = "";
                        }
                        campoPrimerApellidoPasoTodasLasValidaciones=true;
                    }

                    if(validacionCampoVacioSegundoApellido&&validacionCaracteresExtraniosSegundoApellido&&validacionLongitudSegundoApellido)
                    {
                        if(idFormulario==="botonSubmitCero")
                        {
                            let mensajeError = document.getElementById("mensajeValidacionSegundoApellidoCero");
                            mensajeError.textContent = "";
                        }
                        else
                        {
                            let mensajeError = document.getElementById("mensajeValidacionSegundoApellidoUno");
                            mensajeError.textContent = "";
                        }
                        campoSegundoApellidoPasoTodasLasValidaciones=true;
                    }
                    
                    if(validacionCorreoElectronico)
                    {
                        if(idFormulario==="botonSubmitCero")
                        {
                            let mensajeError = document.getElementById("mensajeValidacionCorreoElectronicoCero");
                            mensajeError.textContent = "";
                        }
                        else
                        {
                            let mensajeError = document.getElementById("mensajeValidacionCorreoElectronicoUno");
                            mensajeError.textContent = "";
                        }
                        campoCorreoElectronicoPasoTodasLasValidaciones=true;
                    }

                    if(validacionCampoVacioMensaje&&validacionLongitudMensaje)
                    {
                        if(idFormulario==="botonSubmitCero")
                        {
                            let mensajeError = document.getElementById("mensajeValidacionMensajeCero");
                            mensajeError.textContent = "";
                        }
                        else
                        {
                            let mensajeError = document.getElementById("mensajeValidacionMensajeUno");
                            mensajeError.textContent = "";
                        }
                        campoMensajePasoTodasLasValidaciones=true;
                    }
                    
                    if(campoNombrePasoTodasLasValidaciones&&campoPrimerApellidoPasoTodasLasValidaciones&&campoSegundoApellidoPasoTodasLasValidaciones&&campoCorreoElectronicoPasoTodasLasValidaciones&&campoMensajePasoTodasLasValidaciones)
                    {
                        laTareaPasoTodasLasValidaciones=true;
                    }
                }

                function verificarQueElCampoNoEsteVacio(validacionCampoVacio,elementoInput)
                {
                    // Elimina los espacios en blanco del valor del elemento input
                    let elementoInputSinEspacios = elementoInput.value.trim();

                    // Verifica si el campo nombre está vacío
                    if (elementoInputSinEspacios === "")
                    {
                        // El campo nombre está vacío
                        // Muestra un mensaje de error
                        let mensajeError = document.getElementById("mensajeValidacion"+elementoInput.name);
                        mensajeError.textContent = "*El campo '"+elementoInput.name+"' no puede quedar vacío.";

                        // Evita que el formulario se envíe
                        event.preventDefault();
                    }
                    else
                    {
                        validacionCampoVacio=true;
                    }
                    return validacionCampoVacio;
                }
                function verificarQueElCampoNoContengaCaracteresExtranios(validacionCaracteresExtranios,elementoInput)
                {
                    // Verifica si el campo nombre tiene algún caracter que no sea una letra del alfabeto español
                    const contieneCaracteresNoEspanoles = /[^a-záéíóúüññç\s]/i.test(elementoInput.value);

                    // Si el campo nombre tiene algún caracter que no sea una letra del alfabeto español, muestra un mensaje de error
                    if (contieneCaracteresNoEspanoles)
                    {
                        // El campo nombre tiene algún caracter que no sea una letra del alfabeto español
                        // Muestra un mensaje de error
                        const mensajeError = document.getElementById("mensajeValidacion"+elementoInput.name);
                        mensajeError.textContent = "*Este campo solo puede contener letras del alfabeto español.";

                        // Evita que el formulario se envíe
                        event.preventDefault();
                    }
                    else
                    {
                        validacionCaracteresExtranios=true;
                    }
                    return validacionCaracteresExtranios;
                }
                function verificarLongitud(validacionLongitud,elementoInput,longitudMinima,longitudMaxima)
                {
                    // Verifica si la longitud del campo nombre es menor a 35
                    longitudMaxima=longitudMaxima+1;
                    let longitudMuyCorta=elementoInput.value.length < longitudMinima;
                    let longitudMuyLarga=elementoInput.value.length >= longitudMaxima;
                    /*console.log("Longitud muy corta: "+longitudMuyCorta);
                    console.log("Longitud muy larga: "+longitudMuyLarga);
                    console.log(" ");*/

                    // Si la longitud del campo nombre es mayor o igual a 35, muestra un mensaje de error
                    if(longitudMuyCorta||longitudMuyLarga)
                    {
                        // Muestra un mensaje de error
                        const mensajeError = document.getElementById("mensajeValidacion"+elementoInput.name);
                        longitudMaxima=longitudMaxima-1;
                        if(longitudMuyCorta)
                        {
                            mensajeError.textContent = "*La longitud del campo no puede ser menor a "+longitudMinima+" caracter(es).";
                        }
                        else if(longitudMuyLarga)
                        {
                            mensajeError.textContent = "*La longitud del campo no puede ser mayor a "+longitudMaxima+" caracteres.";
                        }
                        // Evita que el formulario se envíe
                        event.preventDefault();
                    }
                    else
                    {
                        validacionLongitud=true;
                    }
                    return validacionLongitud;
                }
                function verificarSintaxisCorreo(validacionSintaxisCorreo,correo)
                {
                    // Verifica si el valor del input coincide con el patrón
                    const coincideConElPatron = correo.value.match(/[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}/);

                    // Si el valor del input no coincide con el patrón, muestra un mensaje de error
                    if (!coincideConElPatron)
                    {
                        // El valor del input no coincide con el patrón
                        // Muestra un mensaje de error
                        const mensajeError = document.getElementById("mensajeValidacion"+correo.name);
                        mensajeError.textContent = "*El correo electrónico no es válido.";

                        // Evita que el formulario se envíe
                        event.preventDefault();
                    }
                    else
                    {
                        validacionSintaxisCorreo=true;
                    }
                    return validacionSintaxisCorreo;
                }

                return laTareaPasoTodasLasValidaciones;
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
    .elementoSubrayado
    {
        text-decoration: underline;
    }
    .inputText
    {
        background-color: rgba(242, 255, 0, 0.387);
        border:solid  rgba(242, 255, 0) 4px;
        color:rgba(255, 0, 0);
        font-weight: bold;
    }
</style>