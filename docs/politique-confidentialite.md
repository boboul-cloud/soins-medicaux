# Politique de confidentialité — Soins Médicaux

**Dernière mise à jour : 11 août 2026**
**Version de l'application : 1.1**

## En une phrase

L'application Soins Médicaux ne collecte aucune donnée et ne communique avec aucun serveur
de l'éditeur. Tout ce que vous saisissez reste sur votre appareil et, si vous laissez la
sauvegarde active, dans votre propre espace iCloud.

## 1. Qui fait quoi

Cette politique distingue deux rôles, car ils n'ont pas les mêmes obligations.

**L'éditeur de l'application** — Robert Oulhen, éditeur de Soins Médicaux.
L'éditeur ne collecte, ne reçoit, ne consulte et ne conserve **aucune donnée** issue de
l'application. Il n'a techniquement aucun moyen d'accéder à ce que vous y saisissez.

**Vous, professionnel de santé utilisateur** — vous êtes le **responsable de traitement**
au sens du RGPD pour les données de vos patients que vous saisissez dans l'application.
Les obligations qui découlent de ce statut (information des patients, registre des
traitements, sécurité, durées de conservation, réponse aux demandes d'exercice de droits)
vous incombent. La section 7 les détaille.

## 2. Données traitées par l'application

L'application vous permet d'enregistrer :

| Catégorie | Données |
|---|---|
| Patients | Nom, prénom, téléphone, adresse, date de naissance |
| Médecins | Nom, prénom, spécialité, téléphone |
| Types de soins | Libellé, durée, tarif |
| Soins prodigués | Patient, médecin, type de soin, date, notes libres |

Les notes de soins et le lien entre un patient et un acte médical constituent des
**données concernant la santé** au sens de l'article 9 du RGPD. Elles relèvent d'une
catégorie particulière, plus strictement protégée, et sont couvertes par le secret
médical.

## 3. Ce que l'application ne fait pas

L'application ne comporte :

- **aucun serveur de l'éditeur** — elle ne se connecte à aucun service que l'éditeur
  exploite, contrôle ou peut consulter ;
- **aucun compte utilisateur**, aucune authentification, aucune inscription ;
- **aucun outil de mesure d'audience** ni statistique d'usage ;
- **aucune publicité**, aucun traceur, aucun cookie ;
- **aucun kit de développement tiers** (SDK) — le code ne dépend que des bibliothèques
  fournies par Apple ;
- **aucun transfert de données à l'éditeur ni à un tiers destinataire**.

La seule sortie de données hors de l'appareil est la sauvegarde dans **votre propre espace
iCloud Drive**, décrite à la section 4. Elle utilise le réseau, elle est activable et
désactivable par vous, et elle ne va nulle part ailleurs que dans le compte iCloud dont vous
êtes titulaire.

L'éditeur n'hébergeant aucune donnée pour le compte de qui que ce soit, il n'entre pas dans
le champ de la certification **Hébergeur de Données de Santé (HDS)**. Le stockage iCloud
relève de votre propre compte et des conditions que vous avez conclues avec Apple.

## 4. Où sont stockées les données

Les données sont enregistrées dans un fichier unique, `soins-medicaux.json`, situé dans
l'espace privé de l'application sur votre appareil. Cet espace est isolé par iOS : aucune
autre application ne peut y accéder.

**Protection au repos.** iOS chiffre le contenu de cet espace dès que l'appareil est
verrouillé, à condition qu'un **code d'accès soit configuré**. Sans code d'accès, la
protection matérielle d'iOS ne s'applique pas. Configurer un code d'accès, ou Face ID /
Touch ID, est indispensable dans un usage professionnel.

**Sauvegardes.** Si les sauvegardes iCloud ou les sauvegardes locales via un ordinateur
sont activées sur votre appareil, le fichier de données y est inclus, comme pour toute
application. Ces sauvegardes sont chiffrées par Apple. Cela vous protège d'une perte
d'appareil, mais implique qu'une copie des données existe dans votre compte iCloud.
Vous pouvez désactiver la sauvegarde de l'application dans *Réglages → votre nom → iCloud
→ Sauvegarde*.

**Sauvegarde iCloud Drive de l'application.** L'application écrit en outre une copie de vos
données dans **votre** espace iCloud Drive, dossier *Soins Médicaux* : le fichier courant et
une archive par jour sur trente jours. Cette copie existe pour survivre à la désinstallation
de l'application ou à la perte de l'appareil.

**Synchronisation entre vos appareils.** Cette même copie sert à tenir vos appareils à jour :
l'application relit le fichier lorsqu'un autre appareil connecté au même compte iCloud l'a
modifié, et fusionne les deux versions — ajouts, modifications et suppressions — sans
intervention de votre part. Les données circulent donc **dans les deux sens** entre vos
appareils et votre espace iCloud, et uniquement entre eux : elles ne transitent par aucun
service de l'éditeur.

Elle reste sous votre seul contrôle : l'éditeur n'y a aucun accès. Elle est hébergée par
Apple, dans les conditions du compte iCloud dont vous êtes titulaire, et transite chiffrée.
Apple agit ici comme sous-traitant technique de votre propre stockage, non comme
destinataire des données.

Trois conséquences dont vous devez tenir compte en tant que responsable de traitement :

- ces données de santé quittent l'appareil pour l'infrastructure d'Apple ;
- toute personne ayant accès à votre compte iCloud peut lire le dossier *Soins Médicaux*
  depuis l'app Fichiers — protégez ce compte par l'authentification à deux facteurs ;
- activer le **chiffrement de bout en bout** d'iCloud (*Réglages → votre nom → iCloud →
  Protection avancée des données*) place cette copie hors de portée d'Apple elle-même. C'est
  vivement recommandé pour un usage professionnel.

