# À LIRE PAR TOUTE IA — Socle transversal SIBSARD

## 1. Statut transversal

Ce fichier est un **socle transversal volontairement répliqué** dans les composantes SIBSARD afin qu’une IA retrouve la carte du système quelle que soit sa porte d’entrée GitHub.

Cette redondance est voulue. Les copies doivent rester cohérentes. Elle ne remplace ni le référentiel général `AuFilDuBoamp/aufilduboamp-ia`, ni les README et contrats spécialisés de chaque composante.

Pour tout travail substantiel : lire d’abord le référentiel général, puis ce socle, les README/procédures de la composante, ses fichiers courants et enfin le briefing utilisateur.

Pour la reprise documentaire, GitHub peut être plus frais qu’une copie locale. Pour l’état exécutable réel, les fichiers locaux courants prévalent pour notebooks, CONFIG, résultats, secrets et fichiers de travail. Toute divergence GitHub/local doit être signalée, jamais corrigée par supposition.

## 2. Carte courante

- `AuFilDuBoamp/SIBSARD_PILOTE` — orchestration transversale des maîtres autorisés, journalisation et bilan global ; hors pipeline propriétaire de production du BSA.
- `AuFilDuBoamp/aufilduboamp_lab_archives_json_bsa_et_ftp_integral` — maintenance technique des archives JSON BSA et corpus FTP autorisés.
- `AuFilDuBoamp/aufilduboamp_lab_eda_eforms` — référentiel spécialisé pour comprendre prudemment les structures eForms observées.
- `AuFilDuBoamp/aufilduboamp_lab_radar_34_github` — annonces, BSA-SIRET territorial, identifiants, index et JSON ; point de départ des analyses de marchés du Radar.
- `AuFilDuBoamp/aufilduboamp_lab_fonds_documentaire_34_agglo_sete` — fonds DCE ; dérivés légers traçables sur GitHub, originaux locaux/Drive lorsque nécessaires.
- `AuFilDuBoamp/Thau_AuFilDuBoamp_144_preparations_lab` — composante privée de préparation de **Thau AuFilDuBoamp** : sélection territoriale, rapprochements, identité acheteur, analyses, radiographies, objets de publication et préparation des restitutions de la rubrique 144.
- `AuFilDuBoamp/aufilduboamp_sibsard_reperes` — sources extérieures autorisées, textes juridiques, données de référence, méthodes, tutoriels, vocabulaire et capitalisation transversale.
- `AuFilDuBoamp/aufilduboamp_lab_radar_34_spip_148` — restitution par acheteur de la rubrique 148 ; composante technique distincte dont l’architecture modulaire JSON/manifeste/FTP/PHP/modèles sert de référence utile. Sa priorité éditoriale est actuellement rétrogradée, mais son statut dans le Pilote dépend exclusivement du registre exécutable.
- `AuFilDuBoamp/COMMUNE-DE-SETE-19-10-2026-Tonte-et-entretien-des-espaces-plantes-B-26-70532-S-213403017` — audit spécialisé du marché espaces verts de Sète.
- `AuFilDuBoamp/Thau-AuFilDuBoamp` — dépôt **public** des publications Thau ; sortie éditoriale, jamais source de preuve métier.

Espaces locaux distincts :

- préparation privée : `Thau_AuFilDuBoamp_144_preparations_lab` ;
- produits Web immédiatement publiables : `Thau_AuFilDuBoamp_144_publications_web`.

Le répertoire FTP de publication Thau porte également le nom `Thau_AuFilDuBoamp_144_publications_web`, mais il s’agit d’un espace distant distinct du dossier local de publications.

L’ancien dépôt `aufilduboamp_obs_34_agglo_sete` n’est plus une composante GitHub courante. Les fonctions opérationnelles ont été réparties entre Thau 144 et Repères. Une mention dans un document ancien peut être conservée comme provenance historique, mais ce dépôt ne doit plus être proposé comme destination de travail.

## 3. Chaîne Pilote

Ordre fonctionnel courant documenté :

`Archives → eForms → Radar → DCE → SPIP 144 → Repères → SPIP 148`

L’identifiant fonctionnel `SPIP 144` du Pilote correspond désormais au dossier local `Thau_AuFilDuBoamp_144_preparations_lab`.

SPIP 148 reste, tant que le registre exécutable courant le confirme, la dernière composante active et bloquante. Le DCE est non bloquant au niveau transversal. **Le registre local `SIBSARD_PILOTE/CONFIG/chaine_sibsard.json` prévaut toujours** pour ordre, activation, chemins, maîtres et caractère bloquant.

Lancer le Pilote peut déclencher de vrais effets GitHub, Drive, FTP ou HTTP. Toujours annoncer cette portée.

## 4. Routage

