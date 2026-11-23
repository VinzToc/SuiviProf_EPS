# SuiviProf EPS (prototype v0.3)
Carnet de suivi des séances d'EPS intégré à Mes Apps EPS (identifiant d'application : `suiviprof`).
- Une classe = un classeur ; un onglet par cycle + un onglet Bilan automatique.
- Une séance = un groupe de colonnes daté. Par défaut : Appel, Tenue, Dispense, Infirmerie, Comportement (même largeur), puis les colonnes ajoutées (équipe, temps, distance, nombre/note, calcul, texte).
- Page 📅 Organisation : année scolaire et zone (calendrier officiel 2026-2027 intégré, mise à jour en ligne depuis data.education.gouv.fr), jours fériés calculés (option Alsace-Moselle), périodes interruptives par classe, trimestres/semestres, semaines A/B avec bascules.
- Par classe : créneaux (jour, horaires, toutes semaines / A / B), évaluation par trimestres ou semestres, cycles à dates indépendantes rattachés à un ou plusieurs créneaux, répartition automatique en N cycles, génération des séances (les séances déjà saisies sont conservées).
- Séances à venir repliées et grisées ; séance annulable avec motif ; bilan filtrable par période.
- Enregistrement dans Mes Apps EPS en mode « lignes » (une ligne par élève et par séance : Date, Cycle, Séance, Appel, Tenue, Infirmerie, Dispense, Comportement, Équipe, Mesures, Observations).

Dépôt : `VinzToc/SuiviProf_EPS`, publié sur https://vinztoc.github.io/SuiviProf_EPS/ (GitHub Pages).
Ajouter la ligne de `apps.json-ligne.txt` dans `apps.json` du portail.
