<template>
    <div id="procesoAntesDeLaFumigacion" class="modal-dialog modal-dialog-centered">
        <div class="modal-content">
            <div class="modal-header bg-primary">
                <img class="w-100" src="/public/media/imagenes/titulos/proceso_antes_de_la_fumigación.png" alt="Proceso antes de la fumigación" draggable="false">
            </div>
            <div class="modal-body bg-secondary" style="height: 70vh; overflow-y: auto;">
                <div class="container-fluid">
                    <div class="row">
                        <div class="col-sm-12 contenedorFlexible mb-4">
                            <div class="w-50 centrado">
                                <span class="h5 text-primary tipoDeFuenteDos">
                                    Paso 1:
                                </span>
                            </div>
                            <div class="w-50 centrado">
                                <span class="text-primary fw-bold text-center">
                                    Ubicar todos los alimentos y consumibles en un lugar aislado.
                                </span>
                            </div>
                        </div>
                        <hr class="border border-primary">
                        <div class="col-sm-12 contenedorFlexible mb-4">
                            <div class="w-50 centrado">
                                <span class="h5 text-primary tipoDeFuenteDos">
                                    Paso 2:
                                </span>
                            </div>
                            <div class="w-50 centrado">
                                <span class="text-primary fw-bold text-center">
                                    Los utensilios de cocina también deberán ser almacenados en lugares seguros.
                                </span>
                            </div>
                        </div>
                        <hr class="border border-primary">
                        <div class="col-sm-12 contenedorFlexible mb-4">
                            <div class="w-50 centrado">
                                <span class="h5 text-primary tipoDeFuenteDos">
                                    Paso 3:
                                </span>
                            </div>
                            <div class="w-50 centrado">
                                <span class="text-primary fw-bold text-center">
                                    Todo mueble, pegado a la pared y se pueda mover, moverlos de frente al menos 10 centímetros.
                                </span>
                            </div>
                        </div>
                        <hr class="border border-primary">
                        <div class="col-sm-12 contenedorFlexible mb-4">
                            <div class="w-50 centrado">
                                <span class="h5 text-primary tipoDeFuenteDos">
                                    Paso 4:
                                </span>
                            </div>
                            <div class="w-50 centrado">
                                <span class="text-primary fw-bold text-center">
                                    Sacar todas sus Mascotas.
                                </span>
                            </div>
                        </div>
                        <hr class="border border-primary">
                        <div class="col-sm-12 contenedorFlexible mb-4">
                            <div class="w-50 centrado">
                                <span class="h5 text-primary tipoDeFuenteDos">
                                    Paso 5:
                                </span>
                            </div>
                            <div class="w-50 centrado">
                                <span class="text-primary fw-bold text-center">
                                    Desconectar todo electrodoméstico y cerrar los ductos de gas.
                                </span>
                            </div>
                        </div>
                        <hr class="border border-primary">
                        <div class="col-sm-12 contenedorFlexible mb-4">
                            <div class="w-50 centrado">
                                <span class="h5 text-primary tipoDeFuenteDos">
                                    Paso 6:
                                </span>
                            </div>
                            <div class="w-50 centrado">
                                <span class="text-primary fw-bold text-center">
                                    Los artículos tecnológicos, computadoras, impresoras, tvs  etc. Cubrir con toallas o sábanas delgadas.
                                </span>
                            </div>
                        </div>
                        <hr class="border border-primary">
                        <div class="col-sm-12 contenedorFlexible mb-4">
                            <div class="w-50 centrado">
                                <span class="h5 text-primary tipoDeFuenteDos">
                                    Paso 7:
                                </span>
                            </div>
                            <div class="w-50 centrado">
                                <span class="text-primary fw-bold text-center">
                                    En las cocinas,  sacar todo de las alacenas o muebles y colocar las cosas en una mesa de comedor, luego colocar una sábana, plástico o periódico eso es suficiente para iniciar la operación.
                                </span>
                            </div>
                        </div>
                        <hr class="border border-primary">
                        <div class="col-sm-12 contenedorFlexible mb-4">
                            <div class="w-50 centrado">
                                <span class="h5 text-primary tipoDeFuenteDos">
                                    Paso 8:
                                </span>
                            </div>
                            <div class="w-50 centrado">
                                <span class="text-primary fw-bold text-center">
                                    En las habitaciones, donde hay closets o muebles, colocar las cosas de los closets en una cama y luego cubrir o con una sábana, plástico o papel periódico.
                                </span>
                            </div>
                        </div>
                        <hr class="border border-primary">
                        <div class="col-sm-12 contenedorFlexible mb-3">
                            <span class="text-primary fw-bold text-center">
                                Trate de dejar la cocina lo más desnuda posible así como en las fotos, para poder entrar fisuras, rajaduras y hendiduras.
                            </span>
                        </div>
                        <div class="col-sm-12 contenedorFlexible mb-3">
                            <div class="w-100">
                                <img class="w-100" src="/public/media/imagenes/cocinas/cocina_0.jpg" alt="Imagen de prohibido insectos voladores" draggable="false">
                            </div>
                        </div>
                        <div class="col-sm-12 contenedorFlexible">
                            <div class="w-100 centrado">
                                <img class="w-100" src="/public/media/imagenes/cocinas/cocina_1.jpg" alt="Imagen de prohibido insectos voladores" draggable="false">
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="modal-footer bg-primary">
                <button type="button" class="btn btn-secondary fw-bold text-primary" id="botonCerrarModalNuestroEquipo" data-bs-dismiss="modal">
                    Atras
                </button>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style>
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
    .tipoDeFuenteDos
    {
        font-family: "Rammetto One", sans-serif;
    }
</style>