<template>
    <div class="main_div">
        <m-header />
        <div class="legal-page">
            <div class="title">
                <h1>Mentions légales</h1>
            </div>
            <div class="legal-content">
                <h2>Éditeur du site</h2>
                <p>Mathis BEAL<br>
                    Adresse : 23 Allée des Chênes, 43240 Saint-Just-Malmont<br>
                    Email : <a href="mailto:mathis.beal04@gmail.com">mathis.beal04@gmail.com</a><br>
                </p>
                <h2>Contact</h2>
                <p>Pour toute question ou demande concernant ce site, vous pouvez me contacter à l'adresse suivante : <a href="mailto:mathis.beal04@gmail.com">mathis.beal04@gmail.com</a></p>
                <h2>Collecte des données</h2>
                <p>Ce site ne collecte aucune donnée personnelle. Aucune information concernant les visiteurs n'est enregistrée ou exploitée à des fins commerciales ou statistiques.</p>
                <h2>Hébergement</h2>
                <p>Ce site est hébergé par :<br>
                    Le service de page de Github, Github.io<br>
                    <!-- Adresse : [Adresse de l'hébergeur]<br> -->
                </p>
                <h2>Propriété intellectuelle</h2>
                <p>Tous les contenus présents sur ce site (textes, images, logos, etc.) sont la propriété exclusive de
                    Mathis BEAL, sauf mention contraire. Toute reproduction, représentation, modification, publication,
                    adaptation de tout ou partie des éléments du site, quel que soit le moyen ou le procédé utilisé, est
                    interdite, sauf autorisation écrite préalable.</p>
                <h2>Responsabilité</h2>
                <p>Mathis BEAL s'efforce de fournir sur ce site des informations aussi précises que possible. Toutefois,
                    il ne pourra être tenu responsable des omissions, des inexactitudes et des carences dans la mise à
                    jour, qu'elles soient de son fait ou du fait des tiers partenaires qui lui fournissent ces
                    informations.</p>
                <h2>Cookies</h2>
                <p>Ce site n'utilise aucun cookie et ne collecte aucune donnée personnelle via des cookies.</p>
            </div>
        </div>
        <m-footer />
    </div>
</template>

<script setup lang="ts">
// No script needed
</script>

<style scoped>
.title {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: fit-content;
    text-align: center;
    color: #242424;
    margin-bottom: 2rem;
    border-bottom: 0.2rem solid #242424;
}

.legal-page {
    max-width: 32rem;
    margin: auto;
    background: #f8f8f8;
    box-shadow: 0 2px 12px rgba(63, 163, 107, 0.10);
    padding: 2rem 2.5rem;
    color: #2c3e50;
}

.legal-content h2 {
    color: #3fa36b;
    text-decoration: underline #3fa36b;
    margin-top: 2rem;
    margin-bottom: 0.7rem;
    font-size: 1.1rem;
}

.legal-content p {
    margin-bottom: 1.2rem;
    line-height: 1.6;
}
</style>