- orchestration, états transversaux, ordre d’exécution : Pilote ;
- archives JSON BSA et corpus FTP : Archives ;
- annonce, identifiant, BSA-SIRET, routage JSON d’un marché : Radar ;
- structure eForms : eForms, puis JSON réel du marché si nécessaire ;
- RC, CCAP, CCTP, BPU, DQE et autres DCE : fonds documentaire ;
- texte juridique, site, donnée de référence, documentation ou autre source extérieure : Repères ;
- marché `26JA030_MK` : audit spécialisé ;
- analyse territoriale, radiographie, préparation éditoriale et objets de publication Thau : `Thau_AuFilDuBoamp_144_preparations_lab` ;
- publication publique des notebooks et actifs Thau : `Thau-AuFilDuBoamp` ;
- restitution par acheteur / rubrique 148 : SPIP 148.

Une question composite se traite couche par couche dans les sources compétentes.

## 5. Thau 144 et architecture de restitution

Thau 144 est la priorité éditoriale courante. Le périmètre vise les annonces concernant le territoire de Sète Agglopôle Méditerranée, avec liaison contrôlée des avis, rectificatifs et attributions d’un même marché.

La préparation privée est le goulot de contrôle : sélection, rapprochements, identité juridique de l’acheteur, cohérence, provenance, analyse éditoriale, fabrication des JSON/objets SPIP et productions publiques nettoyées.

L’identité acheteur repose sur le SIREN et la dénomination officielle établie ; le libellé publié dans une annonce reste une information distincte.

Architecture éditoriale cible :

`sources qualifiées → traitements/analyses en amont → objets stables → JSON + manifestes → FTP → PHP commun léger → modèles/noisettes SPIP → composition éditoriale libre`

La rubrique 144 est **tout en noisettes** : le squelette d’article ne doit pas imposer un chapo ou un corps métier automatique. Les articles composent explicitement les modèles nécessaires.

PHP/SPIP ne doit pas devenir un moteur métier parallèle : calculs, agrégations, rapprochements et décisions restent dans les notebooks ou traitements de préparation. SPIP lit et restitue des contrats validés.

## 6. Discipline de preuve

Pour une information de marché :

1. BSA / BSA-SIRET / Radar ;
2. eForms / JSON réel ;
3. DCE réellement disponible ;
4. source extérieure autorisée et qualifiée dans Repères ;
5. audit ou restitution comme analyse, jamais comme substitut automatique aux sources.

Les profils eForms ne remplacent pas le JSON réel. Un dérivé DCE ne remplace pas l’original lorsqu’une transformation peut avoir perdu l’information nécessaire. SPIP, le dépôt public Thau et les notebooks publics de restitution ne sont jamais des sources de preuve métier.

Distinguer : `FAIT ÉTABLI`, `OBSERVATION`, `INTERPRÉTATION`, `HYPOTHÈSE`, `NON ÉTABLI`, `ABSENT`, `NON TROUVÉ`, `À VÉRIFIER`.

Ne jamais compléter une donnée absente ni forcer la concordance de sources divergentes.

## 7. Repères et sources extérieures

Repères est le réceptacle par défaut des nouvelles sources extérieures et de la documentation transversale. Une source reste ailleurs seulement si une nécessité fonctionnelle, probatoire ou technique documentée l’exige.

Cette centralisation ne vaut pas autorisation générale de consulter Internet. Aucune recherche Web ou source extérieure non prévue sans demande explicite ou autorisation documentée.

## 7 bis. État documentaire vérifié au 22 septembre 2026

- Thau 144 : **18 marchés / 18 articles SPIP** et 18 radiographies dans le dépôt public.
- Identité acheteur : couple **dénomination officielle + SIREN** issu en priorité de BSA/BSA-SIRET ; contrôle de second niveau dans Repères/Insee-Sirene si nécessaire.
- Repères : bibliothèque documentaire `SOURCES/`, avec ordre `README_SOURCE → manifeste → TXT → PDF original si nécessaire`.
- DCE : lecture spécialisée `README_DCE → manifeste → dérivés → original`, avec `DOSSIER-THAU/` comme vue de travail.
- Pilote : sept composantes actives dans la CONFIG locale vérifiée ; SPIP 148 reste active, dernière et bloquante malgré sa priorité éditoriale rétrogradée.
- Audit `26JA030_MK` : dépôt courant `AuFilDuBoamp/COMMUNE-DE-SETE-19-10-2026-Tonte-et-entretien-des-espaces-plantes-B-26-70532-S-213403017`.
- Espaces Thau distincts : préparation privée, `publications_web` local, FTP et dépôt GitHub public.

## 8. Gouvernance et confidentialité

Ne jamais inventer structure, clé, chemin, identifiant, lien, contenu, relation ou règle métier.

Distinguer architecture cible et état réel. Vérifier les productions avant livraison. Conserver les redondances documentaires voulues.

Validation humaine avant suppression importante, écrasement d’un travail validé, réorganisation majeure, changement de visibilité, publication externe non prévue ou réécriture d’historique.

