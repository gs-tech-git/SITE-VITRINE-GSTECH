# GSTech — site vitrine

Site institutionnel GSTech construit avec React 19 et Vite. Il présente les trois pôles de services, les applications SamaGP et CyberSentinels, et prépare les parcours contact/devis, actualités et réalisations.

## Démarrage

Le dépôt utilise Bun et un monorepo Turborepo. Depuis sa racine :

```bash
bun install
bun run dev
```

Pour compiler le site web : `bun run build:web`. Les scripts complets sont décrits dans [packages/web/README.md](packages/web/README.md).

## Organisation du site

- `packages/web/src/web/app.tsx` : routes React et métadonnées.
- `packages/web/src/web/pages/` : pages et parcours du site.
- `packages/web/src/web/content/site.ts` : données de services, applications, articles et références.
- `packages/web/src/web/components/` : navigation, pied de page et consentement cookies.
- `packages/web/public/images/gstech-logo.jpeg` : logo fourni par GSTech.
- `packages/web/SECURITY.md` : exigences de sécurité et éléments à compléter avant publication.

Le front-end est un squelette éditorial. Les formulaires ne transmettent aucune donnée. Les articles et études de cas attendent un CMS et des contenus approuvés; les textes juridiques, coordonnées, liens des stores et choix d’hébergement restent à fournir.

## Configuration avant production

Renseigner `VITE_SITE_URL` avec le domaine HTTPS réel pour générer `sitemap.xml` et `robots.txt`. Compléter le consentement, l’outil d’e-mailing, le CMS, les en-têtes de sécurité, les sauvegardes et la configuration DNS selon l’hébergement retenu.
# SITE-VITRINE-GSTECH
