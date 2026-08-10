# Guide d'utilisation — Soins Médicaux

Application de gestion de cabinet médical pour iPhone et iPad. Fonctionne intégralement
hors ligne.

## Premier lancement

L'application démarre avec un **jeu de données d'exemple** (5 patients, 8 médecins,
8 types de soins, 15 soins) qui vous permet d'explorer chaque écran immédiatement.

Pour partir d'une base vide : **Plus → Tout effacer**.
Pour retrouver l'exemple : **Plus → Restaurer les données d'exemple**.

## Les cinq onglets

### Accueil

Tableau de bord : nombre de patients, soins enregistrés, soins du mois en cours et revenu
du mois. En dessous, quatre raccourcis (nouveau patient, nouveau soin, recherche,
statistiques) et les cinq derniers soins enregistrés.

### Patients

La liste de vos patients, avec pour chacun son téléphone, son âge et une pastille
indiquant son nombre de soins.

- **Ajouter** — bouton `+` en haut à droite.
- **Rechercher** — champ en bas de l'écran : nom, prénom, téléphone ou adresse.
- **Trier** — bouton en haut à gauche : par nom, par nombre de soins, ou par ordre d'ajout.
- **Supprimer** — balayez la ligne vers la gauche.
- **Ouvrir une fiche** — touchez la ligne.

**La fiche patient** rassemble les coordonnées, le nombre de soins reçus, le montant total,
la répartition par type de soin et l'historique complet. Vous pouvez y modifier le patient,
lui enregistrer un soin directement, ou le supprimer.

> Supprimer un patient supprime aussi tous les soins qui lui sont rattachés.

### Soins

L'historique complet, groupé par mois, avec le total facturé de chaque mois en en-tête.

- **Ajouter** — bouton `+`. Sélectionnez patient, médecin, type de soin, date, et
  éventuellement des notes. La durée et le tarif s'affichent automatiquement.
- **Modifier** — touchez la ligne du soin.
- **Supprimer** — balayez vers la gauche.
- **Rechercher** — par patient, médecin, type de soin ou contenu des notes.

### Recherche

Quatre modes, sélectionnables par les pastilles en haut :

| Mode | Usage |
|---|---|
| **Patient** | Recherche croisée sur nom, prénom, téléphone et adresse. Chaque résultat affiche les derniers soins du patient. |
| **Médecin** | Tous les patients suivis par un médecin donné, avec le détail de leurs soins. |
| **Soins** | Les soins d'un médecin, filtrables par période et par type d'acte. Affiche le nombre de soins, de patients et le revenu correspondant. |
| **Volume** | Analyse par nombre de soins : vue générale, classement des patients ou des médecins, avec bornes minimum et maximum. |

### Plus

Point d'accès à la gestion du cabinet et aux données.

- **Médecins** — ajouter, modifier, supprimer. Chaque fiche indique le nombre de soins
  prodigués, de patients suivis et le revenu généré.
- **Types de soins** — définir les actes, leur durée et leur tarif.
- **Statistiques** — voir ci-dessous.
- **Exporter / Importer** — voir ci-dessous.

> Supprimer un médecin ou un type de soin supprime également les soins associés.
> L'application vous indique combien avant de confirmer.

## Statistiques

Accessible depuis l'Accueil ou l'onglet Plus. On y trouve :

- les chiffres clés et le revenu cumulé ;
- un **graphique d'activité sur 6 mois** ;
- le détail par type de soin (nombre, tarif unitaire, revenu) ;
- le classement des médecins par activité ;
- le détail par patient, sélectionnable dans une liste.

Les montants sont calculés à partir du **tarif actuel** de chaque type de soin. Modifier
un tarif recalcule donc l'historique.

## Sauvegarder et transférer ses données

### Exporter

**Plus → Exporter les données** produit un fichier JSON daté que vous transmettez via la
feuille de partage : AirDrop, app Fichiers, courriel.

Faites-le régulièrement. Les données n'existent que sur votre appareil : sans export, une
perte ou une réinitialisation de l'appareil les fait disparaître définitivement.

> Le fichier exporté n'est pas chiffré. Il contient des données de santé : ne le laissez
> pas traîner sur un service de stockage grand public et ne l'envoyez pas par courriel
> non chiffré.

### Importer

**Plus → Importer un fichier**, puis choisissez un fichier JSON.

> L'import **remplace intégralement** les données présentes. Il ne les complète pas.

### Échanger avec l'application macOS

Le format de fichier est identique à celui de l'application macOS d'origine. Un export
réalisé sur le Mac (⌘E) s'importe sur l'iPhone, et inversement. C'est la façon de reprendre
vos données existantes.

### Transférer entre iPhone et iPad

Les deux installations sont indépendantes et ne se synchronisent pas. Pour transférer :
export d'un côté, AirDrop, import de l'autre.

## Sécurité

L'application n'a ni mot de passe ni verrouillage propre. Sa protection repose sur celle
de l'appareil.

Dans un usage professionnel, configurez impérativement :

- un **code d'accès** et Face ID / Touch ID ;
- un **verrouillage automatique court** (*Réglages → Luminosité et affichage → Verrouillage
  automatique*) ;
- les **mises à jour d'iOS** ;
- des **sauvegardes chiffrées**.

Sans code d'accès, le chiffrement au repos d'iOS ne s'applique pas.

## Questions fréquentes

**L'application fonctionne-t-elle sans connexion ?**
Oui, exclusivement. Elle n'accède jamais au réseau.

**Mes données partent-elles quelque part ?**
Non. Aucun serveur, aucune statistique d'usage, aucun tiers.

**Puis-je l'utiliser sur plusieurs appareils ?**
Oui, mais sans synchronisation automatique : chaque appareil a ses propres données.

**Comment supprimer définitivement toutes les données ?**
*Plus → Tout effacer*, ou désinstallez l'application.

**Puis-je annuler une suppression ?**
Non. Les suppressions sont immédiates et définitives — d'où l'importance des exports.
