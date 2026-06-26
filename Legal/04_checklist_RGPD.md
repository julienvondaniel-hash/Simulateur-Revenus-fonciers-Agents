# Checklist RGPD — avant mise en production

Cochez chaque point. Ceux marqués 🔴 sont **bloquants**.

## Hébergement et sous-traitants
- [ ] 🔴 Projet **Supabase créé dans une région de l'UE** (ex. Frankfurt).
- [ ] 🔴 **DPA signé/accepté** avec Supabase (Data Processing Agreement).
- [ ] 🔴 **DPA signé/accepté** avec Vercel.
- [ ] Vérifier qu'aucun transfert de données hors UE n'a lieu (ou garanties en place).

## Données et minimisation
- [ ] 🔴 Confirmer qu'**aucune donnée nominative de prospect** n'est saisie dans le simulateur.
- [ ] Consigne écrite aux partenaires : « ne saisir que des montants, jamais d'identité ».
- [ ] Durées de conservation paramétrées (purge 24 mois planifiée via pg_cron).
- [ ] Clé `service_role` Supabase **jamais** exposée côté client.

## Information et droits
- [ ] 🔴 **Mentions légales** publiées (compléter `01_mentions_legales.md`).
- [ ] 🔴 **Politique de confidentialité** publiée et accessible depuis l'app.
- [ ] Information des partenaires sur la journalisation de leurs accès.
- [ ] Point de contact pour l'exercice des droits (e-mail dédié).
- [ ] **Registre des traitements** tenu à jour (`03_registre_traitements.md`).

## Sécurité technique
- [ ] HTTPS actif (automatique sur Vercel).
- [ ] RLS activée et testée (un partenaire ne voit pas les données d'un autre).
- [ ] Politique de mots de passe robustes pour les comptes partenaires.
- [ ] Procédure de révocation d'accès documentée (désactiver/supprimer un partenaire).

## Activité réglementée (CGP)
- [ ] 🔴 Mention claire « outil d'aide à la décision, pas un conseil personnalisé ».
- [ ] Numéro **ORIAS** et statut affichés dans les mentions légales.
- [ ] Vérifier les obligations spécifiques **AMF/ACPR** liées à la diffusion d'outils
      de simulation à des partenaires.

## Validation finale
- [ ] 🔴 **Relecture par un juriste / avocat** des documents `legal/` avant publication.
- [ ] Test complet : connexion, déconnexion, accès refusé (compte désactivé/expiré),
      enregistrement d'une simulation, cloisonnement entre 2 partenaires.

---

> Ce document est un guide pratique, pas un avis juridique. La conformité finale
> relève de votre appréciation et de celle de votre conseil.
