# Fiche App Store — Soins Médicaux

Éléments à reporter dans App Store Connect. Les limites de caractères d'Apple sont
indiquées ; les textes proposés les respectent.

---

## Identité

| Champ | Valeur |
|---|---|
| Nom (30 car. max) | `Soins Médicaux` |
| Sous-titre (30 car. max) | `Gestion de cabinet hors ligne` |
| Bundle ID | `com.oulhen.soinsmedicaux` |
| Catégorie principale | **Médecine** |
| Catégorie secondaire | Économie et entreprise |
| Langue principale | Français |
| Prix | À définir |

## Texte promotionnel (170 car. max, modifiable sans nouvelle version)

```
Gérez patients, médecins et soins depuis votre iPhone. Aucun compte, aucun serveur :
vos données restent sur votre appareil.
```

## Description

```
Soins Médicaux est un outil de gestion administrative de cabinet médical, conçu pour
aller à l'essentiel. Patients, praticiens, actes et historique des soins : tout est
accessible en quelques touches, et tout reste sur votre appareil.

VOS DONNÉES NE QUITTENT PAS VOTRE IPHONE

L'application fonctionne intégralement hors ligne. Pas de compte à créer, pas de serveur,
pas de mesure d'audience, pas de publicité, aucun composant tiers. Rien n'est transmis à
qui que ce soit, y compris à l'éditeur.

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

SAUVEGARDE

Export de l'intégralité des données en un fichier lisible, transmissible par AirDrop,
Fichiers ou courriel. Import tout aussi simple pour restaurer ou changer d'appareil.

CONÇU POUR IOS

Interface native, mode sombre, Dynamic Type, compatible iPhone et iPad.

IMPORTANT

Soins Médicaux est un outil de gestion administrative. Ce n'est pas un dispositif médical :
l'application n'assiste ni le diagnostic ni la décision thérapeutique. En tant que
professionnel de santé, vous restez responsable des données de vos patients et du respect
du secret médical. Les données étant stockées uniquement sur votre appareil, pensez à
exporter régulièrement une sauvegarde.
```

## Mots-clés (100 car. max, séparés par des virgules, sans espaces)

```
cabinet,médical,patient,soins,praticien,consultation,gestion,agenda,santé,infirmier,libéral
```

## URL requises

| Champ | Valeur |
|---|---|
| URL de support | *(page web — voir `site/index.html`)* |
| URL de politique de confidentialité | *(même page, ancre `#confidentialite`)* |
| URL marketing | Facultative |

Apple exige une **URL de politique de confidentialité valide et accessible publiquement**
pour toute application. Une page hébergée sur un domaine que vous contrôlez est préférable
à un hébergement temporaire.

---

## Confidentialité des apps (App Privacy)

Réponse à donner dans App Store Connect → *App Privacy* :

> **« Les données ne sont pas collectées »** (*Data Not Collected*)

Cette réponse est exacte : l'application ne transmet aucune donnée hors de l'appareil.
Les données saisies par l'utilisateur restent locales, ce qui ne constitue pas une
« collecte » au sens de la définition d'Apple.

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
Application de gestion administrative de cabinet médical, fonctionnant intégralement
hors ligne.

• Aucun compte ni identifiant n'est nécessaire. Toutes les fonctionnalités sont
  accessibles immédiatement au lancement.
• Un jeu de données fictives (patients et praticiens inventés) est préchargé au premier
  lancement afin de permettre l'évaluation de toutes les fonctionnalités. Il est
  effaçable via Plus > Tout effacer.
• L'application n'effectue aucune requête réseau. Elle ne collecte, ne transmet et
  n'héberge aucune donnée. Aucun SDK tiers n'est intégré.
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
