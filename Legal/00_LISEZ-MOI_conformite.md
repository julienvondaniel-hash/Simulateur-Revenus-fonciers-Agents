# ⚠️ À LIRE AVANT MISE EN LIGNE — Conformité

Ces documents sont des **MODÈLES** destinés à être **complétés puis validés par
un juriste / avocat** (idéalement spécialisé en données personnelles et en
réglementation des CGP). **Ils ne constituent pas un conseil juridique** et ne
vous couvrent pas en l'état.

## Ce que stocke réellement l'application (à confirmer)

1. **Comptes partenaires** : e-mail professionnel + mot de passe (géré par
   Supabase Auth, mot de passe haché). → donnée personnelle *professionnelle*.
2. **Journal d'accès** (`access_logs`) : connexions/déconnexions, date/heure,
   éventuellement IP tronquée et navigateur. → donnée personnelle *professionnelle*.
3. **Simulations anonymes** (`simulations`) : montants saisis et résultats,
   **sans aucune identité de prospect** (pas de nom, e-mail, téléphone).

> 🔴 **Règle d'or** : ne JAMAIS saisir dans le simulateur le nom, les coordonnées
> ou tout élément identifiant un prospect. Tant que c'est respecté, les
> simulations restent anonymes et le risque RGPD reste limité aux comptes
> partenaires. Si vous décidez d'y mettre des données de prospects, vous changez
> de régime juridique (voir checklist).

## Points à trancher avec votre juriste

- **Responsable de traitement** : HEXA Patrimoine (à confirmer : raison sociale
  exacte, SIREN, représentant légal).
- **Base légale** des traitements (intérêt légitime pour les logs partenaires ?).
- **Sous-traitants** : Vercel (hébergement applicatif) et Supabase (base de
  données / auth). Vérifier leurs **DPA** (Data Processing Agreement) et la
  **localisation des données** (choisir une région **UE** chez Supabase).
- **Information des partenaires** : les prévenir que leurs accès et leur activité
  sont journalisés (transparence).
- **Durée de conservation** : 24 mois proposés (modifiable).
- **Droits** : accès, rectification, effacement — prévoir un point de contact.

## Fichiers de ce dossier

- `01_mentions_legales.md` — mentions légales du site.
- `02_politique_confidentialite.md` — politique de confidentialité (RGPD).
- `03_registre_traitements.md` — registre des activités de traitement (art. 30).
- `04_checklist_RGPD.md` — checklist pratique avant mise en production.
- `05_conditions_generales_utilisation.md` — CGU partenaires (responsabilité des données saisies).

## État de complétion (généré le 26/06/2026)

**Renseigné :** SASU Seine Gestion Privée (marque HEXA Patrimoine) · SIRET
999 826 191 00010 · RCS Versailles · capital 1 000 € · TVA FR62 999 826 191 ·
président Julien DANIEL · ORIAS 26004342 (CIF Anacofi-CIF, IAS, carte T) ·
siège 44 rue Jean Mermoz 78600 Maisons-Laffitte · hébergement Vercel + Supabase
(UE-Irlande) · conservation 24 mois · aucune IP enregistrée · aucun traceur.

**Champs restant à compléter ([À COMPLÉTER] dans les fichiers) :**
1. **DPA** Supabase et Vercel : confirmer acceptation + garanties de transfert Vercel.

**Résolu :** DPO = aucun (responsable : Julien DANIEL, président). Les mentions
de **garantie financière** et de **RC Pro** ont été retirées : le simulateur est
positionné comme un **outil pédagogique, non contractuel, ne constituant pas un
conseil**.

