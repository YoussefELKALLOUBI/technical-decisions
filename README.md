# technical-decisions

Décisions techniques prises lors de mon alternance chez Sylvamap.

## Implémentation 2FA

Intégration manuelle vs Bibliothèque
- Choix : Intégration manuelle
- Pourquoi : Contrôle total, adaptation aux besoins, meilleure traçabilité de sécurité
- Rejeté : django-two-factor-auth (trop rigide)

## Fournisseur SMS

Twilio vs Vonage vs Plivo
- Choix : Twilio
- Pourquoi : 99.99% uptime, meilleure communauté, docs excellentes
- Critères : fiabilité, coûts, taille communauté, support

## Stockage du code

Django Cache vs PostgreSQL
- Choix : Django Cache
- Pourquoi : Expiration auto après 15min, pas de nettoyage manuel, plus rapide

## Format du code

CharField vs Integer
- Choix : CharField pour code 6 chiffres
- Pourquoi : Préserve les zéros ("001234" reste "001234")
- Problème Integer : Perd les zéros, casse la validation

## Numéros de téléphone

Champs séparés
- phone_number (profil)
- phone_2fa (sécurité)
- Pourquoi : Changer le téléphone n'affecte pas 2FA. Architecture plus propre.

## Optimisation de code

Fusion de vues Django similaires
- Consolidé activate_2fa_view et disable_2fa_view avec héritage de classe
- Supprimé 50+ lignes dupliquées
- Plus facile à maintenir, respecte le principe DRY


## Processus

Chaque décision documentée via des issues GitHub pour la traçabilité.
