# Fiche App Store — Soins Médicaux

Éléments à reporter dans App Store Connect. Les limites de caractères d'Apple sont
indiquées ; les textes proposés les respectent.

---

## Identité

| Champ | Valeur |
|---|---|
| Nom (30 car. max) | `Soins Médicaux` |
| Sous-titre (30 car. max) | `Cabinet médical, sans serveur` |
| Bundle ID | `com.oulhen.soinsmedicaux` |
| Catégorie principale | **Médecine** |
| Catégorie secondaire | Économie et entreprise |
| Langue principale | Français |
| Prix | À définir |

## Texte promotionnel (170 car. max, modifiable sans nouvelle version)

```
Gérez patients, médecins et soins depuis votre iPhone. Aucun compte, aucun serveur : vos
données restent chez vous, sur vos appareils et dans votre iCloud.
```

## Description

```
Soins Médicaux est un outil de gestion administrative de cabinet médical, conçu pour
aller à l'essentiel. Patients, praticiens, actes et historique des soins : tout est
accessible en quelques touches, et tout reste sur votre appareil.

VOS DONNÉES RESTENT LES VÔTRES

Pas de compte à créer, pas de serveur, pas de mesure d'audience, pas de publicité, aucun
composant tiers. Vos données vivent sur votre appareil et dans votre propre espace iCloud :
rien n'est transmis à l'éditeur ni à qui que ce soit d'autre.

PATIENTS

• Fiches complètes : coordonnées, date de naissance, adresse
• Recherche instantanée par nom, téléphone ou adresse
• Tri par nom, par nombre de soins ou par ordre d'ajout
• Historique des soins et montant total sur chaque fiche

SOINS

• Enregistrement en quelques secondes : patient, praticien, acte, date, notes
• Historique groupé par mois, avec le total facturé de chaque mois
• Modification et suppression à tout moment

CABINET

• Répertoire des médecins avec spécialité et activité détaillée
• Actes personnalisables : libellé, durée, tarif

RECHERCHE

Quatre modes : par patient, par médecin, par période et type d'acte, ou par volume
d'activité avec seuils minimum et maximum.

STATISTIQUES

• Chiffres clés et revenu du mois
• Graphique d'activité sur six mois
• Répartition par type d'acte et classement des praticiens
• Analyse détaillée par patient

SAUVEGARDE ET SYNCHRONISATION

• Sauvegarde automatique dans votre iCloud Drive, avec une archive par jour sur 30 jours
• Vos appareils se tiennent à jour tout seuls : saisissez sur l'iPhone, retrouvez-le sur
  l'iPad, sans rien lancer et sans doublon
• Partage par AirDrop entre deux appareils, avec un écran de revue : rien n'est écrasé,
  vous décidez de ce que vous gardez
• Export de l'intégralité des données en un fichier lisible

CONÇU POUR IOS

Interface native, mode sombre, Dynamic Type, compatible iPhone et iPad.

IMPORTANT

Soins Médicaux est un outil de gestion administrative. Ce n'est pas un dispositif médical :
l'application n'assiste ni le diagnostic ni la décision thérapeutique. En tant que
professionnel de santé, vous restez responsable des données de vos patients et du respect
du secret médical. Pensez à exporter régulièrement une sauvegarde.
```

## Mots-clés (100 car. max, séparés par des virgules, sans espaces)

```
cabinet,médical,patient,soins,praticien,consultation,gestion,icloud,santé,infirmier,libéral
```

## URL requises

| Champ | Valeur |
|---|---|
| URL de support | `https://boboul-cloud.github.io/soins-medicaux/#support` |
| URL de politique de confidentialité | `https://boboul-cloud.github.io/soins-medicaux/#confidentialite` |
| URL marketing | Facultative |

Apple exige une **URL de politique de confidentialité valide et accessible publiquement**
pour toute application. Une page hébergée sur un domaine que vous contrôlez est préférable
à un hébergement temporaire.

---

## Confidentialité des apps (App Privacy)

Réponse à donner dans App Store Connect → *App Privacy* :

> **« Les données ne sont pas collectées »** (*Data Not Collected*)

