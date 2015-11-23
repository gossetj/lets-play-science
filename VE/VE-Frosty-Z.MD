Vision d'Ensemble de [Frosty-Z](https://github.com/Frosty-Z)
==

Principe
-
**Dans un premier temps**, exploiter au maximum les données des commentaires Youtube / Facebook tel que décrit dans le [`Readme`](https://github.com/sveinburne/lets-play-science/blob/master/README.md) via une **application intégrée**. En parallèle, mettre en avant un **[espace Q&A](#II)** aussi adapté que possible au cas de *Let's Play Science*, afin d'exploiter la grande efficacité collaborative mise en évidence par ce type d'outil (s'il ne fallait citer qu'un exemple : [Biology StackExchange](http://biology.stackexchange.com/)).
Evidemment, l'ensemble devra rester simple pour être exploitable rapidement, et éviter de se perdre dans des développements trop coûteux et/ou complexes.

**Dans un deuxième temps**, selon le succès et l'efficacité montrés par ces outils "mis à l'épreuve", des fonctionnalités plus avancées pourront être développées, les performances soignées et améliorées, voire de nouveaux outils (si nécessaire) pourront compléter la plateforme.


<a name="I"></a>
I. Espace de discussion (fil de commentaires, forum...)
-

<a name="I.1"></a>
### I.1. Application intégrée (Youtube + Facebook + interface de "suivi")

**Fonctionnalités** disponibles sur la "plateforme externe"
* Soumettre un commentaire/post
* Cliquer sur les boutons :+1: / :-1: (selon plateforme)
* Répondre spécifiquement à un commentaire (=> arborescence de commentaires)

**Fonctionnalités** disponibles sur la *plateforme Let's Play Science* suite à un traitement des commentaires "bruts" :
* Exploitation de données type metrics (nombre de posts, occurrences de mots...)
* Moteur de recherche de commentaires simple
* Toute autre fonctionnalité simple à mettre en oeuvre (analyseurs syntaxiques existants...) qui peuvent apporter une information générale sur la masse de commentaires bruts sans être trop coûteux.


<a name="I.2"></a>
### I.2. Application souveraine

**Coût global certainement sensiblement plus élevé** que le cas de l'[application intégrée](#I.1). A voir **dans un deuxième temps**.

Implique que Léo bloque les commentaires Youtube, et indique sur Youtube et Facebook un lien vers la plateforme de collaboration pour Let's Play Science (par ex. page d'accueil du défi en cours).

**Fonctionnalités** qui seraient disponibles en plus du cas de l'[application intégrée](#I.1), correspondant autant que possible au [**II.1** du `Readme`](https://github.com/sveinburne/lets-play-science/blob/master/README.md#II), et *à prioriser* :
* Votes par catégorie sur chaque post
* Hashtags (avec éventuellement gestion de namespaces : Hashtags sémantiques)
* etc.

