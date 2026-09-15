# Thau AuFilDuBoamp

**Focus sur une sélection de marchés publics concernant le territoire de Sète Agglopôle Méditerranée, repérés et analysés à partir des sources AuFilDuBoamp établies.**

Ce dépôt public accueille les **publications de Thau AuFilDuBoamp**.

## Porte d’entrée IA

Une IA commence par :

1. `00_LIRE_IA_SIBSARD.md` ;
2. `README.md` ;
3. `README_IA.md` ;
4. seulement ensuite les notebooks ou actifs utiles.

La redondance avec les autres dépôts est volontaire : même depuis ce dépôt public, une IA doit retrouver la carte complète du système et savoir revenir aux sources amont.

## Rôle

Ce dépôt est une **sortie éditoriale publique**. Il n’est ni le dépôt de préparation interne, ni une source de preuve métier autonome.

La préparation est réalisée en amont dans la composante privée :

`AuFilDuBoamp/Thau_AuFilDuBoamp_144_preparations_lab`

Les productions Web locales destinées à la publication sont séparées dans :

`Thau_AuFilDuBoamp_144_publications_web`

## Sources amont

Selon les besoins d’un marché ou d’une publication, la préparation peut s’appuyer sur :

- Radar 34 / BSA / BSA-SIRET pour les annonces, identifiants, identité acheteur et données territoriales ;
- JSON eForms réel lorsque nécessaire ;
- fonds documentaire DCE pour les pièces réellement disponibles ;
- Repères pour les textes, données de référence et autres sources extérieures autorisées ;
- audits spécialisés pour des analyses de cas, sans les substituer aux sources primaires.

Toute information absente ou non établie reste explicitement signalée comme telle.

## Identité acheteur publiée

Pour l’identité juridique d’un acheteur, la publication utilise en priorité le **couple établi dans BSA / BSA-SIRET** :

- **dénomination officielle SIREN/SIRENE** ;
- **numéro SIREN associé**.

Les deux valeurs sont indissociables. Le libellé acheteur et le SIREN présents dans l’annonce BOAMP d’origine peuvent être conservés comme données source, mais ils ne remplacent pas le couple BSA/BSA-SIRET lorsqu’il est établi.

Ne jamais mélanger une dénomination issue de BSA/BSA-SIRET avec un SIREN BOAMP, ni l’inverse. Le pipeline BSA peut corriger ou enrichir substantiellement l’identité de l’annonce d’origine.

## Organisation éditoriale

La rubrique territoriale correspond à **Thau AuFilDuBoamp / rubrique 144**.

La restitution SPIP est construite de manière modulaire : les calculs, rapprochements et analyses sont réalisés en amont ; les objets validés sont ensuite publiés et composés sous forme de modèles/noisettes dans les articles.

Les modèles Thau sont placés directement dans `squelettes/modeles/` sur le site, avec le préfixe `thau_cent_quarante_quatre_...`.

Le site et ce dépôt public ne deviennent jamais des sources de preuve à la place des données et documents qui les alimentent.

## Collection publique

La collection publique est maintenue séparément du pipeline SPIP/FTP. Lorsqu’un marché est ajouté et que ses données sont déjà établies, la mise à jour peut rester légère :

- création ou mise à jour de `radiographie_<IDWEB>.ipynb` ;
- ajout dans `MANIFESTE_PUBLICATIONS.csv` ;
- mise à jour de `00_ACCUEIL.ipynb` lorsque le sommaire évolue.

Cette maintenance directe du dépôt public évite d’ajouter un notebook de fabrication spécifique lorsque ce n’est pas nécessaire.

## État

**Proof of concept éditorial en cours de préparation — publication non encore annoncée.**

La structure comprend un sommaire et un ensemble de radiographies en préparation. Les titres éditoriaux, objets de restitution et contenus détaillés évolueront progressivement à partir de sources établies.

## Lire

Le notebook `00_ACCUEIL.ipynb` constitue le sommaire de la collection lorsqu’il est présent dans la version courante.

Rubrique territoriale : Thau AuFilDuBoamp / rubrique 144.

## Publication et nettoyage

Tout notebook ou actif publié ici doit être réellement nettoyé avant diffusion : aucun secret, token, chemin privé, donnée non publiable, cellule de travail inutile ou détail interne sensible.

## Avertissement

Les documents présents pendant la phase de proof of concept sont susceptibles d’évoluer. Une publication publique reste un dérivé éditorial ; pour une vérification métier, revenir aux sources amont qualifiées.

## Licence

Licence de la collection et conditions de réutilisation : à préciser avant l’annonce publique.
