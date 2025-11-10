# Expériences Techniques

## Sylvamap – 2FA

**Intégration manuelle** vs django-two-factor-auth → Contrôle total, traçabilité sécurité
[📸 Voir](https://github.com/user-attachments/assets/6e5257ca-b98c-49a1-b7bd-68161c9a052f)

**Twilio vs Vonage** → 99.99% uptime, communauté
[📸 Voir](https://github.com/user-attachments/assets/9e9c44ab-7e6c-4410-b0cc-180ee3e4094d)

**Django Cache vs PostgreSQL** → Expiration auto 15min

**CharField vs Integer** → Préserve zéros ("001234")

**phone_number + phone_2fa** → Séparation propre, changement phone n'affecte pas 2FA

**Refactoring views** : activate/disable_2fa fusionnées, -50 lignes, DRY
[📸 Voir](https://github.com/user-attachments/assets/f17ec5e0-0577-4a7c-bb05-2ebfc1c1e23a)

---

## Tests & CI/CD

Tests unitaires + intégration GitHub Actions
[📸 Voir](https://github.com/user-attachments/assets/604da21f-c96a-49ed-9195-9fa1f259751c)

---

## Phileas – Mobile API C# & Authentification

App Mobile → API C# Service → BDD
[📸 Architecture 1](https://github.com/user-attachments/assets/788738d5-e1d0-4cea-9808-2008a52992dd)
[📸 Architecture 2](https://github.com/user-attachments/assets/78e4a70b-926e-48f3-87f0-28cf74ef9262)

AuthPin + Biométrique → Traçabilité via API

Logging d'auth centralisé

---

## Bugs Critiques

Quick fix → Marche ? Oui = Doc. Non = Recul analytique

Comprendre avant de fixer
[📸 Voir](https://github.com/user-attachments/assets/bf843bc5-54fa-40f9-b84f-d1cff240ae29)

---

## Optimisations Performance & Stabilité

**Fuites mémoire** → Correction + nettoyage

**Logs critiques** → Ajouté partout où c'est nécessaire

**Migration progressive C → C++** → Remplacement incrémental
