=================================================
Telemeta : open web audio platform with semantics
=================================================

|

Telemeta_ is a free and open source web audio archiving software which introduces useful and secure methods to backup, index, transcode, analyse and publish any digitalized audio file with extensive metadata. It is dedicated to collaborative media archiving projects, research laboratories and digital humanities - and especially in ethnomusicological use cases - who wants to easily organize, backup and publish documented sound collections of audio files, CDs, digitalized vinyls and magnetic tapes over a strong database, in accordance with open web standards.

Features
========

 * Secure archiving, editing and publishing of audio files over internet.
 * Pure HTML web user interface including dynamical forms and smart workflows
 * Smart dynamical and skinnable audio player (thanks to TimeSide_)
 * "On the fly" audio analyzing, transcoding and metadata embedding based on an easy plugin architecture
 * Social cumulative indexing with semantic ontologies and timecoded markers
 * Multi-format support : FLAC, OGG, MP3, WAV and more
 * User management with individual desk, lists, profiles and rights
 * Playlist management for all users with CSV data export
 * Geo-Navigator for audio geolocalization
 * High level search engine
 * Dublin Core compatibility
 * OAI-PMH_ data provider
 * RSS feed generators
 * XML serialized backup
 * Strong SQL or Oracle backend
 * Multi-language support: english, french, german and chinese
 * Video format support (mp4, webm)

This web audio CMS is exclusively based on open source modules and can be run on any Unix or Linux system.
It is mostly written in Python and JavaScript.

The processing engine of Telemeta is a separate project called TimeSide_ as an open web audio pocessing framework written in Python.


Funding and Support
===================

To continue the development process, the project needs your explicit support. So if you use Telemeta in production or even in development, please let us know by:

 * staring or forking the project on GitHub_
 * tweeting to `@parisson_studio <https://twitter.com/parisson_studio>`_ or `@telemeta <https://twitter.com/telemeta>`_
 * droping us an email to <support@parisson.com>

Thanks for your help!


News
======

 * 1.5

   * Compatible with Django 1.6.x
   * Compatible with TimeSide 0.6.x
   * Huge refactor of all forms, detail and edit views
   * Main styles (buttons, tabs) are now based Bootstrap 3 and JQuery 2.1
   * Update models and views as needed by the CREM
   * New depedencies

 * 1.4.6

   * Drastically improve collection zip packaqe streaming thanks to zipstream (check NEW dependencies)
   * Compatible with TimeSide >= 0.5.2
   * Add URL field to item so that a external sound can be indexed and streamed
   * Add TIMESIDE_AUTO_ZOOM in settings to auto toggle the player in zooming mode
   * Add TIMESIDE_DEFAULT_GRAPHER_ID in settings to select the default grapher in the player
   * Add minor migrations
   * Fix marker display bug


See also the full CHANGELOG_


Usecases
=========

 * `CREM Sound Archives <http://archives.crem-cnrs.fr>`_ of the French Ethnomusicology Research Center (CREM) and the Musée de l'Homme:

  * 120 years of original ethnologic music data online
  * 600 geolocated collections
  * 60000 geolocated items
  * 25000 digitized items
  * More than 400 active users

 * `LAM Sound Archives <http://telemeta.lam.jussieu.fr>`_  of the "Lutherie, Acoustique et Musique" team (LAM_) at UPMC_ (University Paris 6, France)
 * `Parisson Sound Archives <http://parisson.telemeta.org>`_
 * SABIOD_ : ScAled BIODiversity project


Demo
====

 * `demo.telemeta.org <http://demo.telemeta.org>`_
 * login: demo
 * password: demo


API / Documentation
====================

 * Homepage_
 * Publications_
 * API_
 * Player_
 * Example_
 * Installation_


Development
===========

To get and run the lastest development version::

    sudo apt-get install git
    git clone https://github.com/Parisson/Telemeta.git
    cd Telemeta
    git checkout dev
    git submodule foreach git fetch --tags
    git submodule update --init --recursive
    sudo pip install -e .
    export PYTHONPATH=$PYTHONPATH:`pwd`


