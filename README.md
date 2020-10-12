# Upload-file-to-ipfs

>Dans cette session du cours, vous apprendrez à charger un fichier sur IPFS depuis un client JavaScript. L'exercice peut paraître simple, mais comme il fait appel à plusieurs outils qu'il faut orchestrer de la juste manière, il est préférable de les introduire au préalable.

### - [FileReader](https://developer.mozilla.org/fr/docs/Web/API/FileReader)

>Nous aurons besoin tout d'abord de l'objet **FileReader** (natif à JavaScript) qui permet de lire le contenu de fichiers de façon asynchrone. On peut ainsi lire le contenu provenant d'un objet Blob (qui sera d'ailleurs la première partie de l'exercice lorsque nous tenterons de "_fetcher_" une URL distante vers un fichier brut en cross-domain et voudrons récupérer le Blob). Et l'on peut aussi lire, grâce à FileReader, le contenu d'un objet **File**, lorsque nous tenterons, dans un second temps de l'exercice, de charger un fichier sur IPFS depuis notre machine.

### - [IPFS](https://ipfs.io)

>IPFS est un système distribué de fichiers en **pair à pair** qui ne dépend pas de serveurs ~~centralisés~~. D'une certaine manière, IPFS est similaire au World Wide Web, à la différence qu'il peut être vu comme un essaim **BitTorrent** unique, qui échange des objets au sein d'un dépôt **Git**. IPFS n'a pas de point unique de défaillance et les **_nœuds_** n'ont pas besoin de se faire mutuellement confiance

### - [Infura](https://infura.io)

> Nous nous connecterons justement aux **_nœuds_ INFURA** pour l'exercice. Infura est une infrastructure publique et gratuite donnant accès au réseau Ethereum et IPFS pour les applications décentralisées, autrement connues sous le nom de "_dApps_".

### - [js-ipfs-http-client](https://github.com/ipfs/js-ipfs-http-client)

>Pour cela, nous aurons besoin de la librairie JavaScript **js-ipfs-http-client** permettant à notre  application d'ajouter un fichier à un nœud IPFS distant. De plus, cette librairie intègre un ensemble de fonctions utilitaires, comme la librairie **Buffer**, dont nous aurons besoin pour l'exercice.

## - [Buffer](https://github.com/feross/buffer)

>Buffer est une bibliothèque JavaScript totalement browser identique à celle du langage serveur, nodejs, qui fournit un mécanisme de lecture ou de manipulation de flux de données binaires.

### - [jsdelivr](https://www.jsdelivr.com)

>Et nous appeleront ces librairies via le **CDN** **jsDelivr**, qui occupe actuellement la 3ème place parmi les Content Delivery Network publics les plus populaires au monde. Actuellement, il peut servir des fichiers Web directement à partir du registre npm et des référentiels Github sans configuration.

:bulb: Lien vers la version courante **minifiée** de la librairie ipfs JavaScript sur jsdelivr

[ipfs-http-client](https://cdn.jsdelivr.net/npm/ipfs-http-client/dist/index.min.js)
