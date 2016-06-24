---
redirect_from: /fr/appendices/index.html
section: guide
lang: fr
title: Formats de fichier.
---

## Une vue d'ensemble des formats de fichiers

### JSON

JSON est un format de fichier simple dont la lecture est vraiment facile pour tous les langages de programmation. Cette simplicité signifie que comparé a d'autres, il est généralement plus facile à exécuter pour un ordinateur, tel que le XML.

### XML

XML est un format largement utilisé pour l'échange de données, car il conserve la structure des données et la façon dont les fichiers sont construits, et permet aux développeurs d'écrire des parties de la documentation avec les données sans interférer avec leur lecture.

### RDF

Un format recommandé par le W3C est le RDF, car il permet de représenter les données sous une forme qui rend la combinaison de données de différentes sources plus facile. Les données RDF peuvent être stockées, parmi d'autres formats, en XML et JSON. Le format RDF encourage l'utilisation d'URL en tant qu'identifiant, facilitant ainsi l'interconnexion des initiatives d'open data à travers le web. Le format RDF, bien que pas encore largement répandu, a été utilisé par certaines initiatives d'open governement, comme les projets espagnols et britanniques d'open data lié. L'inventeur du web, Tim Berners-Lee, a récemment proposé un programme de notation des initiatives d'open data en cinq étoiles, qui place les données liées au format RDF comme le but à atteindre.

### Classeurs

De nombreuses autorités ont des informations qui sont restées dans les classeurs, par exemple Microsoft Excel. Ces données peuvent souvent être utilisées immédiatement à partir des descriptions correctes des différentes colonnes.

Cependant, dans certains cas, des macros et des formules subsistent dans les feuills de calcul, ce qui peut s'avérer plus compliqué à manipuler. Il est donc conseillé de documenter ces calculs dans les feuilles de calcul, pour que cela soit plus facilement compréhensible par les utilisateurs.

### Fichiers de valeurs séparées par des virgules

Les fichiers CSV sont un format très utile, car ils sont compacts et permetttent ainsi de transférer de larges ensembles de données en conservant la même structure. Cependant, ce format est tellement fruste que, sans métadonnées, certaines données peuvent être inutiles car il est impossible de deviner le sens des différentes colonnes. C'est pourquoi il est important, lors du recours à des formats séparés par des virgules, que les métadonnées des champs individuels soient renseignées.

Par ailleurs, il est essentiel que la structure du fichier soit conservée, car une seule omission d'un champ peut perturber la lecture de tout le document et des données qui suivent, sans pouvoir corriger l'erreur pusiqu'il ne préjuge aucunement de la façon dont les données suivantes doivent être interprétées.

### Document texte

Les documents classiques dans des formats comme Word, ODF, OOXML, ou PDF peuvent être suffisants pour montrer certains types de données - par exemple, des listes de diffusion relativement stables ou équivalent. Il peut être simple et bon marché de présenter les données sous ces formats, puisqu'il est souvent le format natif des données. Cependant, le format texte ne permet pas de conserver une structure de données cohérente et compréhensible, ce qui signifie souvent qu'il est difficile de saisir des données par des moyens automatisés. Veillez à utiliser des modèles comme base des documents pour permettre d'afficher des données de réutilisation, de sorte qu'il soit au moins possible d'extraire des informations de ces documents.

Il peut également aider l'utilisation ultérieure des données par l'utilisation de balises typographiques au plus possible de sorte qu'il soit plus facile à une machine de distinguer les titres (tout type spécifié) du contenu et ainsi de suite. Généralement, il est recommandé de ne pas exposer les données au format texte, ci celles-ci existent dans un format différent.

### Texte

Les documents au format de texte plein (.tx) sont très facile à lire pour les ordinateurs. En général, ils excluent cependant les métadonnées structurelles à l'intérieur du document, ce qui signifie que les développeurs devront créer un parseur qui peut interpréter chaque document tel qu'il apparaît. 

Certains problèmes peuvent être liés à la commutation des fichiers texte entre les systèmes d'exploitation. MS Windows, Mac OS X et d'autres variantes d'Unix ont leur propre façon de dire à l'ordinateur qu'ils ont atteint la fin de la ligne.

### Image numérisée

Certainement la forme la moins adaptée à la plupart des données, mais aussi bien le TIFF que le JPEG-2000 peuvent au moins ajouter une documentation de ce que contient l'image - jusqu'à marquer une image d'un document avec le contenu du texte intégral du document. Il peut être pertinent pour les données affichées comme images dont les données ne sont pas nées électroniquement - les vieux registres paroissiaux et d'autres documents d'archive en sont des exemples évidents - et une image vaut mieux que rien. 