Feedback
=========

Email:

 * <guillaume@parisson.com>
 * <thomas@parisson.com>

Twitter:

 * `@telemeta <https://twitter.com/telemeta>`_
 * `@parisson_studio <https://twitter.com/parisson_studio>`_
 * `@yomguy <https://twitter.com/yomguy>`_

If you find some bugs, please `leave a ticket <https://github.com/Parisson/Telemeta/issues/new>`_


Authors
========

The Telemeta project is managed by:

  * Guillaume Pellerin, Parisson_ <guillaume.pellerin@parisson.com> `@yomguy <https://twitter.com/yomguy>`_
  * Joséphine Simonnot, CREM_ <josephine.simonnot@mae.u-paris10.fr>

The application is or has been developed by:

  * Guillaume Pellerin
  * Thomas Fillon
  * Paul Brossier
  * Riccardo Zaccarelli
  * Olivier Guilyardi


Partners and sponsors
======================

  * CNRS_ : Centre National de la Recherche Scientifique (French Natianal Research and Scientific Center)
  * MCC_ : Ministère de la Culture et de la Communication (the french Ministry of the Culture and Communication)
  * CREM_ : Centre de Recherche en Ethnomusicologie (Ethnomusicology Research Center, University Paris 10, France)
  * Parisson_ : Open audio development agency, Paris, France
  * LAM_ : Equipe Lutherie, Acoustique et Musique, UPMC_ (Instrument design, Acoustic and Music team of  University Paris 6, France)
  * MNHN_ : Museum National d'Histoire Naturelle (National Museum of BioParis, France)
  * ANR_ : Agence Nationale de la Recherche (French Research Agency) through the DIADEMS_ project. Partners : IRIT_, LIMSI_, LAM_, CREM_, LABRI_, MNHN_, Parisson_
  * HumaNum_ : TGIR des humanités numériques


License
=======

You can use this application in accordance with term of the CeCILL license v2 which is compatible with GPL v2 (see `LICENSE <http://github.com/yomguy/Telemeta/blob/master/LICENSE.txt>`_) for more informations.


.. _Telemeta: http://telemeta.org
.. _TimeSide: https://github.com/yomguy/TimeSide/
.. _OAI-PMH: http://fr.wikipedia.org/wiki/Open_Archives_Initiative_Protocol_for_Metadata_Harvesting
.. _Parisson: http://parisson.com
.. _CNRS: http://www.cnrs.fr
.. _MCC: http://www.culturecommunication.gouv.fr
.. _CREM: http://www.crem-cnrs.fr
.. _HumaNum: http://www.huma-num.fr
.. _IRIT: http://www.irit.fr
.. _LIMSI: http://www.limsi.fr/index.en.html
.. _LAM: http://www.lam.jussieu.fr
.. _LABRI: http://www.labri.fr
.. _MNHN: http://www.mnhn.fr
.. _MMSH: http://www.mmsh.univ-aix.fr
.. _UPMC: http://www.upmc.fr
.. _Samalyse: http://www.samalyse.com
.. _DIADEMS: http://www.irit.fr/recherches/SAMOVA/DIADEMS/fr/welcome/
.. _ANR: http://www.agence-nationale-recherche.fr/
.. _SABIOD: http://sabiod.telemeta.org
.. _CHANGELOG: http://github.com/yomguy/Telemeta/blob/master/CHANGELOG.rst
.. _Publications: https://github.com/Parisson/Telemeta-doc
.. _API : http://files.parisson.com/doc/telemeta/
.. _Player : https://github.com/Parisson/TimeSide/
.. _Example : http://archives.crem-cnrs.fr/archives/items/CNRSMH_E_2004_017_001_01/
.. _Homepage: http://telemeta.org
.. _Installation: http://github.com/yomguy/Telemeta/blob/master/INSTALL.rst
.. _GITHUB: https://github.com/Parisson/Telemeta

