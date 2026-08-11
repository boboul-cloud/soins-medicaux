# Guide d'utilisation — Soins Médicaux

Application de gestion de cabinet médical pour iPhone et iPad. Fonctionne hors ligne ; seules
la sauvegarde et la synchronisation, dans votre propre espace iCloud, utilisent le réseau.

*Version 1.1 de l'application — 11 août 2026.*

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
- **Partager / Recevoir des données** — échange par AirDrop entre appareils, voir ci-dessous.
- **Sauvegarde iCloud** — copie automatique hors de l'application et synchronisation entre
  vos appareils, voir ci-dessous.

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

### Partager entre deux iPhone (AirDrop)

**Plus → Partager mes données**, puis AirDrop et le nom de l'autre appareil. Rapprochez les
deux téléphones, tous deux déverrouillés, Wi-Fi et Bluetooth allumés.

Sur l'appareil qui reçoit, la sauvegarde s'ouvre directement dans Soins Médicaux et affiche
un écran de revue.

### L'écran de revue

C'est le point important : **rien n'est écrasé**. L'écran classe ce qu'il a reçu en quatre
catégories, et vous cochez ce que vous gardez.

| Étiquette | Ce que cela veut dire |
|---|---|
| **Nouveau** | Absent de cet appareil. Coché par défaut. |
| **Mise à jour** | Présent des deux côtés, la version reçue est plus récente. Cochée par défaut. |
| **Conflit** | Modifié des deux côtés, et c'est *votre* version qui est la plus récente. **Décoché** par défaut. |
| **Identiques** | Rien à faire, simplement comptés. |

Touchez le chevron d'une ligne pour voir le détail des différences, champ par champ, avant
et après. Vos patients, médecins et soins qui ne figurent pas dans le fichier reçu ne sont
jamais touchés.

Une dernière section, **Supprimés sur l'autre appareil**, apparaît si l'expéditeur a
supprimé des fiches que vous avez encore. Ces lignes sont toujours décochées : à vous de
décider.

> L'ancien comportement reste disponible : le menu **⋯** en haut à droite propose
> *Tout remplacer par ce fichier*.

### Reprendre un fichier reçu autrement

**Plus → Recevoir des données** ouvre le sélecteur de fichiers, pour une sauvegarde arrivée
par courriel, Messages ou déposée dans l'app Fichiers. Elle passe par le même écran de revue.

### La sauvegarde iCloud, et la synchronisation entre vos appareils

**Plus → Sauvegarde iCloud.**

C'est à la fois la seule copie qui survive à la désinstallation de l'application — le dossier
de l'app est effacé avec elle, celui d'iCloud Drive non — et ce qui tient vos appareils à jour
les uns par rapport aux autres.

- Elle est **automatique** : chaque modification est écrite quelques secondes plus tard.
- Elle est visible dans l'app **Fichiers**, dossier *iCloud Drive → Soins Médicaux*.
- Elle conserve une **archive par jour sur 30 jours**, que vous pouvez comparer et fusionner,
  ou restaurer entièrement.

**Ce qui est écrit par un appareil revient tout seul sur les autres.** Tous ceux qui sont
connectés au même compte iCloud — iPhone, iPad, Mac — suivent le même fichier : un patient
ajouté sur l'iPhone apparaît sur l'iPad quelques instants plus tard, sans rien demander et
sans rien écraser. Les deux versions sont fusionnées fiche par fiche, la plus récemment
modifiée l'emportant, et **les suppressions sont propagées elles aussi** : une fiche effacée
ici disparaît là-bas, elle ne revient pas.

Vous n'avez rien à confirmer : l'écran de revue à cocher est réservé aux fichiers reçus
(AirDrop, app Fichiers, ou une archive que vous comparez), dont l'origine n'est pas connue
d'avance.

