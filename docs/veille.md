# Veille

Ce tableau retrace les différentes recherches effectuées au cours de mon projet pour le déploiement et sa sécurité mais aussi le choix de version de Node.js . 

| Sources | Dates | Informations retenues | Risques ou Opportunités | Décision |
|---------|-------|-----------------------|--------------------------|---------|
| vercel.com/docs/deployments | 22/09/2026 | - Réaliser un déploiement <br> - Les types d'environnements | - Possibilité avec Git, directement sur Vercel( ligne de commande, glisse, via une URL, API REST) <br> - Preview est utilisé après un premier déploiement en production | - Création d'un repository <br> - Déploiement en production|
| vercel.com/docs/functions/ | 22/09/2026 | La version de Node.js peut être modifiée | Node.js peut être modifié depuis les paramètres du projet sur vercel ou dans le fichier package.json | Modification depuis le dashbord, utilisation de la dernière version 24.x |
|vercel.com/docs/project-configuration/security-settings | 22/09/2026 | - Journaux de compilation et protection du code source | - Activez la fonctionnalité protection du code et suivi des compilations : seul les membres autorisés peuvent le voir <br> - Activez la fonctionnalité protection des branches : nécessite une validation de la pull request avant d'être déployé sur le projet  | Activation de ces deux fonctionnalités |
| tuxcare.com/fr/blog/node-eol/ | 22/09/2026 | Ancienne version de Node.js, impact sur le déploiement | Le site ne sera pas déployé correctement si le projet utilise une version antérieure à node 20.x. Les anciennes versions n'obtiennent plus les correctifs nécessaires à la sécurité. Le code deviendra plus difficile à maintenir.