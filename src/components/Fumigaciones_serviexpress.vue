<template>
    <header>
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
                            <a class="nav-link dropdown-toggle" data-bs-toggle="dropdown" href="tratamientos" role="button" aria-haspopup="true" aria-expanded="false">
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
                                <a class="dropdown-item" href="#">F. termitas, carcoma, polilla, comejen.</a>
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
    <section>

    </section>
    <footer>

    </footer>
</template>

<script>
    export default {
        
    }
</script>

<style>
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
</style>