L'écran *Sauvegarde iCloud* affiche l'état complet : **Dernière sauvegarde** (le moment où
vos données ont été écrites), **Envoi en cours** tant qu'iCloud n'a pas fini de les
téléverser — c'est seulement une fois cette ligne disparue que les autres appareils peuvent
les voir — et **Dernière réception** (le dernier changement arrivé d'un autre appareil).

Si vous réinstallez l'application, elle repère la sauvegarde au premier lancement et vous
propose de la restaurer avant d'écrire quoi que ce soit.

> Si l'écran indique *Indisponible* : vérifiez dans *Réglages → votre nom → iCloud* que vous
> êtes connecté et qu'iCloud Drive est activé.

> Deux appareils modifiés hors ligne chacun de leur côté se rattrapent dès qu'ils retrouvent
> le réseau. Si la **même fiche** a été modifiée des deux côtés pendant ce temps, c'est la
> modification la plus récente qui est conservée ; l'autre est perdue, sans avertissement.

### Exporter un fichier

**Plus → Exporter pour le Mac** produit un fichier JSON daté, à transmettre par la feuille
de partage.

> Le fichier exporté n'est pas chiffré. Il contient des données de santé : ne le laissez
> pas traîner sur un service de stockage grand public et ne l'envoyez pas par courriel
> non chiffré.

### Échanger avec l'application Mac

L'application Mac partage la **même sauvegarde iCloud** que l'iPhone. Si les deux sont
connectés au même compte iCloud, il n'y a rien à transférer à la main :

- ce que vous saisissez sur l'iPhone part dans iCloud quelques secondes plus tard ;
- le Mac s'en aperçoit et l'intègre de lui-même, sans rien demander ;
- dans l'autre sens, ce que vous saisissez sur le Mac revient sur l'iPhone de la même façon.

*Fichier ▸ Synchroniser avec iCloud* (⌘S) sur le Mac ne sert qu'à ne pas attendre : la
synchronisation a lieu de toute façon.

Les deux applications calculent les identités de fiches de la même façon : un patient créé
sur le Mac et le même patient créé sur l'iPhone ne feront jamais deux fiches. Vous pouvez
échanger autant de fois que vous voulez sans accumuler de doublons.

Le transfert par fichier reste possible — export sur le Mac (⌘E), import sur l'iPhone — pour
les cas où les deux appareils ne partagent pas le même compte iCloud.

> Un export de l'**ancienne** version Mac ne contient pas de date de modification :
> l'application ne peut alors pas savoir laquelle des deux versions est la plus récente, et
> les fiches modifiées des deux côtés apparaissent en **conflit**, à trancher à la main.

### Utiliser plusieurs appareils au quotidien

iPhone, iPad et Mac connectés au même compte iCloud se tiennent à jour tout seuls : saisissez
là où vous êtes, sans vous demander où sont les « vraies » données. Il n'y a rien à lancer.

Pour un échange ponctuel, ou entre **deux comptes iCloud différents** — deux praticiens, un
appareil prêté —, passez par AirDrop : la fusion reconnaît les fiches déjà présentes et n'en
crée pas de doublon, même si vous échangez plusieurs fois de suite.

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
Oui, entièrement. Seules la sauvegarde et la synchronisation iCloud ont besoin du réseau, et
elles rattrapent leur retard dès que la connexion revient.

**Mes données partent-elles quelque part ?**
Dans votre espace iCloud privé, si la sauvegarde est active — et nulle part ailleurs. Aucun
serveur de l'éditeur, aucune statistique d'usage, aucun tiers.

**Puis-je l'utiliser sur plusieurs appareils ?**
Oui, et ils se synchronisent d'eux-mêmes dès qu'ils sont connectés au même compte iCloud :
ajouts, modifications et suppressions circulent dans les deux sens, sans rien demander et
sans créer de doublon. Entre deux comptes iCloud différents, l'échange se fait par AirDrop,
avec l'écran de revue.

**Mes données survivent-elles à la désinstallation de l'application ?**
Seulement si la sauvegarde iCloud est active. Le dossier de l'application est effacé avec
elle ; le dossier iCloud Drive, non.

**J'ai supprimé un patient et il est revenu.**
Cela ne devrait plus arriver : l'application retient ses suppressions et ne les défait pas
lors d'une fusion. Entre appareils synchronisés par iCloud, une suppression est appliquée
partout ; dans un fichier reçu par AirDrop, elle vous est proposée séparément, décochée par
défaut.

**Comment supprimer définitivement toutes les données ?**
*Plus → Tout effacer*, ou désinstallez l'application.

**Puis-je annuler une suppression ?**
Non. Les suppressions sont immédiates et définitives — d'où l'importance des exports.
