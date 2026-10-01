# COMMENT FONCTIONNE Bitcoin ?

Des règles, pas des dirigeants

tic-tac/
/bloc suivant

* Bitcoin utilise la preuve de travail, la cryptographie à clé publique et un réseau pair à pair pour traiter et vérifier les paiements dans un registre mondial, distribué et accessible en ligne.

>**Cryptographie** (nom)
>
>*: chiffrement et déchiffrement de messages au moyen d'un code secret ou d'un chiffre
>: encodage et décodage informatisés de l'information*

~ Merriam Webster Dictionary

>**Hachage** (nom)
>
>*: procédé utilisant un algorithme mathématique appliqué à des données afin de produire une valeur numérique (une empreinte ou « hash ») représentative de ces données.*

~ csrc.nist.gov

>**Rappel :**
>
>L'écosystème Bitcoin comprend >>
>
>**bitcoin :** l'**actif monétaire** numérique
>
>**Bitcoin :** le **réseau de paiement** composé de mineurs et de nœuds

1 bitcoin = 100 000 000 satoshis (sats)

**(Vous pouvez acheter des sats, c'est-à-dire une fraction de bitcoin.)**

---

>*Nous définissons une pièce électronique comme une chaîne de signatures numériques. Chaque propriétaire transfère la pièce au suivant en signant numériquement une empreinte de la transaction précédente ainsi que la clé publique du propriétaire suivant, puis en ajoutant ces éléments à la fin de la pièce. Le bénéficiaire peut vérifier les signatures afin de vérifier la chaîne de propriété.*

~ Satoshi Nakamoto
Livre blanc de Bitcoin, partie 2, 2008
Description du fonctionnement d'une transaction bitcoin dans le registre distribué

---
## L'ÉCOSYSTÈME BITCOIN...
**se compose de mineurs, de nœuds, d'utilisateurs et de développeurs**

qui travaillent tous indépendamment,

et en même temps de manière interdépendante,

pour faire vivre ce qui est

BITCOIN !

![bitcoin](figure-06-m-u-n-d.png)

---
## MINEURS
* Des **nœuds spécialisés** — des ordinateurs appelés ASIC — qui **« minent » les blocs** intégrés à la blockchain Bitcoin.
* Ce faisant, ils **vérifient les transactions déjà validées par les nœuds, émettent de nouveaux bitcoins** et **contribuent à sécuriser l'ensemble du réseau.**

## UTILISATEURS
* **Vous et moi. Nous tous.** Les gens.
* En reconnaissant la valeur des biens et services fournis, nous effectuons des transactions : nous donnons et recevons des bitcoins, ou nous les conservons pour une utilisation ultérieure selon nos besoins.

## NŒUDS
* **Les nœuds sont des ordinateurs qui exécutent le logiciel Bitcoin.**
* **Des milliers de nœuds** constituent le **réseau volontaire, mondial et décentralisé qui valide les transactions**, empêchant ainsi la double dépense et contribuant à sécuriser le système.

## DÉVELOPPEURS (DEVS)
* **Développeurs, programmeurs et auteurs numériques** qui travaillent à **maintenir et faire évoluer le réseau, améliorer la sécurité, la confidentialité et l'interface utilisateur, et rendre le code** compréhensible et utilisable par le reste d'entre nous.

---

## UNE TRANSACTION BITCOIN :
Ali veut envoyer des bitcoins à Benji :

>1. Ali **ouvre son portefeuille bitcoin** sur son téléphone et **appuie sur « Envoyer ».**
>2. Benji **ouvre son portefeuille** et **appuie sur « Recevoir ».**
>3. **S'ils sont ensemble :** Ali scanne le QR code affiché dans le portefeuille de Benji.
>4. **S'ils ne sont pas ensemble :** Ali copie et colle dans son portefeuille l'adresse que Benji lui a envoyée.
>5. Ali **saisit le montant à envoyer** et appuie sur **« Envoyer ».**
>6. **Quelques secondes plus tard,** Benji voit apparaître le montant en attente dans son portefeuille.
>7. **Si le paiement passe par Lightning,** il est confirmé presque instantanément et coûte très peu.
>8. **S'il est envoyé « on-chain »** (sur la chaîne principale de Bitcoin), il comporte des frais et prend généralement environ 10 minutes pour obtenir une première confirmation. Cela peut être plus long selon l'activité du réseau.

---

## UNE TRANSACTION BITCOIN SOUS LE CAPOT :
(Les termes **en gras** sont définis plus bas.)

>1. Lorsque Ali envoie ces sats à Benji, la **transaction** est **diffusée** sur le réseau.
>2. La transaction est validée par des **nœuds**, qui vérifient qu'Ali possède bien les bitcoins qu'elle souhaite envoyer et qu'ils n'ont pas déjà été dépensés, afin d'empêcher la double dépense.
>3. Une fois validée par un nœud, elle attend dans la **mempool** avec les transactions des autres utilisateurs.
>4. Les transactions de la mempool sont intégrées dans un **bloc** de la **blockchain** lorsqu'un **mineur** trouve un **nonce** produisant une empreinte conforme à la **cible de difficulté**.
>5. Chaque **bloc** comporte un **horodatage**.
>6. Cela contribue à l'**immutabilité** et aide à protéger l'ajustement de la difficulté contre les manipulations.
>7. Chaque bloc représente une confirmation pour les transactions qu'il contient.
>8. À mesure que les blocs s'ajoutent, en moyenne toutes les dix minutes, la difficulté de modifier l'historique de la blockchain augmente.

---

## GLOSSAIRE

---
>* **TRANSACTION ~ Envoi/réception de bitcoins**
---
* Un transfert de valeur, sous forme de satoshis, d'un détenteur de bitcoins à un autre.

---
>* **NŒUD ~ Une « branche » du réseau Bitcoin décentralisé. Tout le monde peut faire fonctionner un nœud.**
---

* Les nœuds sont des ordinateurs qui exécutent le logiciel Bitcoin.
* Les nœuds, avec les mineurs, les utilisateurs et les développeurs, forment le réseau pair à pair Bitcoin.
* Imaginez **chaque nœud complet comme une copie indépendante du registre Bitcoin.**
* Ils interagissent et parviennent à un consensus en acceptant et en validant les transactions provenant d'autres nœuds ainsi que les blocs proposés par les mineurs, puis en les relayant aux autres nœuds.
* Les nœuds sont exploités de manière volontaire par des milliers de personnes à travers le monde.
* Un nœud complet est un nœud qui a validé indépendamment l'ensemble de la blockchain Bitcoin depuis le bloc Genesis miné par Satoshi en 2009.
* Plus il existe de nœuds actifs, plus le réseau est distribué et donc résilient.
* Il existe **plus de 19 000 nœuds complets publiquement joignables dans le monde, auxquels s'ajoutent de nombreux nœuds non joignables publiquement.**
* Tous les nœuds participants appliquent les mêmes règles de consensus.

---

>* **DIFFUSION ~ Informer le réseau que vous envoyez des bitcoins à quelqu'un.**
---

* Lorsque vous appuyez sur « Envoyer », votre portefeuille signe la transaction avec votre clé privée et la diffuse, informant les nœuds de votre intention de transférer de la valeur afin qu'ils puissent la valider.

---
>* **MEMPOOL ~ Salle d'attente des transactions**
---

* Il s'agit de la « salle d'attente » où les transactions valides restent en attendant d'être sélectionnées par un mineur et intégrées à un bloc.

---
>* **BLOC ~ Une « page » du registre Bitcoin**
---

* Le registre distribué Bitcoin est constitué de « blocs » numériques.
* Chaque bloc contient des transactions bitcoin vérifiées qui maintiennent le registre mondial à jour. Il contient aussi notamment un nonce, un horodatage et l'empreinte du bloc précédent, éléments qui contribuent à l'immutabilité de la blockchain Bitcoin.

---
>* **BLOCKCHAIN ~ L'ensemble du registre Bitcoin**
---

* La blockchain Bitcoin, également appelée timechain, est le registre distribué contenant tous les blocs et toutes les transactions bitcoin effectuées depuis le bloc Genesis miné par Satoshi en 2009.

---

>* **MINEUR ~ Un nœud spécialisé qui confirme des transactions en les intégrant à des blocs et participe à l'émission de nouveaux bitcoins**
---

* Les mineurs Bitcoin sont des ordinateurs spécialisés. Ils consacrent une importante puissance de calcul — le hashrate — à une loterie numérique consistant à chercher une valeur permettant de produire une empreinte inférieure à la cible de difficulté actuelle, et ainsi à « miner » un bloc.
* Un bloc miné est horodaté puis ajouté à la blockchain, ou timechain.

---
>* **DIFFICULTÉ ~ Un mécanisme adaptatif qui permet de maintenir prévisible le rythme d'émission des nouveaux bitcoins.**
---

* C'est l'une des solutions ingénieuses de Satoshi pour empêcher que l'émission de bitcoins n'accélère avec l'apparition d'ordinateurs plus puissants.
* Lorsque davantage de puissance de minage rejoint le réseau, la cible devient plus difficile à atteindre.
* Lorsque moins de puissance de minage est présente, elle devient plus facile à atteindre.
* La difficulté **s'ajuste automatiquement tous les 2016 blocs** — environ toutes les deux semaines — afin de maintenir un rythme prévisible d'environ un bloc toutes les dix minutes.

---
>* **NONCE ~ Une valeur que les mineurs font varier lors du hachage**
---

* Les mineurs font varier le nonce et d'autres données du bloc afin de produire différentes empreintes et tenter d'atteindre la cible de difficulté.
* Lorsqu'un mineur produit une empreinte inférieure à la cible actuelle, il a trouvé un bloc : il peut le proposer au réseau et réclamer la récompense correspondante.

---

>* **HORODATAGE ~ Indication du moment associé au bloc**
---

* Chaque bloc miné comporte un horodatage.
* Il contribue notamment au fonctionnement du réseau et à l'ajustement de la difficulté.

---
>* **IMMUTABILITÉ ~ Extrêmement difficile à modifier rétroactivement.**
---

* Plus un bloc est profondément enfoui sous de nouveaux blocs, plus modifier son historique demanderait de refaire une quantité considérable de preuve de travail.

---
>* **PREUVE DE TRAVAIL (PoW) ~ Preuve cryptographique qu'un travail de calcul coûteux a été effectué afin de satisfaire une cible.**
---

* Les mineurs utilisent la preuve de travail en consacrant de la puissance de calcul et de l'électricité à la recherche de blocs. Ce mécanisme permet au réseau décentralisé de converger vers un historique commun et rend coûteux le spam ou la réécriture de l'historique.

---
>* **CRYPTOGRAPHIE À CLÉ PUBLIQUE ~ Procédé utilisant des paires de clés cryptographiques**
---

* Il s'agit d'un système dans lequel une clé privée permet de produire des signatures numériques qui peuvent être vérifiées à l'aide de données publiques correspondantes.
* **Les informations publiques** peuvent être utilisées pour recevoir des bitcoins.
* **La clé privée** doit rester secrète : elle permet de signer les transactions dépensant les bitcoins contrôlés par cette clé.
* **Vous devez protéger soigneusement votre clé privée**, car toute personne qui y a accès peut potentiellement dépenser vos bitcoins.

---

>* **RÉSEAU PAIR À PAIR (P2P) ~ Réseau décentralisé sans intermédiaire central**
---

* Les nœuds complets — les pairs — maintiennent collectivement un réseau pair à pair pour valider et relayer transactions et blocs.
* Dans ce type de réseau, chaque nœud peut fournir et demander des données à ses pairs.
* Il n'y a pas de gardien central dans un réseau P2P.

---
>* **LIGHTNING NETWORK ~ Réseau construit au-dessus de Bitcoin permettant d'envoyer ou de recevoir des sats très rapidement et à très faible coût.**
---

* Lightning est une solution de seconde couche (Layer 2). Il permet à Bitcoin de traiter un nombre beaucoup plus important de paiements sans inscrire chaque paiement individuel sur la chaîne principale.

---
>* **PORTEFEUILLE ~ Un « wallet » gère les clés cryptographiques permettant de contrôler vos bitcoins.**
---

* Il peut prendre la forme d'une application sur téléphone ou ordinateur, ou d'un appareil matériel dédié.
* Un portefeuille bitcoin serait plus précisément décrit comme un dispositif de signature : les bitcoins ne sont pas physiquement « contenus » dans le portefeuille ; ils sont représentés par des sorties de transaction sur le registre Bitcoin.
* Lorsque vous souhaitez envoyer ou dépenser vos bitcoins, le portefeuille signe la transaction puis la diffuse sur le réseau afin qu'elle puisse être validée et, pour une transaction on-chain, intégrée à un bloc.

---
>* **DÉVELOPPEURS ~ Programmeurs informatiques**
---

* Des cypherpunks et programmeurs qui maintiennent les logiciels, améliorent la sécurité, recherchent les bugs, proposent des pull requests, relisent celles des autres et auditent le code.

---

>* **CLÉ PUBLIQUE ~ Donnée cryptographique dérivée d'une clé privée**
---

* Elle sert notamment à vérifier des signatures. Les adresses utilisées pour recevoir des bitcoins sont dérivées de données publiques, mais une adresse Bitcoin n'est pas, au sens strict, simplement une clé publique.

---
>* **CLÉ PRIVÉE ~ Secret permettant d'autoriser la dépense de bitcoins**
---

* Une clé privée bitcoin est une valeur secrète qui permet de signer les transactions dépensant les bitcoins qu'elle contrôle.
* Vous devez la conserver en sécurité : toute personne qui l'obtient peut potentiellement dépenser ces bitcoins.

---
>* **REGISTRE DISTRIBUÉ ~ Registre vérifié indépendamment par les participants qui le souhaitent.**
---

* Au lieu d'un registre contrôlé de manière centralisée et invisible au public, comme celui tenu par une banque, Bitcoin possède un registre ouvert et décentralisé que chacun peut vérifier.
* Les transactions font référence à des adresses ou scripts, pas à des noms civils.
* Bien que Bitcoin soit pseudonyme, il est possible d'analyser et de suivre les transactions, notamment lorsque les bitcoins ont été achetés sur une plateforme centralisée appliquant le KYC.
* Le réseau Bitcoin permet à chacun d'auditer les règles et l'historique sans devoir faire confiance à un teneur de registre central.

---

## PLUS D'INFORMATIONS SUR LE MINAGE
![whatsminer](figure-07-whatsminer.png) Whatsminer M50S

![Antminer](figure-08-Antminer.png) Antminer S21 Pro

![Bitaxe](figure-09-Bitaxe%20.png) Bitaxe 401 Supra

* **Les mineurs consacrent de la puissance de calcul — le hashrate — et de l'électricité au réseau** afin de produire des blocs pour la blockchain Bitcoin.
* Ces machines fonctionnent 24 heures sur 24, seules ou regroupées par dizaines, centaines ou milliers.
* **Elles participent en quelque sorte à une loterie. Lorsqu'une machine trouve une combinaison de données** produisant une empreinte conforme à la cible de difficulté, **le mineur peut proposer le bloc suivant de la timechain.**
* **C'est cette preuve de travail (PoW) qui sécurise la création de nouveaux blocs et accompagne l'émission des nouveaux bitcoins.**

---

## RÉCOMPENSE DE BLOC BITCOIN
**= Subvention + Frais**

>* **Pour leur travail, les mineurs reçoivent :**
> * **Une subvention de bloc sous forme de bitcoins nouvellement émis.**
> * **Les frais des transactions incluses dans ce bloc.**

* **Lorsque vous envoyez une transaction bitcoin on-chain, elle peut inclure des frais** afin d'inciter un mineur à l'intégrer dans un bloc.
* La **subvention de bloc** est divisée par deux environ tous les quatre ans.
* Elle est **actuellement de 3,125 bitcoins** par bloc miné.
* **Le prochain halving est attendu en 2028**, après quoi la subvention passera à 1,5625 bitcoin par bloc.
* Comme indiqué plus haut, **cela contribue à maintenir une émission monétaire prévisible.**
* **Vers l'année 2140, la dernière fraction prévue de bitcoin sera émise.**
* Après cela, les mineurs seront rémunérés uniquement par les frais des transactions incluses dans les blocs.

>*Dans quelques décennies, lorsque la récompense deviendra trop faible, les frais de transaction constitueront la principale rémunération des nœuds (mineurs).*

~ Satoshi Nakamoto
Bitcointalk.org, 2010-02-14

>* **Les mineurs resteront nécessaires pour produire les blocs et contribuer à maintenir le réseau à jour et sécurisé.**

* Il faut tenir compte des coûts et la rentabilité du minage domestique peut être faible, mais miner chez soi peut contribuer à la décentralisation et à la robustesse du réseau.
* Les machines de minage peuvent fonctionner pendant de nombreuses années. Certains Antminer S9, par exemple, fonctionnent depuis plus de six ans.
* Lorsqu'elles sont retirées du service, **elles peuvent être démontées et recyclées.**
* **De nombreuses innovations intéressantes se développent autour de la récupération de chaleur :** chauffage de maisons, saunas, serres, jacuzzis, séchage d'aliments ou de bois, etc.

---
