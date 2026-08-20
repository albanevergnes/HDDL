### Projet axé sur les architectures de Deep Learning génératives, en implémentant et optimisant un Conditional Variational Autoencoder (CVAE) en PyTorch sur le dataset Fashion-MNIST.

Objectifs du projet :

Étudier la théorie des VAE et l'apport du conditionnement (CVAE) pour guider la génération d'images à partir d'étiquettes de classes.

Concevoir et entraîner une architecture convolutive conditionnée pour reconstruire et générer des images ciblées d'articles de mode.

Évaluer l'impact de la fonction de perte et du paramètre de régularisation dans l'espace latent.

Travaux réalisés :

Modélisation & Architecture (PyTorch) :

Conception d'un encodeur convolutif (avec BatchNorm et ReLU) intégrant les images et les labels sous forme de cartes d'étiquettes étirées (One-Hot).

Utilisation de la technique de reparamétrisation (reparameterization trick) dans l'espace latent.

Implémentation d'un décodeur convolutif (ConvTranspose2d) conditionné pour la reconstruction des images.

Optimisation & Fonction de perte :

Combinaison de la perte de reconstruction (Binary Cross-Entropy) et de la divergence KL pour régulariser l'espace latent.

Analyse de l'impact du coefficient de pondération Beta sur le compromis entre fidélité de reconstruction et lissage de l'espace latent.

Entraînement avec l'optimiseur Adam sous environnement GPU (CUDA).

Génération & Validation :

Génération sous condition d'images synthétiques d'habits et chaussures (T-shirts, manteaux, baskets, etc.).

Visualisation et analyse comparative des reconstructions par rapport aux images d'origine.
