DL0MUC Homepage
===============

This is the Jekyl based DL0MUC Homepage
The theme is based on the jekyll template by https://github.com/svmiller

Anwenderhinweise
================

Erstellen von Posts
-------------------

* Posts befinden sich im _posts Verzeichnis
* Filename bitte IMMER mit YYYY-MM-DD-Kurzname.md ablegeb
* layout: post
* Posts können automatisiert einem Projekt oder Kategorie hinzugefügt werden (auch Mehrfach).
  * categories:
    * post - muss bei Blogeintrag immer vorhanden sein
    * project - Post kann einem bestimmten Projekt zugefügt werden
    * logbuch - Post wird im Aufbaulogbuch aufgelistet
  * project:
    * Wenn project in Post und einer Page übereinstimmen, werden die Posts unten an die Seite angehängt
    
Erstellen von Pages
-------------------

* Pages befinden sich entweder im Wurzelverzeichnis oder im projects Verzeichnis. Pages für Projekte bitte immer im projects Verzeichnis anlegen.
* layout: page
* categories: project oder none.
* project: Wenn categorie 'project' enthält werden auf der page alle Posts angezeigt die den selben project tag haben
    
