# Expériences Techniques

## Sylvamap – 2FA

**Intégration manuelle** vs django-two-factor-auth → Contrôle total, traçabilité sécurité

**Twilio vs Vonage** → 99.99% uptime, communauté

**Django Cache vs PostgreSQL** → Expiration auto 15min

**CharField vs Integer** → Préserve zéros ("001234")

**phone_number + phone_2fa** → Séparation propre, changement phone n'affecte pas 2FA

**Refactoring views** : activate/disable_2fa fusionnées, -50 lignes, DRY

---

## Tests & CI/CD

Tests unitaires + intégration GitHub Actions

---

## Phileas – Mobile API C# & Authentification

App Mobile → API C# Service → BDD

AuthPin + Biométrique → Traçabilité via API

Logging d'auth centralisé

---

## Bugs Critiques

Quick fix → Marche ? Oui = Doc. Non = Recul analytique

Comprendre avant de fixer
