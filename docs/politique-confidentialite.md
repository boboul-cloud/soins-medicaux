# Politique de confidentialité — Soins Médicaux

**Dernière mise à jour : 10 août 2026**
**Version de l'application : 1.0**

## En une phrase

L'application Soins Médicaux ne collecte aucune donnée, n'envoie rien sur Internet et ne
communique avec aucun serveur. Tout ce que vous saisissez reste sur votre appareil.

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

- **aucune connexion réseau** — elle fonctionne intégralement hors ligne ;
- **aucun compte utilisateur**, aucune authentification, aucune inscription ;
- **aucun outil de mesure d'audience** ni statistique d'usage ;
- **aucune publicité**, aucun traceur, aucun cookie ;
- **aucun kit de développement tiers** (SDK) — le code ne dépend que des bibliothèques
  fournies par Apple ;
- **aucun transfert de données**, ni vers l'éditeur, ni vers un tiers, ni hors de l'Union
  européenne.

Aucune donnée n'étant hébergée chez un tiers, la certification **Hébergeur de Données de
Santé (HDS)** ne s'applique pas à cette application.

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

**Suppression.** Désinstaller l'application supprime définitivement le fichier de données
et l'ensemble de son contenu. Cette suppression est irréversible et aucune copie ne
subsiste, hors sauvegardes existantes.

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
