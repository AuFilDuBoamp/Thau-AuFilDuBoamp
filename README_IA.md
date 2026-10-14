# README IA — Thau AuFilDuBoamp — dépôt public

## Consignes actuelles — 14 octobre 2026

Après le Pilote, toute consultation GPT se fait **en ligne sur GitHub uniquement**, sur les versions compatibles GPT courantes et historiques. Un lien BOAMP, FTP/HTTPS national, annuaire ou site acheteur n'autorise pas sa consultation. Drive sert séparément à rechercher les originaux, uniquement sur ordre explicite. Sans autorisation supplémentaire, une preuve inaccessible reste `NON ÉTABLI` ; aucun recours automatique au poste, à Drive ou au Web.

Lire la source utile, conserver sa date, son commit et sa provenance. Un index route ; le fichier réellement lu établit le fait. Distinguer `FAIT ÉTABLI`, `OBSERVATION`, `INTERPRÉTATION`, `HYPOTHÈSE`, `NON ÉTABLI`, `ABSENT` et `NON TROUVÉ`. Ne jamais inventer valeur, relation, clé, fichier, URL ou complétude. Une absence n'est ni zéro ni suppression.

Pour un marché Thau, commencer par [le routeur Thau](https://github.com/AuFilDuBoamp/Thau_AuFilDuBoamp_144_preparations_lab/blob/main/GUIDE_IA_BSA_SIRET_THAU.md), puis [le fonds brut cumulatif](https://github.com/AuFilDuBoamp/Thau_AuFilDuBoamp_144_preparations_lab/blob/main/GUIDE_IA_FONDS_CONNAISSANCE_THAU.md). Les schémas courants sont **144 colonnes pivot / 152 liées** ; les anciens 142/143/149/150 restent historiques. La chaîne Thau comprend huit étapes avec 0250 après 0200. [Pilote du 14 octobre : 8/8 OK, sans alerte](https://github.com/AuFilDuBoamp/SIBSARD_PILOTE/blob/main/ETAT_VALIDATION_2026-10-14.md). Ce bilan technique ne certifie ni chaque fait métier ni l'affichage de chaque article.

Les chiffres et résultats datés ci-dessous gardent leur date : ils ne remplacent pas les manifestes actuels. Pour la production, CONFIG et bilans locaux vérifiés déterminent l'état exécutable ; cette règle de maintenance n'autorise aucun accès local pendant une consultation GPT. Les documentations locales republiées doivent être synchronisées avant le prochain Pilote.

## Ordre de reprise

1. `00_LIRE_IA_SIBSARD.md` ;
2. `README.md` ;
3. présent `README_IA.md` ;
4. uniquement les notebooks et actifs utiles au sujet.

## Rôle

Ce dépôt `AuFilDuBoamp/Thau-AuFilDuBoamp` est la **sortie publique** de Thau AuFilDuBoamp.

Il accueille des notebooks et actifs éditoriaux destinés à la diffusion. Il n’est ni le dépôt de préparation interne, ni une source de preuve métier autonome.

## Carte du système utile à une IA

La redondance ci-dessous est volontaire : une IA entrant par ce dépôt public doit comprendre immédiatement d’où viennent les publications.

- orchestration transversale : `AuFilDuBoamp/SIBSARD_PILOTE` ;
- archives JSON BSA et corpus FTP : `AuFilDuBoamp/aufilduboamp_lab_archives_json_bsa_et_ftp_integral` ;
- annonces, identifiants, BSA-SIRET et JSON : `AuFilDuBoamp/aufilduboamp_lab_radar_34_github` ;
- structures eForms : `AuFilDuBoamp/aufilduboamp_lab_eda_eforms` ;
- DCE : `AuFilDuBoamp/aufilduboamp_lab_fonds_documentaire_34_agglo_sete` ;
- préparation privée de Thau 144 : `AuFilDuBoamp/Thau_AuFilDuBoamp_144_preparations_lab` ;
- sources extérieures, méthodes, tutoriels et capitalisation : `AuFilDuBoamp/aufilduboamp_sibsard_reperes` ;
- restitution par acheteur / rubrique 148 : `AuFilDuBoamp/aufilduboamp_lab_radar_34_spip_148` ;
- audit spécialisé du marché `26JA030_MK` : dépôt d’audit dédié ;
- présent dépôt : publications publiques Thau.

Le dossier local de produits Web destinés à publication est `Thau_AuFilDuBoamp_144_publications_web`.

L’ancien dépôt `aufilduboamp_obs_34_agglo_sete` n’est plus une destination de travail GitHub. Les analyses territoriales relèvent de Thau 144 ; les méthodes et capitalisations transversales relèvent de Repères.

## Sources et preuve

Pour vérifier une information publiée ici, revenir aux sources amont :

1. Radar / BSA / BSA-SIRET ;
2. JSON eForms réel si nécessaire ;
3. DCE réellement disponible ;
4. source extérieure autorisée et qualifiée dans Repères ;
5. audit ou analyse comme couche interprétative.

Le présent dépôt, SPIP et les notebooks publics sont des **dérivés de publication**. Ils ne remplacent jamais les sources métier.

## Identité acheteur — règle prioritaire

Pour toute identité juridique affichée dans une publication Thau, utiliser en priorité le **couple BSA / BSA-SIRET établi** :

- **dénomination officielle SIREN/SIRENE** ;
- **numéro SIREN associé**.

Ces deux valeurs doivent rester appariées. Le libellé acheteur et le SIREN provenant de l’annonce BOAMP d’origine sont conservables comme données source, mais ne doivent pas remplacer ce couple lorsqu’il est établi.

Ne jamais fabriquer un hybride en associant une dénomination corrigée issue de BSA/BSA-SIRET à un SIREN BOAMP, ni l’inverse. Le pipeline BSA peut apporter des corrections substantielles à l’identité de l’annonce d’origine.

## Thau 144

La rubrique 144 suit une architecture modulaire **tout en noisettes** :

`sources → traitements métier en amont → JSON/manifestes → FTP → PHP léger → modèles/noisettes → composition éditoriale SPIP`

Les modèles/noisettes Thau sont placés directement dans :

`squelettes/modeles/`

avec le préfixe :

`thau_cent_quarante_quatre_...`

Exemple établi :

`<thau_cent_quarante_quatre_marche_identite|>`

Un `id_article` explicite peut cibler les données d’un autre article.

Les calculs, rapprochements et décisions métier ne doivent pas être reconstruits dans la couche de publication.

## État public vérifié — 6 octobre 2026

Le dépôt public et le dossier local `Thau_AuFilDuBoamp_144_publications_web` sont cohérents sur le périmètre courant :

- 20 radiographies ;
- 20 lignes dans `MANIFESTE_PUBLICATIONS.csv` ;
- 20 IDWEB uniques ;
- 20 fichiers uniques ;
- toutes les entrées au statut `EN_PREPARATION` ;
- `00_ACCUEIL.ipynb` annonce vingt radiographies.

Le dernier ajout du périmètre courant est `26-93200`, article SPIP `25`.

## Publication

La collection GitHub/nbviewer est distincte du pipeline `0900` SPIP/FTP. Lorsque les informations nécessaires sont déjà établies, la maintenance peut être directe et légère dans ce dépôt : `radiographie_<IDWEB>.ipynb`, `MANIFESTE_PUBLICATIONS.csv`, puis `00_ACCUEIL.ipynb` si le sommaire doit évoluer.

Les notebooks et actifs présents ici doivent être nettoyés avant diffusion : aucun secret/token, chemin privé inutile, donnée non publiable, cellule de travail inutile ou détail interne sensible.

## Non-invention

Une information absente ou non établie reste `NON ÉTABLI`, `ABSENT`, `NON TROUVÉ` ou statut explicite équivalent.

Ne jamais compléter une publication publique par supposition.


## Articulation avec le site SPIP — 2 octobre 2026

La collection publique GitHub/nbviewer est maintenue séparément des JSON affichés dans les noisettes SPIP. Le pipeline 0900 Thau publie ces JSON et leur manifeste sur FTP ; il ne met pas à jour les notebooks de ce dépôt. Les fiches **EN PRÉPARATION** restent volontairement à ce stade tant que leur rédaction détaillée n'est pas demandée.

Voir la [procédure de synchronisation Thau](https://github.com/AuFilDuBoamp/Thau_AuFilDuBoamp_144_preparations_lab/blob/main/SYNCHRONISATION_SIBSARD_SPIP.md) pour les responsabilités et contrôles. Une mise à jour des données du site n'implique pas une mise à jour du présent dépôt.


## Illustrations 95 — articulation du 3 octobre 2026

Pour préparer ou publier des illustrations visuelles ou interactives, rejoindre [la composante Illustrations 95](https://github.com/AuFilDuBoamp/aufilduboamp_lab_illustrations_95/blob/main/00_LIRE_IA_SIBSARD.md), dépôt privé `AuFilDuBoamp/aufilduboamp_lab_illustrations_95` et dossier local de même nom. Elle prépare les agrégats en Python et les restitue dans sa version active documentée en SVG statique avec modèles SPIP, sans iframe ; le détail reste dans sa procédure spécialisée. Son pilote local est autonome : elle n’est pas inscrite dans la chaîne transversale. Les méthodes générales restent dans Repères ; les contrats et procédures de publication propres aux illustrations restent dans leur dépôt. L’accès à une documentation privée exige une authentification ou des copies fournies par l’utilisateur.