### Formats propriétaires

Some dedicated systems, etc. have their own data formats that they can save or export data in. It can sometimes be enough to expose data in such a format - especially if it is expected that further use would be in a similar system as that which they come from. Where further information on these proprietary formats can be found should always be indicated, for example by providing a link to the supplier's website. Generally it is recommended to display data in non-proprietary formats where feasible.

### HTML

Nowadays much data is available in HTML format on various sites. This may well be sufficient if the data is very stable and limited in scope. In some cases, it could be preferable to have data in a form easier to download and manipulate, but as it is cheap and easy to refer to a page on a website, it might be a good starting point in the display of data.

Typically, it would be most appropriate to use tables in HTML documents to hold data, and then it is important that the various data fields are displayed and are given IDs which make it easy to find and manipulate data. Yahoo has developed a tool (<http://developer.yahoo.com/yql/>) that can extract structured information from a website, and such tools can do much more with the data if it is carefully tagged.

## Formats de Fichier Ouvert

Même si l'information est fournie sous forme électronique, directement lisible par les machines, et détaillée, il peut y avoir des problèmes en relation avec le format de fichier en lui même.

The formats in which information is published – in other words, the digital base in which the information is stored - can either be "open" or "closed". An open format is one where the specifications for the software are available to anyone, free of charge, so that anyone can use these specifications in their own software without any limitations on re-use imposed by intellectual property rights.

If a file format is "closed", this may be either because the file format is proprietary and the specification is not publicly available, or because the file format is proprietary and even though the specification has been made public, re-use is limited. If information is released in a closed file format, this can cause significant obstacles to reusing the information encoded in it, forcing those who wish to use the information to buy the necessary software.

Le bénéfice des formats de fichier ouverts est qu'ils permettent aux développeurs de produire une multitude de briques logicielles et de services utilisant ces formats. Cela diminue ainsi les obstacles à la réutilisation des informations qu'ils contiennent.

Using proprietary file formats for which the specification is not publicly available can create dependence on third-party software or file format license holders. In worst-case scenarios, this can mean that information can only be read using certain software packages, which can be prohibitively expensive, or which may become obsolete.

The preference from the {term:open government data} perspective therefore is that information be released in **open file formats which are machine-readable.**

### Par exemple: les données anglaises relatives au trafic.

Andrew Nicolson is a software developer who was involved in an (ultimately successful) campaign against the construction of a new road, the Westbury Eastern bypass, in the UK. Andrew was interested in accessing and using the road traffic data that was being used to justify the proposals. He managed to obtain some of the relevant data via freedom of information requests, but the local government provided the data in a proprietary format which can only be read using software produced by a company called Saturn, who specialise in traffic modelling and forecasting. There is no provision for a "read only" version of the software, so Andrew's group had no choice but to purchase a software license, eventually paying £500 (€600) when making use of an educational discount. The main software packages on the April 2010 price list from Saturn start at £13,000 (over €15,000), a price which is beyond the reach of most ordinary citizens.

Although no access to information law gives a right of access to information in open formats, open government data initiatives are starting to be accompanied by policy documents which stipulate that official information must be made available in open file formats. Setting the gold standard has been the Obama Administration, with the Open Government Directive issued in December 2009, which says:

> *To the extent practicable and subject to valid restrictions, agencies should publish information online in an open format that can be retrieved, downloaded, indexed, and searched by commonly used web search applications. An open format is one that is platform independent, machine readable, and made available to the public without restrictions that would impede the re-use of that information.*

## Comment j'utilise un format spécifique ?

When an authority must exhibit new data – data that has not been exhibited before – you should choose the format that provides the best balance between cost and suitability for purpose. For each format there are some things you should be aware of, and this section aims to explain them.

This section focuses only on how the cut surfaces are best arranged so that machines can access them directly. Advice and guidance about how web sites and web solutions should be designed can be found elsewhere.

### Services web

For data that changes frequently, and where each pull is limited in size, it is very relevant to expose data through web services. There are several ways to create a web service, but some of the most used is SOAP and REST. Generally, SOAP over REST, REST services, but are very easy to develop and use, so it is a widely used standard.

### Base de données

Like web services, databases provide direct access to data dynamically. Base de donnéess have the advantage that they can allow users to put together just the extraction that they are interested in.

There are some security concerns about allowing remote database extraction and database access is only useful if the structure of the database and the importance of individual tables and fields are well documented. Often, it is relatively simple and inexpensive to create web services that expose data from a database, which can be an easy way to address safety concerns.
