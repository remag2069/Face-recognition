# Face-recognition

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/16_7BgzzsmTO0dyA3e7usqVv5swUmCApi?usp=sharing)

implenting a face recognition algorithm using triplet loss 

Follow the google collab notebook for detailed explaination, the weightfile exceed 100mb, so it is saved on drive instead of on github, the code to download it is in the ".ipynb" file.

The algorithm is based on triplet loss function, inspired from the SOTA in face recognition "Facenet". The network is trained such that it generates 128 dimensional embedding for each image of a face passed to it. These embedding are generated such that faces from the same person are closer then faces from different ones in this high dimensional space.

Suprisingly,the network achieved a 64% accuracy on the LFW dataset even without any alignment software on just 10 epochs. The performance is lacking due to time and resources constraint, but it can be improved by:

1. Using 3-rd party face alignment algorithms
2. Increaseing network depth
3. Increasing image resolution being fed to the network
4. Increasing training epochs (might be prone to over fitting)

The suggestions are ordered in descending order of expected improvement in performance.
