<script setup>
    import digiresaLogo from '../assets/digiresa-logo.webp'
    import flamsLogo from '../assets/flams-logo.png'
    import mdvLogo from '../assets/mdv-logo.png'
</script>
<template>
    <div id="projects" class="projects pt-[80px] lg:pt-[110px] px-6 lg:my-12">
        <div class="block text-2xl lg:text-[50px] font-bold mb-8 flex flex-col">
            <span>Mes projets</span>
            <span class="italic font-normal text-sm lg:text-lg lg:py-5">(et j'en suis vraiment fier)</span>
        </div>
        <div class="list">
            <div class="project-item">
                <div class="flex flex-col grow">
                    <div class="infos">
                        <picture>
                            <img :src="digiresaLogo" alt="Logo DigiResa">
                        </picture>
                        <div class="texts">
                            <span class="title">DigiResa - Application web pour restaurants</span>
                            <p>Lead développeur Angular et Symfony de DigiResa, une application web de réservation et de fidélisation pour restaurants. Actuellement en production pour 5 restaurants en France.</p>
                        </div>
                    </div>
                    <div class="technos">
                        <span>#angular</span>
                        <span>#symfony</span>
                        <span>#plesk</span>
                        <span>#cloudflare</span>
                        <span>#déploiements automatisés</span>
                    </div>
                </div>
                <a href="https://www.digiresa.com/" target="_blank">Voir le site</a>
            </div>
            <div class="project-item">
                <div class="flex flex-col grow">
                    <div class="infos">
                        <picture>
                            <img :src="flamsLogo" alt="Logo Flam's">
                        </picture>
                        <div class="texts">
                            <span class="title">Flam's - Carte dématérialisée pour restaurants</span>
                            <p>Solution de gestion de cartes dématérialisées pour restaurants en Angular et Symfony utilisé par plus d'une vingtaine de restaurants en France.</p>
                        </div>
                    </div>
                    <div class="technos">
                        <span>#angular</span>
                        <span>#symfony</span>
                    </div>
                </div>
                <a href="https://carte.flams.fr/#/carte/strasbourg" target="_blank">Voir le site</a>
            </div>
            <div class="project-item">
                <div class="flex flex-col grow">
                    <div class="infos">
                        <picture>
                            <img :src="mdvLogo" alt="Logo Massif des Vosges">
                        </picture>
                        <div class="texts">
                            <span class="title">Massif des Vosges - Destination touristique</span>
                            <p>Site internet d'une destination touristique réalisé lors de ma mission à l'agence Thuria à Strasbourg.</p>
                        </div>
                    </div>
                    <div class="technos">
                        <span>#wordpress</span>
                        <span>#scss</span>
                        <span>#gulp</span>
                        <span>#adobexd</span>
                    </div>
                </div>
                <a href="https://www.massif-des-vosges.fr/" target="_blank">Voir le site</a>
            </div>
        </div>
    </div>
</template>
<style>
    .projects {

        .list {
            @apply grid grid-cols-1 lg:grid-cols-3 gap-6;

            .project-item {
                @apply flex flex-col p-4 border border-slate-300 rounded shadow-md;

                .infos {
                    picture {
                        @apply block bg-slate-950 w-full p-6 flex items-center justify-center mb-4;

                        img {
                            @apply h-[70px];
                        }
                    }

                    .texts {
                        .title {
                            @apply block font-semibold py-4;
                        }
                    }
                }

                .technos {
                    @apply py-6 flex gap-x-6 gap-y-2 flex-wrap;
                }

                a {
                    @apply flex justify-center p-4 bg-[#FC9828] text-white;
                }
            }
        }
    }
</style>