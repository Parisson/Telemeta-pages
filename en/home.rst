========
KAMOULOX
========



Basis and rationale for the project
===================================

KAMoulox aims at developing cutting-edge audio processing techniques and making them available for research and educational  purpose to a large audience, in an open-source environment embedded in real-world sound archives. The main assumption of the project is that audio separation and restoration can help shape new practices regarding our immaterial audio heritage. It can notably benefit to the scientific and educational exploitation of this heritage through the concept of crowd processing.

Main issues and general objectives
==================================

The users of large audio repositories lack convenient signal processing tools to help them manipulate the recordings, whether they be a linguist trying to remove noise from a very old recording featuring a native speaker of a language now extinct or an ethnomusicologist working on sacred musical structures with field-material strongly corrupted by noise.

The purpose of the KAMoulox project is to leverage on recent research on signal processing to provide the web-based audio processing tools and interfaces needed to clean or separate audio recordings easily, when the user is a neophyte in sound engineering. The applicative domain of this project lies in the context of large-scale sound archives and revaluation of our musical heritage through its exploitation by the researchers and the public itself. In my opinion, the most remarkable aspect of this project is the technology transfer from cutting-edge signal processing to the promotion of our cultural heritage. 

This project would serve several concurrent objectives. First, it would dig in the promising research directions in audio processing that I have proposed very recently in a joint work with my national and international partners, thus benefiting from our advance in the field. Second, it would ease the work of the professional ethnomusicologist, linguist or archivist and thus be extremely useful for research and educational purposes. Third, it would immediately transform unique audio repositories into extraordinary raw material for all artists to use in their musical or multimedia creations, by restoring old testimonies or isolating some particular elements of interest. Those cultural borrowings would create a bridge between generations and would be a very exciting way to promote each and every culture in the world through the positive idea of artistic sharing and reuse.

Methods or technologies used
============================

KAMoulox is decomposed into 4 work-packages (WPs) of equal importance, that closely reflect its numerous scientific and technical objectives. From a transversal application perspective, all WPs revolve around incrementally improving a web-based source separation software architecture. 

WP1 Robust separation methods: builds on recent advances I proposed in probabilistic signal processing, that are based on the alpha-stable formalism and which notably extend the classical Gaussian methodology to heavy-tailed signals. This part of the project feature two main challenges. The first one is the estimation of parameters in models that do not come with likelihood functions. Ideas include moment fitting and Monte Carlo methods. Second, the case of multichannel signals brings interesting research directions for probabilistic signal processing.

WP2 Extensions of KAM: will introduce new nonparametric ways of estimating the parameters of sources, notably their time-frequency energy profiles. This also comes with new ways to format the feedback displayed to the user for interacting with him. This work-package is divided into two main parts: first, the design of new non-parametric spectrogram models, such as deep-nets or nonnegative alpha-stable. Second, the iterative processing achieved through an interaction between the filtering machine and a user.

WP3 Separation web-service will provide computationally efficient implementations to separation and parameter estimation procedures. It will also be critical in embedding the whole architecture on the existing  platform of the CNRS - Musée de l'Homme.

WP4 Design and science outreach will first focus on the design of the client-side application using a resolutely user-centered methodology. It will then lead to the actual realization of this multimedia client, but also to the promotion of this technology through the realization of multimedia content and through the participation of strategical social events.



.. _Telemeta: http://telemeta.org
.. _TimeSide: https://github.com/Parisson/TimeSide/
.. _Kamoulox: http://www.agence-nationale-recherche.fr/?Projet=ANR-15-CE38-0003

