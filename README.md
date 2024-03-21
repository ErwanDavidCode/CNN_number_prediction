# Presentation
Ce projet en Python utilise la librairie PyTorch pour prédire la valeur d'un chiffre représentée par une image (28x28x3). Ces images de chiffre ont des colorations différentes.

# Installation
- Installer les librairies Python
```sh
pip install -r requirements.txt
```
Lorsque le programme est executé, les fichiers suivants sont téléchargés en local dans le répertoire cloné : 
- __MACOSX
- customX_test
- customX_train.NPY
- customY_train.NPY
- dataset

Ils représentent les données d'entraintement et de test. Ils ne pèsent pas beaucoup plus que 50Mo. Ils peuvent être supprimés sans problème.

# Configuration de l'algorithme
Les valeurs internes utilisées pour l'algorithme peuvent être modifiés dans le fichier `Automaton_CNN_chiffres.py`.
Pour n'en citer que quelques-unes importantes :

```python
BATCH_SIZE = 64
EPOCHS = 10
lr=1e-4
```

|argument|type|description|
|-|-|-|
|BATCH_SIZE|int|La taille du batch de données utilisé pour l'entrainement|
|EPOCHS|int|Le nombre d'époch utilisé pour entrainer le modèle|
|lr|float|Le learning rate de l'optimizer ("Adam" ici)|


**Remarques** : Toutes les valeurs doivente être modifiées en connaissance de cause. Aucune vérification n'est effectuée sur la cohérence des valeurs.
La dernière partie "Interacion avec le modèle" ne peut être executée que dans google colab. Elle permet de dessiner des chiffres de manière interactive et de voir la prédiction associée du modèle.