Ne jamais divulguer pipeline propriétaire BSA, méthodes sensibles, règles confidentielles de rapprochement, secrets, tokens, BSA-SIRET national complet, archives nationales non publiables ou composants confidentiels.

## Convention documentaire commune — 24 septembre 2026

### Repères = source canonique des connaissances générales

Le dépôt `AuFilDuBoamp/aufilduboamp_sibsard_reperes` est la **source canonique unique** pour les connaissances générales réutilisables :

- méthodes, tutoriels et vocabulaire ;
- sources extérieures autorisées et règles de provenance ;
- Code de la commande publique et documentation Légifrance ;
- grille chronologique CCP de classement des faits marché ;
- références Insee / Sirene ;
- DUME, données essentielles et Chorus Pro ;
- autres capitalisations transversales.

Une composante spécialisée conserve ses **preuves, données, contrats et procédures propres**. Elle ne doit pas recopier une documentation générale déjà tenue dans Repères, sauf nécessité fonctionnelle, probatoire ou technique explicitement documentée.

### Classement CCP des faits marché

Pour toute analyse d'un marché :

1. établir d'abord le fait dans la source compétente : Radar, JSON eForms réel, DCE, source extérieure qualifiée, etc. ;
2. conserver la provenance et le statut de preuve dans la composante source ou l'étude de cas ;
3. si le fait doit être structuré dans la vie du marché, lire :
   `AuFilDuBoamp/aufilduboamp_sibsard_reperes/CAPITALISATION/CCP_CHRONOLOGIE_MARCHE/00_LIRE_IA_CCP.md` ;
4. appliquer la rubrique CCP sans déplacer ni dupliquer la preuve.

Le Code officiel est documenté sous :
`SOURCES/DILA/LEGIFRANCE/CODE_COMMANDE_PUBLIQUE/`.

### Audit Sète

Le dépôt `COMMUNE-DE-SETE-19-10-2026-Tonte-et-entretien-des-espaces-plantes-B-26-70532-S-213403017` est une **étude de cas consommatrice de Repères**.

Il conserve les preuves et constats propres au marché `26JA030_MK`. Ses besoins généraux doivent être satisfaits depuis Repères selon `DEPENDANCES_REPERES.md`, sans recréer de glossaire, tutoriel, source juridique ou grille CCP parallèle.

### Règle de reprise GPT

Quelle que soit la porte d'entrée :

`00_LIRE_IA_SIBSARD.md → README.md → README_IA.md → procédure spécialisée utile → Repères seulement si besoin transversal`.

Ne pas charger en masse les autres dépôts. Router la question vers la composante compétente puis lire uniquement les fichiers nécessaires.

## Point d'entrée marché Thau — convention commune du 26 septembre 2026

Pour tout travail portant sur un **marché du périmètre Thau**, la composante
`AuFilDuBoamp/Thau_AuFilDuBoamp_144_preparations_lab` devient le **point d'entrée opérationnel prioritaire**.

Commencer par :

1. `DATA/BSA_SIRET_THAU/bsa_siret_thau_courant.csv` ;
2. `schema-bsa-siret-thau-142-cols.csv` ;
3. `GUIDE_IA_BSA_SIRET_THAU.md` ;
4. `DATA/BSA_SIRET_THAU/MANIFESTE_BSA_SIRET_THAU.json`.

La vue courante comporte 142 colonnes : 139 colonnes historiques BSA-SIRET et trois colonnes de routage, `urlAnnuaireEntreprise`, `urlDceGithub` et `urlSiteAcheteur`.

Elle sert d'**index documenté et de routeur**, pas de nouvel entrepôt de preuve. Pour une fiche exhaustive, la restitution de référence est :
`variable → définition du schéma → valeur`.

Depuis cette ligne :

- `B_41_GESTION_URL_JSON` et `B_43_DONNEES_URL_JSON` routent vers les JSON réels Radar ; leur interprétation suit `aufilduboamp_lab_eda_eforms/GUIDE_IA_EXPLORER_JSON_EFORMS.md` ;
- `urlDceGithub` route vers le dossier DCE du marché ; lecture `README_DCE → manifeste → dérivés utiles → original si nécessaire` ;
- `urlAnnuaireEntreprise` est un pointeur canonique contrôlé vers l'Annuaire des entreprises ;
- `urlSiteAcheteur` route vers le site institutionnel de l'acheteur, à partir du référentiel contrôlé Thau ;
- `B_38_urlAvis` conserve le lien BOAMP.

La montée en priorité de Thau **ne diminue pas le rôle de Repères** : `aufilduboamp_sibsard_reperes` reste la source canonique des connaissances générales réutilisables et des sources extérieures capitalisées.

Règle synthétique :

`marché Thau → BSA-SIRET Thau + schéma → source spécialisée nécessaire → preuve → analyse → restitution`

Ne pas parcourir en masse les autres composantes avant d'avoir exploité ce point d'entrée et identifié le besoin réel.

