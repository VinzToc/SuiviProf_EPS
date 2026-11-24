# SuiviProf EPS (v0.9.0)
Carnet de suivi des séances d'EPS intégré à Mes Apps EPS (identifiant d'application : `suiviprof`).
- Une classe = un classeur ; un onglet par cycle + un onglet Bilan automatique.
- Une séance = un groupe de colonnes daté. Par défaut : Appel, Tenue, Dispense, Infirmerie, Comportement (même largeur), puis les colonnes ajoutées (équipe, temps, distance, nombre/note, calcul, texte).
- Page 📅 Organisation : année scolaire et zone (calendrier officiel 2026-2027 intégré, mise à jour en ligne depuis data.education.gouv.fr), jours fériés calculés (option Alsace-Moselle), périodes interruptives par classe, trimestres/semestres, semaines A/B avec bascules.
- Par classe : créneaux (jour, horaires, toutes semaines / A / B), évaluation par trimestres ou semestres, cycles à dates indépendantes rattachés à un ou plusieurs créneaux, répartition automatique en N cycles, génération des séances (les séances déjà saisies sont conservées).
- Cycles nommés par APSA (liste reprise de Gestion AS Pronote) avec leur champ d'apprentissage (CA1 à CA5), proposé automatiquement et modifiable.
- Bilan « Parcours par champ d'apprentissage » : séances pratiquées par élève et par CA, CA non programmés signalés.
- Séances à venir repliées et grisées ; séance annulable avec motif ; bilan filtrable par période.
- Colonne « 🧩 Grille CompEval » : grilles d'évaluation par compétences lues dans CompEval (clé `compeval_v1` du navigateur, même adresse vinztoc.github.io) ou importées (.json exporté par CompEval). La grille est copiée dans la colonne ; évaluation élève par élève, note calculée comme dans CompEval.
- Enregistrement dans Mes Apps EPS en mode « lignes » (une ligne par élève et par séance : Date, Cycle, Séance, Appel, Tenue, Infirmerie, Dispense, Comportement, Équipe, Mesures, Observations).

Dépôt : `VinzToc/SuiviProf_EPS`, publié sur https://vinztoc.github.io/SuiviProf_EPS/ (GitHub Pages).
Ajouter la ligne de `apps.json-ligne.txt` dans `apps.json` du portail.

## Programmation d'équipe (CoordoEPS)
- Organisation annuelle → « 📥 Importer la programmation d'équipe » : fichier `.json` produit par CoordoEPS (application du coordonnateur), ou directement depuis CoordoEPS ouvert dans le même navigateur.
- Choix de l'enseignant (classes cochées automatiquement, créneaux filtrés dans les classes partagées), reprise du calendrier de l'équipe, génération des séances.
- Créneaux importés marqués `pg:1` (id du coordonnateur), cycles importés marqués `pg:<id du cycle CoordoEPS>` : un réimport met à jour sans dupliquer ; cycles retirés supprimés seulement s'ils n'ont aucune saisie.
