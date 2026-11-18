# Résumé du projet — Yumio

## Présentation

Yumio est une application web de recettes de cuisine. Elle permet aux visiteurs de parcourir un catalogue, de filtrer les recettes et de consulter leurs ingrédients, leurs quantités, leurs étapes et leurs images. Le projet prévoit également la création de comptes, la publication de recettes, la gestion des favoris et des espaces utilisateur et administrateur.

## Objectifs

L’application vise à rendre la recherche et le partage de recettes simples. Un utilisateur peut retrouver une idée de repas, consulter les informations nécessaires à sa préparation et, à terme, contribuer au catalogue en publiant ses propres recettes.

## Fonctionnalités réalisées ou amorcées

- Une interface web réalisée avec Angular, comprenant l’accueil, le catalogue, la recherche/filtrage, le détail des recettes, l’inscription et la connexion.
- Une API organisée en services Spring Boot pour l’authentification, les recettes et les ingrédients, avec une gateway, un service de découverte et un serveur de configuration.
- Un modèle de données reliant les utilisateurs aux recettes et les recettes à leurs ingrédients.
- Des bases PostgreSQL prévues pour les données métier et un stockage objet Cloudflare R2 prévu pour les images.
- Des fonctions de profil, favoris, administration et création de recettes présentes à des degrés d’avancement différents.

## Environnement technique

**Frontend :** Angular 22, TypeScript, Tailwind CSS.  
**Backend :** Java, Spring Boot, Spring Security, API REST.  
**Données et infrastructure :** PostgreSQL, Cloudflare R2, Docker Compose, JWT.

## État d’avancement

Le socle frontend et l’architecture backend sont en place. Le catalogue et la consultation des recettes sont amorcés. Plusieurs parcours — notamment la publication complète d’une recette, les favoris et la gestion de session — nécessitent encore des corrections et une validation de bout en bout.

Avant une ouverture à de vrais utilisateurs, les priorités sont de sécuriser les accès et les données personnelles, de finaliser l’authentification côté serveur, de fiabiliser les formulaires et les erreurs, puis de tester les parcours complets. Les vérifications locales disponibles portent principalement sur le chargement des applications ; elles ne valident pas encore le comportement de toute la plateforme en conditions réelles.

## Conclusion

Yumio constitue une base de prototype full-stack pour la découverte et le partage de recettes. Son architecture et ses principaux écrans sont amorcés ; la prochaine étape consiste à consolider la sécurité et à terminer les parcours essentiels avant de le présenter comme un MVP prêt pour ses utilisateurs.