Pour désactiver cette copie, désactivez iCloud Drive pour l'application dans *Réglages →
votre nom → iCloud*. L'application continue alors de fonctionner en local, et l'écran
*Plus → Sauvegarde iCloud* indique `Indisponible`.

**Partage entre appareils.** Le partage par AirDrop transmet un fichier directement d'un
appareil à l'autre, en pair-à-pair, sans passer par aucun serveur. Le fichier transmis
n'est pas chiffré une fois arrivé à destination : ne le partagez qu'avec un appareil dont
vous avez la maîtrise, et supprimez-le du dossier de réception une fois importé.

**Suppression.** Supprimer une fiche dans l'application la supprime sur tous vos appareils
synchronisés : la suppression est propagée avec le reste, et aucun appareil ne la rétablit.
Elle subsiste en revanche dans les **archives quotidiennes** tant que celles-ci n'ont pas
défilé — trente jours au plus.

Désinstaller l'application supprime définitivement le fichier de données local et l'ensemble
de son contenu. **La sauvegarde iCloud Drive, elle, n'est pas supprimée** — c'est sa raison
d'être. Pour l'effacer, supprimez le dossier *Soins Médicaux* dans l'app Fichiers, puis videz
la corbeille d'iCloud Drive.

## 5. Exports

La fonction *Plus → Exporter les données* produit un fichier JSON contenant l'intégralité
de vos données, que vous transmettez ensuite via la feuille de partage d'iOS (AirDrop,
Fichiers, courriel…).

**Ce fichier n'est pas chiffré et son contenu est lisible en clair.** Sa protection relève
entièrement de vous à partir du moment où il quitte l'application. Évitez de l'envoyer par
courriel non chiffré ou de le déposer sur un service de stockage grand public : il contient
des données de santé.

## 6. Absence de dispositif médical

L'application est un outil de **gestion administrative** de cabinet. Elle n'effectue aucun
calcul clinique, ne formule aucune recommandation, n'aide à aucun diagnostic ni à aucune
décision thérapeutique. Elle ne constitue pas un dispositif médical au sens du règlement
(UE) 2017/745 et n'a fait l'objet d'aucun marquage CE à ce titre.

## 7. Vos obligations en tant que responsable de traitement

Si vous utilisez l'application dans le cadre de votre activité professionnelle, il vous
appartient notamment de :

- **informer vos patients** du traitement de leurs données, de sa finalité et de leurs
  droits ;
- **tenir un registre des activités de traitement** (article 30 du RGPD) ;
- **répondre aux demandes d'exercice de droits** — accès, rectification, effacement,
  limitation, portabilité, opposition. L'application vous permet de consulter, modifier,
  supprimer et exporter les données d'un patient, ce qui couvre les besoins techniques
  correspondants ;
- **définir et appliquer des durées de conservation.** L'application ne supprime rien
  automatiquement. Le dossier médical est en principe conservé 20 ans à compter de la
  dernière consultation, mais cette durée dépend de votre situation ; il vous revient de
  la déterminer ;
- **assurer la sécurité de l'appareil** : code d'accès, verrouillage automatique, mises à
  jour d'iOS, chiffrement des sauvegardes ;
- **respecter le secret médical**, en particulier lors des exports.

## 8. Modifications

Toute modification substantielle de cette politique fera l'objet d'une nouvelle version,
identifiée par sa date de mise à jour. Les versions antérieures restent consultables sur
demande.

## 9. Contact

Pour toute question relative à cette politique : **bob.oulhen@gmail.com**

Vous disposez par ailleurs du droit d'introduire une réclamation auprès de la Commission
nationale de l'informatique et des libertés (CNIL), 3 place de Fontenoy, TSA 80715,
75334 Paris Cedex 07 — [www.cnil.fr](https://www.cnil.fr).
