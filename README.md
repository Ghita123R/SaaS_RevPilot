# SaaS Revenue — dépôt propre pour démarrer de zéro

Prototype de démonstration pour suivre les revenus SaaS reconnus de SyGED, Constellio et CSP.

## Contenu
- `index.html` : tableau de bord web.
- `saas_ged_data.json` : données de démonstration extraites du classeur fourni.
- `SAAS_GED_Gabarit_Donnees_Fictives.xlsx` : classeur source de démonstration.
- `.gitignore` : exclusions de base.

## Publier dans un nouveau dépôt GitHub privé
1. Sur GitHub, crée un nouveau dépôt avec l’option **Private**.
2. Ne coche pas l’option pour ajouter un README si tu téléverses déjà ce dossier.
3. Décompresse ce ZIP sur ton ordinateur.
4. Dans le nouveau dépôt, clique **Add file → Upload files**.
5. Téléverse le contenu du dossier (les fichiers, pas uniquement le ZIP), puis **Commit changes**.

## Lancer le prototype
Le tableau de bord charge `saas_ged_data.json` avec `fetch`, donc ouvre-le via un serveur web local ou un hébergement configuré, pas simplement par double-clic sur `index.html`.
Pour un test local, dans ce dossier :
`python -m http.server 8000`
Puis ouvre `http://localhost:8000`.

## Limites
- Démonstration uniquement, données fictives.
- Aucun stockage persistant ni synchronisation Microsoft 365 n’est configuré.
- Les chiffres sont repris du classeur; valider les règles de reconnaissance du revenu avant un usage opérationnel.
- Garder le dépôt privé. Pour un déploiement, activer une protection d’accès adaptée.
