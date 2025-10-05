# Sondage

Contrat sur Celo : 0xefdfba94544fc85074267307c8753def4866b931

Créer et gérer des sondages :
creerSondage(question, options[], dureeEnSecondes)

Créer un sondage avec une question et 2 à 10 options
Définir une durée de validité
Exemple : creerSondage("Quelle est votre pizza préférée?", ["Margherita", "4 fromages", "Pepperoni"], 86400) pour 24h

voter(idSondage, indexOption)

Voter pour une option (un seul vote par adresse)
Vérifie automatiquement que le sondage est actif

fermerSondage(idSondage)

Le créateur peut fermer son sondage avant la fin

Consulter les résultats :
Informations générales :

obtenirInfosSondage() - Détails du sondage, nombre de votes, statut
obtenirToutesLesOptions() - Liste complète des options et votes
obtenirResultats() - Résultats avec pourcentages (×100 pour précision)
obtenirOptionGagnante() - L'option avec le plus de votes

Statistiques :

obtenirTempsRestant() - Temps avant la fin du sondage
aVote(utilisateur) - Vérifier si quelqu'un a voté
estActif() - Statut du sondage

Navigation :
Lister les sondages :

obtenirSondagesActifs() - Tous les sondages en cours
obtenirMesSondages() - Sondages que vous avez créés
obtenirSondagesCreateur(adresse) - Sondages d'un créateur spécifique

Caractéristiques :
✅ Sécurité :

Un vote par adresse
Vérification automatique de la durée
Seul le créateur peut fermer son sondage

✅ Transparence :

Résultats visibles en temps réel
Calcul automatique des pourcentages
Historique complet des votes via événements

✅ Flexibilité :

Durée personnalisable
2 à 10 options par sondage
Fermeture manuelle ou automatique

Le contrat est parfait pour des votes communautaires, des décisions de groupe, ou des enquêtes d'opinion, sans aucun fonds nécessaire ! 🗳️
