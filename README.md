# SaaS RevPilot — prototype de démonstration

## Fichiers
- `index.html` : application web.
- `saas_ged_data.json` : données fictives de démonstration.

## Déploiement GitHub Pages
Remplacer `index.html` et `saas_ged_data.json` à la racine du dépôt, puis attendre le redéploiement GitHub Pages.

## Fonctionnalités
- Dashboard mensuel en USD.
- Forecast du mois suivant basé sur les dates de service.
- Saisie manuelle de facture et pièce jointe PDF/JPG/PNG (limite de 2 Mo dans ce prototype).
- Import Excel de certains onglets du gabarit.
- Export CSV.

## Limites importantes
- Cette version est un prototype statique, sans base de données ni authentification. Les données de saisie sont stockées dans le navigateur utilisé (localStorage); elles ne sont pas synchronisées entre appareils et peuvent être effacées par le navigateur.
- Les pièces jointes restent en mémoire de session dans cette version et ne doivent pas être considérées comme archivées durablement.
- Le code affiche les montants en USD, mais ne convertit pas automatiquement les factures en EUR/MAD/GBP. Pour les factures en devises autres que USD, un taux de change doit être ajouté avant usage.
- L'import Excel attend des onglets `SAAS SYGED`, `SAAS CSTLO`, `SAAS CSP`; les lignes importées sont supposées en USD. Vérifier les en-têtes et le calcul de reconnaissance avant usage opérationnel.
- Ne pas déposer de factures ou données financières réelles dans un dépôt public.
