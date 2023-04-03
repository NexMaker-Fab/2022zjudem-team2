<!-- project/intro.md -->
# POUBELLE INTELLIGENTE
<br>

### I. Informations de base

Une bonne gestion des déchets est devenue une question essentielle pour notre planète. Dans les espaces publics et naturels, nombreux sont ceux qui ne prêtent pas attention aux déchets qu'ils laissent derrière eux. Lorsqu'il n'y a pas de collecteur de déchets disponible, il est plus facile de laisser les déchets sur place que de les ramener. Même les espaces dits préservés sont pollués par les déchets. C'est pourquoi notre système basé sur l'IA est conçu pour les maisons, les bureaux, les rues et les lieux publics. Il simplifie le recyclage, trie et compresse automatiquement les déchets, contrôle le niveau de remplissage et traite les données pour une gestion pratique des déchets.
<br><div class="loader"><img src="images/garbage1.jpg" alt="#" /></div>

<br>Pour préserver les zones naturelles, les maisons et les bureaux, il est important de fournir des points de collecte de déchets bien gérés:
<br><br>
<br>Pour éviter qu'ils ne débordent, les poubelles doivent être vidées régulièrement. Il est difficile de trouver le bon moment : trop tôt, et la poubelle peut être vide, trop tard et la poubelle peut déborder. Ce problème est d'autant plus critique lorsque la poubelle est difficile d'accès (comme sur les sentiers de randonnée en montagne)

<br><br><div class="loader"><img src="images/garbage2.jpg" alt="#" /></div>
<br><br>
Dans cette gestion rationnelle des déchets, le tri peut constituer un défi majeur. Les déchets organiques peuvent être directement traités par la nature, en compostage. Les déchets non organiques doivent être collectés pour être traités par des processus spécifiques.

<br><br>

<h1 style="font-size:1.5vw"><span style="color:black">But du projet</span></h1>

Le but de notre projet est de fournir un dispositif de supervision pour poubelle intelligente. Ce dispositif intègre plusieurs capteurs pour surveiller l'état de la poubelle.

- Capteur de niveau : basé sur un système ultrasonique, utilisé pour éviter les débordements en alertant l'équipe de collecte des déchets.

- Capteur de température et d'humidité : utilisé pour surveiller l'environnement des déchets. Cela peut être utile pour gérer l'état du compost organique et prévenir la contamination dans certains cas spécifiques (conditions très humides ou chaudes, risque d'incendie dans des conditions très sèches).

- Capteur de flamme : certains peuvent déposer des déchets incandescents (comme des mégots de cigarette) ou intentionnellement mettre le feu à la poubelle. Un incendie de déchets peut avoir des effets dramatiques sur l'environnement (par exemple, il peut causer un incendie de forêt). Le capteur de flamme peut alerter l'équipe de supervision sur le problème.

- Capteur d'humidité : pour le processus de compostage, il est important de maintenir un certain niveau d'humidité dans le matériau de compostage. Le capteur d'humidité inclus dans notre projet mesurera le niveau d'humidité sur le compost.

- Capteur d'ouverture : un détecteur d'ouverture sera installé sur le couvercle de la poubelle pour obtenir des statistiques sur l'utilisation des déchets et détecter une mauvaise fermeture.

- Capteur vocal : un microphone sera installé sur la poubelle (pour les maisons et les bureaux)

- Système de localisation : les déchets doivent être identifiés et localisés pour aider l'équipe de collecte des déchets dans leur gestion. Cela offrira plus d'agilité dans la gestion de la localisation des déchets, avec la possibilité de déployer des poubelles temporaires (par exemple en été sur la plage et les sentiers de randonnée, en hiver sur les pistes de ski, lors d'événements spéciaux tels que des compétitions sportives ou des festivals de musique).
<br>Le projet prend tout son sens avec une poubelle à deux compartiments :

- Un pour les déchets non-organiques.
- Un pour les déchets organiques avec un processus de compostage.
<br>
<br><br><br><br><div class="loader"><img src="images/garbage3.avif" alt="#" /></div>

<br>
<br><br>

<h1 style="font-size:1.5vw"><span style="color:black">Utilisation de Sigfox</span>(S'il vous plaît, spécifiez ce que vous voulez traduire en français.)</h1>

Les poubelles seront installées dans des zones isolées. L'alimentation sera assurée par une batterie, éventuellement connectée à un panneau solaire. Pour nous, Sigfox semble être une très bonne solution jusqu'à présent :

- Le système de communication Sigfox a une large couverture : cela permet de déployer le projet à grande échelle.

- Le système Sigfox offre des capacités de communication suffisantes pour notre cas d'utilisation.

- Sigfox peut fournir une solution de localisation de 100m : pas besoin d'ajouter un module GPS sur la poubelle.

- Sigfox est une solution à faible consommation d'énergie, ce qui permet au dispositif de fonctionner pendant longtemps de manière autonome.

<br><br>
<br>

### Détails du projet

Exemple de méthode de conception matérielle

<br><br><br><br><div class="loader"><img src="images/diagram.avif" alt="#" /></div>
<br><br>
<br><br>

<h1 style="font-size:1.5vw"><span style="color:black">Étapes du proje</span></h1>

<h1 style="font-size:1vw"><span style="color:black">Step 1: Comprendre Sigfox</span></h1>

Sigfox est une solution permettant de connecter des dispositifs dans le cadre de l'Internet des objets. Elle est actuellement utilisée dans plus de 45 pays et sur plus de 3 millions de dispositifs. Le message peut atteindre 12 octets avec un maximum de 140 uplinks et 4 downlinks par jour.

<h1 style="font-size:1vw"><span style="color:black">Step 2: Recherche de matériel</span></h1>

<br><br><br><br><div class="loader"><img src="images/harwares.avif" alt="#" /></div>

# 2. Suivi d'énergie du panneau solaire
Notre système de suivi d'énergie solaire est une technologie permettant d'orienter un collecteur solaire, un réflecteur ou un panneau photovoltaïque vers le soleil. Au fur et à mesure que le soleil se déplace dans le ciel, un dispositif de suivi s'assure que le collecteur solaire suit automatiquement et maintient l'angle optimal pour recevoir le plus de rayonnement solaire possible.