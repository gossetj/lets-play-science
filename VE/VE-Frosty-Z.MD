Vision d'Ensemble de [Frosty-Z](https://github.com/Frosty-Z)
==

<a name="I"></a>
I. Espace de discussion (fil de commentaires, forum...)
-

<a name="I.1"></a>
### I.1. Cas 1 : s'appuyer sur l'existant (Youtube + Facebook)

Fonctionnalités *à détailler* disponibles sur la plateforme Let's Play Science suite à un traitement des commentaires "bruts"
* Exploitation de données type metrics (par ex. occurrences de mots)
* Possibilité d'un début de structuration sémantique ?
* Revue collaborative ? Pour en faire quoi précisément, par qui à part Léo ?

<a name="I.1"></a>
### I.1. Cas 2 : espace de discussion "souverain"

Implique que Léo doit bloquer les commentaires Youtube, et indiquer sur Youtube et Facebook un lien vers la plateforme de collaboration pour Let's Play Science (par ex. page d'accueil du défi en cours).

Fonctionnalités qui seraient disponibles en plus du **cas 1** : *à détailler*
* Votes par catégorie sur chaque post
* Hashtags (avec éventuellement gestion de namespaces : Hashtags sémantiques)

Coût certainement sensiblement plus élevé que le **cas 1**.

<a name="II"></a>
Espace Q&A + écriture collaborative
-

Inspiré de StackOverflow, Yahoo Q&A, Tricider... ou [autre](http://web.appstorm.net/roundups/18-awesome-survey-poll-apps/), ou "fait maison" si on ne trouve rien qui correspond aux fonctionnalités que l'on souhaite en gratuit.

Fonctionnalités *à détailler*
* Questions/Réponses
* Votes
* Réputation
* Modération
* Possibilité d'éditer les questions et réponses de manière collaborative (= [posts versionnés](https://github.com/sveinburne/lets-play-science/blob/master/THE_APP.MD#b-post-versionné))
* Structuration sémantique (tags, sous-questions...)




**Rappel des guidelines restant à suivre**

<a name="II.1"></a>
#### 1. Critères de soumission d'une VE
Voici **les critères** pour qu'une pull request de VE soit acceptée :
//- elle doit être sensiblement différente d'une VE existante
- elle doit s'appuyez rigoureusement sur le vocabulaire définit en [**I**](#I)
- elle doit être rédigée avec **concision** et esprit de **synthèse**
- elle doit offrir une **perspective** à minima sur les points suivants :
//  1. Application Souveraine vs Application intégrée ?
  2. Posts Versionnés vs posts simples
  3. Type de modération
  4. Choix technologique sur la sémantique
  5. Vote simple vs vote catégorique
  6. Politique de rôles ?
- elle doit expliciter un cycle de vie d'un défi
- elle doit proposer une priorisation de ses fonctionnalités
- elle doit offrir un titre qui explicite le parti pris de cette vision
- le nom du fichier markdown doit être `VE-nomAuteur.MD`, elle sera renommée lors du merge.

Remarques importantes :
- Une solution ne s'oppose pas nécessairement à sa concurrente, elle peut être offerte provisoirement en attendant le développement de fonctionnalités plus avancées, cf. priorités.
- Si des **définitions** manquent ou des nuances sont nécessaires à apporter, merci de **soumettre une issue** ou une **pull request** en exprimant clairement votre besoin.
- Une fois acceptée, l'auteur de la **pull request** doit créer une issue portant le titre de la PR. Ce sera le fil de discussion officiel autour de cette VE. Des critiques et des propositions d'amendements pourront être soumises.
