# README IA — Thau AuFilDuBoamp — dépôt public

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

## Publication

Les notebooks et actifs présents ici doivent être nettoyés avant diffusion : aucun secret/token, chemin privé inutile, donnée non publiable, cellule de travail inutile ou détail interne sensible.

## Non-invention

Une information absente ou non établie reste `NON ÉTABLI`, `ABSENT`, `NON TROUVÉ` ou statut explicite équivalent.

Ne jamais compléter une publication publique par supposition.
