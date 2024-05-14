<script setup>
</script>
<template>
    <div id="career" class="career pt-[110px] px-6 py-8 lg:py-20">
        <div class="block text-2xl lg:text-[50px] font-bold mb-8 lg:mb-20 flex flex-col">
            <span>Mon parcours pro</span>
        </div>
        <div class="list">
            <div class="item">
                <div class="flex items-center justify-between mb-4">
                    <span class="font-semibold uppercase text-xl">ATI4 GROUP</span>
                    <span class="italic">Oct. 2020 - Juin 2024</span>
                </div>
                <p>Développement et maintenances de boutiques Magento2 en PHP pour des clients internationnaux. Travail en équipe et en méthode agile</p>
                <ul class="tags">
                    <li>Magento2</li>
                    <li>PHP</li>
                    <li>TailwindCSS</li>
                    <li>KnockoutJS</li>
                    <li>Hyva Themes</li>
                    <li>Git</li>
                    <li>Jira</li>
                </ul>
            </div>
            <div class="item">
                <div class="flex items-center justify-between mb-4">
                    <span class="font-semibold uppercase text-xl">Sirfull</span>
                    <span class="italic">Oct. 2020 - Avril 2021</span>
                </div>
                <p>Développement d'une solution digitalisée d'inspection et de maintenance d'équipements sous pression pour le groupe Total Energies</p>
                <ul class="tags">
                    <li>Angular</li>
                    <li>C#</li>
                    <li>Entity Framework</li>
                    <li>Git</li>
                    <li>Jira</li>
                </ul>
            </div>
            <div class="item">
                <div class="flex items-center justify-between mb-4">
                    <span class="font-semibold uppercase text-xl">Thuria</span>
                    <span class="italic">Juil. 2020 - Oct. 2020</span>
                </div>
                <p>Développement de sites internet de destinations touristiques avec Wordpress</p>
                <ul class="tags">
                    <li>Wordpress</li>
                    <li>Gulp</li>
                    <li>SCSS</li>
                    <li>Front-end</li>
                    <li>Adobe XD</li>
                </ul>
            </div>
        </div>
    </div>
</template>
<style>
    .career {
        .list {
            @apply flex flex-col lg:w-2/3 2xl:w-1/2 gap-4 lg:gap-12;

            .item {
                @apply border-b mb-4 pb-4;
            }
        }

        .tags {
            @apply flex flex-wrap gap-x-2 gap-y-2 my-4;
            
            li {
                @apply py-2 px-3 text-xs border rounded-lg flex-shrink-0 bg-slate-950 text-white;
            }
        }
    }
</style>