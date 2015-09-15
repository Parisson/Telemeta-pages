.. image:: images/help.png
    :align: left

﻿================================ 
Pages d'aide de Telemeta - LAM
================================
Contacts
--------
Pour obtenir une aide technique, merci de vous inscrire à la mailing liste de Telemeta :

    `http://lists.parisson.com/cgi-bin/mailman/listinfo/telemeta <http://lists.parisson.com/cgi-bin/mailman/listinfo/telemeta>`_

ou bien contacter la hotline parisson par e-mail :

    support@parisson.com

ou twitter :

    `http://twitter.com/telemeta <http://twitter.com/telemeta>`_

Pour plus d'informations sur le système Telemeta, voir `telemeta.org <http://telemeta.org>`_

Telemeta utilise la librairie audio TimeSide : `code.google.com/p/timeside/ <http://code.google.com/p/timeside/>`_

Description générale
---------------------
Ces pages (en construction) constituent une aide dans l'utilisation de Telemeta - LAM. Elles décrivent la structure des données permettant la compréhension du modèle de données et la façon d'accéder aux enregistrements ; les actions à réaliser pour y ajouter de nouveaux fichiers sons et les métadonnées associées.


Les différents descripteurs du modèle de données sont organisés en 4 niveaux hiérarchiques, les niveaux Fonds, Corpus, Collections et Item. Les métadonnées sont structurées selon le modèle Dublin Core et il a été décidé qu'un item correspond, le plus souvent, à un fichier numérisé. Cependant, l'opérateur de numérisation peut être amené à découper un fichier trop long afin de permettre une meilleure lecture localisée de son signal. Une durée maximale pour un item lui sera précisée.

Lorsque l'on se retrouve sur Telemeta, le menu Archives déroule les différents niveaux à partir desquels il est possible d'accéder en lecture aux différents enregistrements. A chaque niveau, chaque enregistrement est identifié par sa cote unique.

- Au 1er octobre 2012, le niveau Fonds caractérise 4 enregistrements :

	Etudes et expériences						(cote LAM_ETUD)

	Évènements							(cote LAM_EVEN)

	Patrimoine instrumental						(cote LAM_PATR)

	Travaux de recherche d'étudiants				(cote LAM_TRAV)

Chaque fichier son (ou item) découle de l'un de ces 4 enregistrements, d'un corpus unique et d'une collection et une seule.

- A chaque fonds, on associe un certain nombre de corpus dont la cote est LAM_FONDS_dd(CORPUS).

- De même, à chaque corpus, on associe des collections dont la cote a pour format LAM_FONDS_dd(CORPUS)_dd(COLLECTION). 

Par exemple, la collection  « Etude sur les instruments à cordes » appartient au fonds « Etudes et expériences » et au corpus « Etudes d'instruments de musique européens » et sa cote est LAM_ETUD_01_02.

- Le niveau Items liste tous les fichiers sons. Chaque fichier son ou item est caractérisé par sa cote :  LAM_FONDS(nom)_dd(CORPUS)_dd(COLLECTION)_ddd(ITEM)

Par exemple, l'item « Guitare Dominique Douau – Expérience barrage – 3 barres – 5 barres 2/5 »  dont la cote est LAM_ETUD_01_02_002 est le 2ème item contenu dans la collection « Etude sur les instruments à cordes ».

Connexion
----------------

L'utilisateur se connecte. Le menu Bureau (de l'utilisateur connecté) apparaît dans la barre des menus et comprends les éléments Listes (listes de lecture), Profil et Accueil.

Pour un utilisateur ayant le profil Administrateur, les menus Utilisateurs (liste des utilisateurs inscrits) et Générale (administration du site) apparaissent également.


Ajout d'un item
----------------

Choisir l'élément Items dans le menu Archives. Les différents descripteurs associés au niveau Items s'affichent. Le nouvel item est créé par l'enregistrement de la fiche de description.


Organisation de l'arborescence des niveaux
-------------------------------------------

Corpus et collections du Fonds Évènements  (EVEN) :

+------------------------------------------+-----------------------------------------------------+-----------------------+
|                  Corpus                  |        Collections                                  |           Cote        |
+==========================================+=====================================================+=======================+
|  Rencontres scientifiques (exposé, conf, |                                                     | LAM_EVEN_01_dd        | 
|  congrès, exposé, séminaire)             |                                                     |                       |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Voix humaine (paroles, voix chantée, icophone)      | LAM_EVEN_01_01        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Instruments de musique                              | LAM_EVEN_01_02        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Timbre, acoustique des salles, …                    | LAM_EVEN_01_03        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|  Réunions du GAM                         | Par bulletin (ordre chronologique croissant)        | LAM_EVEN_02_01        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|  Cours                                   | Par personne                                        | LAM_EVEN_03_01        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|  Concerts                                | Par genre (musique contemporaine, classique, …) ?   | LAM_EVEN_04_01        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|  Valorisation et diffusion               |                                                     | LAM_EVEN_05_dd        | 
|  grand publique du LAM                   |                                                     |                       |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Montage pour la radio                               | LAM_EVEN_05_01        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Montage pour la TV                                  | LAM_EVEN_05_02        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Archives diverses                                   | LAM_EVEN_05_03        |
+------------------------------------------+-----------------------------------------------------+-----------------------+

