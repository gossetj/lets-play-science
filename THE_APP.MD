Les specs collectives de l'application hypo-thétique
---------------------------------------------------
*Avant de concevoir une application, c'est une bonne idée de savoir à quoi elle ressemble, d'analyser quels sont les enjeux techniques de sa réalisation*

**Ce document n'est pas du tout déstiné spécifiquement aux développeurs, bien au contraire. On a tous une expérience utilisateur.**

Sommaire
--------------------------------------------------

- I. [Définitions](#I)
    1. [Post](#I.1)
    2. [Commentaire](#I.2)
    3. [Carte Heuristique / Mind map](#I.3)
    4. [Arbre sémantique](#I.4)
    5. [Hash sémantique](#I.5)
    6. [Filtre sémantique](#I.6)
    7. [Fusion](#I.7)
    8. [Soumission](#I.8)
    9. [Version](#I.9)
    10. [Post cible](#I.10)
    11. [Post source](#I.11)
    12. [Référence](#I.12)
    13. [Défi](#I.13)
- II. [Cycle de vie d'un défi](#II)
- III. [Associations sémantiques](#III)
- IV. [Versionnement](#IV)
- V. [Rôles](#V)

<a name="I"></a>
## I. Définitions & Concepts
*On va p'tet commencer par s'accorder sur le sens des mots nan?*

<a name="I.1"></a>
#### 1. Post
Document collaboratif qui propose une approche de réponse possible.  
**Problème** : comment correctement circoncir le périmètre de la réponse ?

<a name="I.2"></a>
#### 2. Commentaire
Observation, critique, avis fait sur un post. Ce n'est pas un document collaboratif.

<a name="I.3"></a>
#### 3. Carte Heuristique / Mind map
Vue en 2D sous forme de diagramme de graphe ordonné des liens sémantiques *entre posts*

<a name="I.4"></a>
#### 4. Arbre sémantique
*[README.md#II.3.b](README.md#II.3.b)*  
Vue sous forme d'arbre des liens sémantiques *entre posts*  
**Remarque** : Une feuille peut être dupliquée sur différents noeuds !
Ex :
> ├── Ascenceurs spatiaux  
│   ├── Ascenseur  
│   ├── Skyhook  
│   └── …  
├── Propulsion  
│   ├── Capsules à explosions nucléaire  
│   ├── Fusées  
│   │   ├── Explosion  
│   │   ├── Hydrogène  
│   │   └── …  
│   └── …  
└── …

<a name="I.5"></a>
#### 5. Hash sémantique
*[README.md#II.3.c](README.md#II.3.c)*  
Chemin de l'arbre sémantique exprimé sous forme de hashtag, chaque feuille est séparée de son noeud par un `:`

Ex :
> `#Propulsion:Fusées:Explosion`

<a name="I.6"></a>
#### 6. Filtre sémantique
Expression textuelle permettant de filtrer les posts suivant les noeuds sélectionnés
Ex :
> `#Propulsion:Fusées`

Affiche tous les posts référés dans le chemin `Propulsion:Fusées`.  

**Remarque** :  
> `#Fusées`

Va aggréger (fusionner) tous les noeuds appellés `Fusées`

<a name="I.7"></a>
#### 7. Fusion
Action de fusionner deux posts sémantiquement proches.
- Questions : qui propose la fusion ? Un utilisateur peut-il suggérer la fusion de deux posts qu'il trouve proches? P'tet une option "proposer une fusion", cette dernière devant être validée par les deux auteurs...

<a name="I.8"></a>
#### 8. Soumission
*Non, pas le machin de Houellebecq*
Action de soumettre à l'auteur d'un post une nouvelle **version** du document.

<a name="I.9"></a>
#### 9. Version
Une version figée d'un post, qu'on peut rétablir plus tard.
**Remarque** : Une fusion créée automatiquement une nouvelle version du **post cible**.

<a name="I.10"></a>
#### 10. Post cible
C'est la destination (reçu par l'hôte) de la fusion

<a name="I.11"></a>
#### 11. Post source
C'est l'origine (proposé par l'offreur) de la fusion

<a name="I.12"></a>
#### 12. Référence
Référence (source littéraire, culturelle) associée à un post.

<a name="I.13"></a>
#### 13. Défi
Question soumise pour l'organisateur de l'évênement, ici Léo, et par extension, tous le processus d'élaboration de réponses par les participants.

<a name="II"></a>
### II. Cycle de vie d'un défi
*Description détaillée du cycle de vie d'un [défi](#I.13)*

<a name="III"></a>
## III. Associations sémantiques
*Aspects techniques des associations sémantiques*

<a name="IV"></a>
### IV. Versionnement
*Aspects techniques sur le versionnement des posts*

<a name="V"></a>
### V. Rôles
*Déscription détaillée des rôles endossés par les participants*
