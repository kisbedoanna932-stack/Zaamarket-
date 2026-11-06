# Zaamarket — pack de démarrage

Ce pack contient une base de site web responsive connectée à Supabase.

## Fichiers
- `index.html` : interface du site et connexion Supabase.
- `supabase.sql` : tables, catégories et règles RLS de départ.
- `manifest.webmanifest` et `service-worker.js` : base installable/PWA.
- `assets/icon.svg` : icône simple.

## Installation
1. Dans Supabase, ouvrez Project Settings / API Keys et copiez l'URL du projet ainsi que la clé **Publishable** (`sb_publishable_...`) ou l'ancienne clé `anon`.
2. Dans `index.html`, remplacez `https://VOTRE-PROJET.supabase.co` et `VOTRE_CLE_PUBLIQUE_SUPABASE`.
3. N'insérez jamais une clé `sb_secret_...` ou `service_role` dans le navigateur.
4. Si le projet Supabase est neuf, exécutez `supabase.sql` dans SQL Editor. Si vos tables existent déjà, ne relancez pas le script sans sauvegarde.
5. Envoyez les fichiers à la racine du dépôt GitHub Pages.

## Important
Cette version est un **socle de démarrage**, pas une marketplace prête à encaisser des paiements.
Le panier est local au navigateur. La création de commandes, le calcul sécurisé des montants, les paiements Mobile Money, la livraison, les remboursements, les notifications et les contrôles anti-fraude doivent être ajoutés et testés avant une ouverture au public.
L'approbation de boutiques et de produits nécessite des politiques et fonctions serveur robustes. Les règles RLS de départ ne remplacent pas un audit de sécurité.