Corpus du Fonds Etudes et expériences  (ETUD) :

+------------------------------------------+-----------------------------------------------------+-----------------------+
|                  Corpus                  |        Collections                                  |           Cote        |
+==========================================+=====================================================+=======================+
|  Etudes d'instruments de musique         | Selon organologie (et par année)                    | LAM_ETUD_01_dd        | 
|  européens                               |                                                     |                       |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Instruments à vent                                  | LAM_ETUD_01_01        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Instruments à cordes                                | LAM_ETUD_01_02        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Instruments à percussion                            | LAM_ETUD_01_03        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Instruments électriques et électromécaniques        | LAM_ETUD_01_04        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Synthèse sonore                                     | LAM_ETUD_01_05        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|  Etudes sur la voix humaine              |                                                     | LAM_ETUD_02_dd        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Voix chantée                                        | LAM_ETUD_02_01        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Voix parlée                                         | LAM_ETUD_02_02        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Synthèse de la parole (icophone, synthèse vocale)   | LAM_ETUD_02_03        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Pathologie (voix et audition)                       | LAM_ETUD_02_04        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Voix d’enfants                                      | LAM_ETUD_02_05        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|  Etudes sur la perception                |                                                     | LAM_ETUD_03_dd        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Tests de catégorisation                             | LAM_ETUD_03_01        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Tests d'écoute                                      | LAM_ETUD_03_02        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Tests linguistiques                                 | LAM_ETUD_03_03        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Entretiens                                          | LAM_ETUD_03_04        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|  Etudes de l'acoustique des salles       |                                                     | LAM_ETUD_04_dd        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Salles de spectacles (concert, spectacle...)        | LAM_ETUD_04_01        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Lieux d'enseignement (intelligibilité)              | LAM_ETUD_04_02        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Salles de cultes                                    | LAM_ETUD_04_03        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|  Etudes d'ambiances sonores              |                                                     | LAM_ETUD_05_dd        | 
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Enregistrements en milieu urbain                    | LAM_ETUD_05_01        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Enregistremens en milieu rural                      | LAM_ETUD_05_02        |
+------------------------------------------+-----------------------------------------------------+-----------------------+
|  Etudes des musiques de traditions orales| Selon organologie ou pays (selon pertinence)        | LAM_ETUD_06_dd        | 
+------------------------------------------+-----------------------------------------------------+-----------------------+
|  Etudes d'archives sonores (cf JMF)      | Par session                                         | LAM_ETUD_07_dd        | 
+------------------------------------------+-----------------------------------------------------+-----------------------+
|  Communications animales                 | Cris des animaux,...                                | LAM_ETUD_08_dd        | 
+------------------------------------------+-----------------------------------------------------+-----------------------+


Corpus du Fonds Patrimonial (PATR) :

+------------------------------------------+-----------------------------------------------------+-----------------------+
|                  Corpus                  |        Collections                                  |           Cote        |
+==========================================+=====================================================+=======================+
|  orgue                                   | Par mission                                         | LAM_PATR_01_dd        | 
+------------------------------------------+-----------------------------------------------------+-----------------------+
|  cloche                                  | Par mission                                         | LAM_PATR_02_dd        | 
+------------------------------------------+-----------------------------------------------------+-----------------------+
|  clavecin, piano forte                   | Par session                                         | LAM_PATR_03_dd        | 
+------------------------------------------+-----------------------------------------------------+-----------------------+
|  flûte                                   | Par session                                         | LAM_PATR_04_dd        | 
+------------------------------------------+-----------------------------------------------------+-----------------------+
|  Autres                                  | Par session                                         | LAM_PATR_05_dd        | 
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Diapason, porte-voix                                | LAM_PATR_05_01        | 
+------------------------------------------+-----------------------------------------------------+-----------------------+

Corpus du Fonds travaux de Recherche d'étudiants (TRAV) :

+------------------------------------------+-----------------------------------------------------+-----------------------+
|                  Corpus                  |        Collections                                  |           Cote        |
+==========================================+=====================================================+=======================+
|  Mémoires                                | Par niveau d'étude                                  | LAM_TRAV_01_dd        | 
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | DEA- MASTER                                         | LAM_TRAV_01_01        | 
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Thèse                                               | LAM_TRAV_01_02        | 
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Rapport de recherche, de mission, d’expertise       | LAM_TRAV_01_03        | 
+------------------------------------------+-----------------------------------------------------+-----------------------+
|                                          | Autre (Prix CNSM, ...)                              | LAM_TRAV_01_04        | 
+------------------------------------------+-----------------------------------------------------+-----------------------+





