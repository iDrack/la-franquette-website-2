<script setup> 
let features = [
    {
       icon: "/ressources/img/icons-product/feature-solution.png",
       iconAlt: "Image de résolution de problème",
       title: "La solution",
       subtitle: "plutôt que des solutions",
       description: "Nous avons spécialement conçu nos fonctionnalités pour répondre aux besoins uniques des petits restaurateurs."

    },
    {
       icon: "/ressources/img/icons-product/feature-rapide.png",
       iconAlt: "Image présentant le gain de temps associé à notre produit",
       title: "Gagnez du temps",
       subtitle: "au quotidien",
       description: "Notre application vous permet de vous concentrer sur vos clients et le développement de votre entreprise."
    },
    {
       icon: "/ressources/img/icons-product/feature-paiement.png",
       iconAlt: "Image d'adaptabilité sans compromis",
       title: "Adaptabilité",
       subtitle: "sans compromis",
       description: "Nous croyons en la puissance du choix en vous laissant maître de votre processus de paiement."
    },
    {
       icon: "/ressources/img/icons-product/feature-gratuit.png",
       iconAlt: "Image de résolution de problème",
       title: "Installation gratuite",
       subtitle: "et facile",
       description: "Nous nous occupons de tout pour la première installation et ainsi vous permettre de démarrer facilement."     
    }
];
</script>

<template>
    <div class="title  mt-4 mb-8 text-center">
        <h2 class="font-sans text-3xl text-deep-purple-accent-400">Notre solution pour votre lancement</h2>
        <h3 class="mt-2">
            Laissez vous séduire par nos fonctionnalités, pensées pour 
            <span class="font-bold">vous</span>
        </h3>
    </div>
    <div class="grid place-content-center">
        <div class="features mx-4 flex justify-center flex-col lg:flex-row lg:space-x-12 lg:space-x-6 md:mt-8 my-0">
            <card class="rounded-xl shadow-lg p-8 md:min-w-48 lg:basis-1/5 basis-1/3 my-4"
                 v-for="feature in features">
                <div class="grid place-content-center my-2">
                    <img class="max-w-20":src="feature.icon" :alt="feature.iconAlt">
                </div>
                <h4 class=" mt-8 text-center font-bold">{{feature.title}}</h4>
                <h4 class=" mb-2 text-center">{{feature.subtitle}}</h4>
                <p class="my-2 text-center">{{feature.description}}</p>   
            </card>
        </div>
    </div>
</template>