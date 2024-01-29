# Projet de traduction automatique et assistée

## Description
Ce projet correspond à une analyse et une évaluation à grande échelle du moteur de traduction neuronale OpenNMT.

## Groupe
- Laura Darenne, Inalco
- Camille Clavier, Inalco

## Training et fichiers notebook
Toutes les run ont été faites sur google colab car nos ordinateurs n'étaient pas assez performants. Chacun des notebooks se trouvent directement dans les dossiers liés à chacune des runs : `./data/corpus_europarl/run*` et `.data/corpus_emea_europarl/run*`. Normalement, chacune des runs à son log du training : `train.log`. Le git OpenNMT (https://github.com/OpenNMT/OpenNMT-py) était cloné avant de commencer à faire tourner les fichiers jupyter.

## Evaluation
Les fichiers ont parfois été detokénisé pour refaire le test du score bleu. Nous avons utiliser le detokenizer de mosesdecoder (https://github.com/moses-smt/mosesdecoder/).

L'évaluation a été faite avec le fichier python `compute_bleu.py` reprise d'un repository de Yasmin Moslem (https://github.com/ymoslem/MT-Evaluation). Il nous a servi à calculer le score BLEU. Nous avons aussi testé le script `multiperl.perl` de mosesdecoder. Les résultats étaient très similaires.

<br>

*projet initialement fait sur gitlab*