Cette réponse reste exacte malgré la sauvegarde iCloud. Apple exclut explicitement de la
« collecte » les données que l'application se contente de stocker dans le compte iCloud de
l'utilisateur lui-même : le développeur n'y a aucun accès et n'en reçoit rien. C'est la
réponse attendue pour toute application n'utilisant que la base privée iCloud / CloudKit.

Ne cochez aucune catégorie de données. Aucun SDK tiers n'étant intégré, aucune déclaration
de partenaire n'est requise.

## Classification par âge

Au questionnaire, la seule question susceptible de s'appliquer est celle relative aux
**informations médicales ou de traitement**. L'application affiche des libellés d'actes et
des notes saisies par le praticien, sans contenu médical éditorial.

Réponse suggérée : **Aucun / Aucune**, ce qui conduit à une classification **4+**.
Si vous préférez la prudence, « Peu fréquent / Léger » conduit à 12+. Répondez selon
l'usage réel que vous en faites.

## Notes pour l'équipe de validation (App Review Information)

À coller dans le champ *Notes* — ces précisions évitent les rejets les plus courants pour
ce type d'application :

```
Application de gestion administrative de cabinet médical, fonctionnant sans compte ni
serveur.

• Aucun compte ni identifiant n'est nécessaire. Toutes les fonctionnalités sont
  accessibles immédiatement au lancement.
• Un jeu de données fictives (patients et praticiens inventés) est préchargé au premier
  lancement afin de permettre l'évaluation de toutes les fonctionnalités. Il est
  effaçable via Plus > Tout effacer.
• L'application ne communique avec aucun serveur du développeur et n'intègre aucun SDK
  tiers. Le seul usage du réseau est la sauvegarde du fichier de données dans le
  conteneur iCloud Documents de l'utilisateur (iCloud.com.oulhen.soinsmedicaux), qui sert
  également à synchroniser ses propres appareils. Le développeur n'y a aucun accès.
• Sans compte iCloud ou avec iCloud Drive désactivé, l'application fonctionne normalement
  en local ; l'écran Plus > Sauvegarde iCloud indique alors « Indisponible ».
• Il ne s'agit pas d'un dispositif médical : aucune fonction de diagnostic, de calcul
  clinique ou d'aide à la décision thérapeutique. L'application se limite au suivi
  administratif des actes et à des statistiques d'activité.
• Les données saisies par l'utilisateur sont stockées dans le conteneur privé de
  l'application et protégées par le chiffrement au repos d'iOS.
```

## Ressources visuelles à préparer

| Élément | Exigence |
|---|---|
| Icône | 1024 × 1024 px, sans transparence — déjà présente dans le projet |
| Captures iPhone | 6,9 pouces (1320 × 2868) — obligatoire |
| Captures iPad | 13 pouces (2064 × 2752) — obligatoire si l'app est proposée sur iPad |

Écrans à privilégier : Accueil, Patients, fiche patient, Soins, Statistiques.

---

## Points de vigilance avant soumission

**Directive 5.1.1** — La politique de confidentialité doit être accessible depuis l'URL
déclarée et décrire précisément le traitement des données. Le texte fourni le fait.

**Sauvegarde iCloud** — la capacité *iCloud Documents* suppose un compte développeur payant
et un conteneur `iCloud.com.oulhen.soinsmedicaux` déclaré dans le profil de provisionnement.
La politique de confidentialité décrit cette copie et la synchronisation entre appareils,
ce qu'exige la directive 5.1.1 dès lors que des données quittent l'appareil.

**Directive 1.4.1** — Les applications de santé font l'objet d'un examen renforcé. La
mention explicite de l'absence de qualité de dispositif médical, dans la description
comme dans les notes de validation, réduit sensiblement le risque de rejet.

**Compte de développeur individuel** — L'application sera publiée sous le nom
« Robert Oulhen ». Si vous souhaitez un nom commercial, il faut un compte de type
organisation, qui exige un numéro DUNS.

**Diffusion à d'autres praticiens** — Dès lors que l'application est utilisée par des
tiers, chacun devient responsable de traitement pour ses propres patients. Vous n'avez
accès à aucune donnée, ce qui vous place hors du champ de la sous-traitance au sens du
RGPD : aucun contrat de sous-traitance (article 28) n'est nécessaire.
