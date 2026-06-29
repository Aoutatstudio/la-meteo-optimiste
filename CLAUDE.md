# Déploiement — La Météo Optimiste

Ce repo (`Aoutatstudio/la-meteo-optimiste`) est connecté à Netlify : https://la-meteo-optimiste.netlify.app

**Règle impérative : toute modification de `index.html` doit être suivie d'un `git push` sur la branche `main` pour que le site en ligne se mette à jour.** Netlify redéploie automatiquement après chaque push sur GitHub, mais ne voit jamais les changements tant qu'ils ne sont pas poussés — éditer le fichier localement ne suffit pas.

`index.html` est le **seul fichier source** (avec `robots.txt` et `sitemap.xml`). Ne pas créer de copie/doublon — ça désynchronise silencieusement le site en ligne de ce qui est édité.

Workflow de push :

```bash
git add index.html
git commit -m "<message>"
git push origin main
```

(Authentification : via token GitHub personnel ou `gh auth login` selon l'environnement. Ne jamais laisser de token en dur dans l'URL du remote une fois le push terminé.)
