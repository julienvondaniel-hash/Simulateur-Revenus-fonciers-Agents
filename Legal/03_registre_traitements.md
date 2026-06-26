# Registre des activités de traitement (art. 30 RGPD)

> Document interne, obligatoire, **non publié**. Tenu à jour par le responsable.
> Dernière mise à jour : 26/06/2026

## Responsable du traitement

- **Seine Gestion Privée** (SASU, marque HEXA Patrimoine) — SIREN 999 826 191
- 44 rue Jean Mermoz, 78600 Maisons-Laffitte
- Représentant : Julien DANIEL, président
- Contact : **j.daniel@hexa-patrimoine.com** — 06 58 80 36 30
- DPO : **aucun DPO désigné** (désignation non obligatoire). Responsable : Julien DANIEL, président.

---

## Traitement n°1 — Gestion des accès partenaires

- **Finalité** : authentifier et gérer les partenaires autorisés à utiliser le simulateur.
- **Catégories de personnes** : partenaires (agences immobilières et collaborateurs).
- **Catégories de données** : e-mail professionnel, mot de passe (haché), nom, agence/société, statut (actif/expiré).
- **Base légale** : intérêt légitime / relation contractuelle partenaire.
- **Destinataires** : Seine Gestion Privée (admin), Supabase (sous-traitant, UE-Irlande), Vercel (sous-traitant).
- **Transferts hors UE** : hébergement en UE (Irlande) ; **[À COMPLÉTER : garanties Vercel]**.
- **Durée de conservation** : durée de la relation + 24 mois.
- **Sécurité** : mots de passe hachés, RLS, accès admin restreint, HTTPS.

## Traitement n°2 — Journalisation des accès

- **Finalité** : sécurité, contrôle des accès, suivi d'activité des partenaires.
- **Catégories de données** : identifiant partenaire, date/heure, type d'événement (connexion/déconnexion/inscription). **Aucune adresse IP.**
- **Base légale** : intérêt légitime (sécurité, suivi).
- **Durée de conservation** : 24 mois.
- **Sécurité** : idem traitement n°1.

## Traitement n°3 — Simulations anonymes

- **Finalité** : amélioration de l'outil, statistiques d'usage.
- **Catégories de données** : montants saisis et résultats (**anonymes**).
- **Particularité** : **aucune donnée identifiant un prospect** n'est collectée. Les partenaires s'engagent par les CGU à ne saisir que des montants.
- **Base légale** : intérêt légitime.
- **Durée de conservation** : 24 mois.

---

> ⚠️ Si des **données de prospects identifiables** venaient à être saisies par un
> partenaire en violation des CGU, ce partenaire en serait le **responsable de
> traitement** distinct. Si Seine Gestion Privée décidait un jour de collecter
> volontairement de telles données, créer un **traitement n°4** dédié (base
> légale, information des personnes, durée propre) et réévaluer la nécessité
> d'une **analyse d'impact (AIPD)**.
