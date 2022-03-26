# Projet_Advanced_DL

Notre projet porte sur le thème du oneshot learning pour la reconnaissance d'animaux.
Certains animaux rares et/ou vivants dans des habitats extrêmes sont rarement photographiés par l'homme. Construire un modèle capable d'apprendre à reconnaître des animaux à partir d'un seul cliché peut donc avoir des applications intéressantes.

Pour ce projet, nous utiliserons la base LHI-Animal-Faces ( https://vcla.stat.ucla.edu/people/zhangzhang-si/HiT/exp5.html?fbclid=IwAR1u7ujdsYO9xw2dPGW-hTZd3x4dAJSeZEovJqodcPvnCp32ViTzaG9bjwQ ) contenant 100 images de 20 animaux différents (2000 images au total).

Dans un premier temps, nous avons choisi 5 animaux "rares" dont nous conservons un unique cliché. (Les autres clichés de ces animaux serviront pour tester le modèle). Selon la stratégie, les 15 autres animaux peuvent servir ou non à préentrainer un modèle, afin de pouvoir exploitier un modèle spécialisé dans la détection d'animaux.

Nous avons alors entraîné plusieurs modèles avec différentes stratégies afin d'évaluer et de comparer leur performance vis-à-vis de cette tâche de oneshot learning :
- 1-NN
- CNN simple
- Transfer learning à partir d'un EfficientNet
- Réseaux siamois
- Modèle CLIP par OpenAI (spécialisé dans le zero shot learning)


| Model | 1-NN | CNN | Transfer Learning | Reseaux Siamois | CLIP |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| Accuracy | 25,3% | Accuracy | 70% | Accuracy | 97% |
