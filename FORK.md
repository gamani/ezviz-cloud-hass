# Fork gamani/ezviz-cloud-hass

Fork de [bvis/ezviz-cloud-hass](https://github.com/bvis/ezviz-cloud-hass), basé sur la version officielle **v0.14.0**, avec des modifications locales :

| Commit | Changement |
|---|---|
| `feat(ws)` | Les utilisateurs non administrateurs peuvent regarder le direct |
| `fix(card)` | Le voile de chargement ne repasse plus devant une vidéo déjà lancée |
| `feat(card)` | Bouton plein écran (et double-clic), vidéo centrée |
| `feat(card)` | Bouton Capture : télécharge l'image affichée |
| `feat(card)` | `max_seconds: 0` = direct sans limite de durée |
| `feat(card)` | Option `hd: true` (flux HD) |
| `feat(card)` | Option `background: camera.xxx` : image de fond avant le direct |

## Mettre à jour vers une nouvelle version officielle

```bash
git fetch --depth=50 upstream tag vX.Y.Z
git rebase --onto vX.Y.Z v0.14.0 main   # rejoue les commits du fork sur la nouvelle version
```

Puis ajuster la version dans `manifest.json` et `pyproject.toml` (`X.Y.Z-gamani.1`).