Excepté la notion de [posts versionnés](https://github.com/sveinburne/lets-play-science/blob/master/THE_APP.MD#b-post-versionné) car déjà présente dans [l'espace Q&A](#II). Les posts seraient tout de même éditables par l'auteur + les modos, mais sans gestion d'historique de versions.



<a name="II"></a>
II. Espace Q&A + écriture collaborative
-

Inspiré de StackOverflow, Yahoo Q&A, Tricider... ou [autre](http://web.appstorm.net/roundups/18-awesome-survey-poll-apps/), ou "fait maison" si on ne trouve rien qui correspond aux fonctionnalités que l'on souhaite en gratuit.

### Avantages

* Permet de **structurer les propositions de manière arborescente**, s'apparentant à un **"mind map"** en temps réel (un "mind map" succinct peut également être envisagé en ne retenant que les *titres* des sous-propositions, sous-défis, sous-sous-propositions, etc. et pourrait très bien faire office de page d'accueil)

* **Tous nouveaux élements** (références, arguments, etc.) **sont agrégés au fil des participations** (modification, ou proposition de modification possible par tous, Wiki-like) **et visibles facilement par tous** (vs. revue fastidieuse de posts souvent redondants, hors sujet, d'une file de discussion)
 * Constitue une expérience d'écriture collaborative
 * Favorise la revue entre pairs
 * Chaque participant choisit à tout moment le(s) rôle(s) qu'il souhaite jouer, quelle contribution il souhaite apporter et sur quel sujet / sous-sujet, sans nécessiter de tâches d'administration ou d'adaptation de l'application (seule exception : le rôle de modérateur).

* **La fin du défi peut intervenir à tout moment**, lorsque les diverses propositions semblent être arrivées à "maturité" (par ex. en suivant un metric sur le nombre de propositions / edits par jour)


### Fonctionnalités

#### Questions/Réponses
* Au début du cycle de vie, seule la question principale (correspondant au défi) serait posée.
* Chaque participant peut formuler une ou plusieurs propositions
* Les propositions sont classées par "score" (nb. votes positifs + nb. votes négatifs) décroissant
* Tout participant, dès qu'il l'estime nécessaire, peut créer une ou plusieurs sous-questions ("sous-défis"), permettant d'affiner les "propositions principales" (par ex. défi *"Peut-on envoyer l'humanité dans l'espace ?"*, une proposition est formulée sur l'idée de fusée, un participant peut créer la question associée : *"Quel est le meilleur système de propulsion pour une fusée ?"*).

#### Votes
* Chaque participant peut donner un seul vote positif ou négatif pour une réponse (proposition) donnée. Authentification obligatoire pour réduire les risques de votes automatiques.

#### Réputation *(proposition)*
Valorisant, motivant, reflète le niveau de confiance accordé à un participant par la communauté.

Peut permettre à terme de "débloquer" certaines fonctionnalités avancées (alerter un modo, modifier une définition de hashtag...), par défaut inacessibles.

* +1 par contribution (proposition, création de sous-défi, édition approuvée par un modo...)
* +3 par vote positif reçu sur sa propre proposition
* -1 par vote négatif donné ou reçu
* *[Dev de priorité moindre]* +1 par vote positif reçu sur une proposition à laquelle on a participé (par ex. édition d'au moins 100 caractères, approuvée par un modo)

Ce mécanisme de réputation peut être combiné à des participations sur la *plateforme de discussion*, notamment en cas de vote par catégorie
* +3 pour un vote "intéressant" reçu

#### Modération
* Possibilité de modifier tout (sous-)défi, et (sous-)proposition, avec versionnage

#### Possibilité d'éditer les questions et réponses de manière collaborative (= [posts versionnés](https://github.com/sveinburne/lets-play-science/blob/master/THE_APP.MD#b-post-versionné))
* L'auteur de la question/proposition, un modo, ou un participant authentifié (avec validation par modo), peut modifier son contenu (titre, description, hashtags...), avec versionnage, permettant ainsi une *rédaction collaborative* des (sous-)propositions.
* Modifications concurrentes : dans un premier temps, je propose un simple "c'est le dernier commit qui gagne" étant donné qu'on aurait le versionnage d'entrée de jeu. A voir dans le temps et selon le succès de la plateforme, pour une gestion plus poussée.

#### Structuration sémantique (tags, sous-questions...)
* Chaque (sous-)défi et (sous-)proposition peut être associé à des hashtags.
* Si possible, ces hashtags et la gestion de leurs définitions seront partagés avec les autres espaces d'échange sur la plateforme (interface de gestion commune).
* Il devra être possible à tout moment de rechercher les défis/propositions correspondant à un ou plusieurs hashtags, mots clés, etc. via un moteur de recherche
* En consultant un défi, pouvoir accéder facilement :
 * Aux sous-défis associés à chaque proposition
 * Au "défi parent" s'il existe

#### Authentification
* Autant que possible, elle doit être partagée avec le reste de la *plateforme Let's Play Science*
* Support authentification via Google+ / Facebook souhaitable, plus simple pour de nombreux utilisateurs.


<a name="III"></a>
III. Modération
-

Considérations d'ordre général :

* Dans un premier temps, Léo + les développeurs de la plateforme seraient modos, tous espaces confondus.
* Ensuite si nécessaire des fonctionnalités permettant l'élection des modérateurs (durée de mandat à définir), pourraient être envisagées.




***


**Rappel des guidelines restant à suivre**

<a name="II.1"></a>
#### 1. Critères de soumission d'une VE
Voici **les critères** pour qu'une pull request de VE soit acceptée :
//- elle doit être sensiblement différente d'une VE existante
//- elle doit s'appuyez rigoureusement sur le vocabulaire définit en [**I**](#I)
//- elle doit être rédigée avec **concision** et esprit de **synthèse**
//- elle doit offrir une **perspective** à minima sur les points suivants :
//  1. Application Souveraine vs Application intégrée ?
//  2. Posts Versionnés vs posts simples
//  3. Type de modération
//  4. Choix technologique sur la sémantique
//  5. Vote simple vs vote catégorique
//  6. Politique de rôles ?
//- elle doit expliciter un cycle de vie d'un défi
//- elle doit proposer une priorisation de ses fonctionnalités
- elle doit offrir un titre qui explicite le parti pris de cette vision
//- le nom du fichier markdown doit être `VE-nomAuteur.MD`, elle sera renommée lors du merge.

Remarques importantes :
- Une solution ne s'oppose pas nécessairement à sa concurrente, elle peut être offerte provisoirement en attendant le développement de fonctionnalités plus avancées, cf. priorités.
- Si des **définitions** manquent ou des nuances sont nécessaires à apporter, merci de **soumettre une issue** ou une **pull request** en exprimant clairement votre besoin.
- Une fois acceptée, l'auteur de la **pull request** doit créer une issue portant le titre de la PR. Ce sera le fil de discussion officiel autour de cette VE. Des critiques et des propositions d'amendements pourront être soumises.
