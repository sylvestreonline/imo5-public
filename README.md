# web-public — pages statiques IMO5

Pages HTML autonomes à héberger sur un sous-domaine public (ex.
`https://imo5.app/privacy`, `https://imo5.app/terms`) pour satisfaire
l'exigence Play Store d'une URL publique de politique de confidentialité.

## Déploiement rapide via GitHub Pages

1. Pousser le repo sur GitHub (déjà fait → `sylvestreonline/imo5`)
2. GitHub.com → **Settings → Pages** du repo
3. **Source** : `Deploy from a branch`
4. **Branch** : `main` + **folder** : `/web-public`
5. **Save**
6. Attendre ~1 min, l'URL est :
   `https://sylvestreonline.github.io/imo5/privacy.html`

Soumettre cette URL à Play Console → App content → Privacy policy.

Plus tard quand le domaine `imo5.app` sera actif : CNAME GitHub Pages
vers `imo5.app` → `https://imo5.app/privacy.html` → URL propre.

## Alternative : Notion / Netlify Drop

Si tu préfères :
- **Notion** : créer une page publique, copier-coller le texte, "Partager
  → publier sur le Web" → URL publique immédiate (ok Play Store).
- **Netlify Drop** : drag & drop du dossier `web-public/` sur
  [app.netlify.com/drop](https://app.netlify.com/drop) → URL immédiate.

## Fichiers

- `privacy.html` — Politique de confidentialité (contenu identique à
  l'écran in-app `lib/features/legal/privacy_screen.dart`).
- `terms.html` — à produire si Play Store demande explicitement un
  lien CGU public (pour l'instant il accepte juste privacy).
