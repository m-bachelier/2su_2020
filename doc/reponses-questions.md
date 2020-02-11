### Quels sont les chemins d'attaque possibles sur la signature d'un système embarqué?

- Récupérer physiquement sur l'appareil embarqué sa clé privée pour se faire passer pour l'appareil embarqué auprès du serveur
- Changer la clé publique du serveur par notre clé publique pour se faire passer pour le serveur et pouvoir communiquer avec l'appareil embarqué
- Trouver une faiblesse sur l'algorithme générant le jeu de clés, par exemple au niveau du générateur d'aléatoire (générateur déterministe)
- Si la clé publique est transmise par un canal non sécurisé on peut faire une attaque man in the middle et intercepter la clé lorsqu'elle transite afin de la remplacer par la notre

### A quoi sert la chaine de confiance? Pourquoi est-elle nécessaire?



### Décrire la méthode pour aborder la sécurité sur un produit embarqué. Pourquoi établir un modèle d'attaquant est-il important?

### Trouver un moyen rapide de faire du debug embarqué (par exemple sur cible ARM)? Expliquer les avantages

### Lister les catégories de bug possibles et comment les exploiter et les défendre

### Quelles idées pour améliorer la sécurité en embarqué? (IA, Anti-debug, Obfuscation, Crypto ...) Choisissez une idée, chercher si elle existe et développer en quelques phrases quel avantage elle apporte et ses limites