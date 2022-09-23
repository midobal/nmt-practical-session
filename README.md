# Neural Machine Translation: a Practical Session
This repo contains a [Google Colab](https://colab.research.google.com/) notebook which presents a practical session to introduce the training of neural machine translation systems to students. It was created for the lab sessions of the *machine translation* module of the [IARFID](https://www.upv.es/titulaciones/MUIARFID/) master from [Universitat Politècnica de València](https://www.upv.es/en).

You can open the notebook by cliking on [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/midobal/nmt-practical-session/blob/master/nmt-practical-session.ipynb).

## Overview
The goal of this lab session is to build machine translation systems based on neural networks (neural machine translation; NMT) from a dataset of bilingual parallel sentences using a [custom version](https://github.com/PRHLT/OpenNMT-py/tree/lab_sessions) of the **OpenNMT-py** toolkit (Klein et al., 2017).

### Dataset

The dataset we are going to use in this practical session is the Spanish–English language pair of the **EuTrans** corpus (Casacuberta et al., 2004), whose content involves the interaction of a customer with a receptionist at the frontdesk of a hotel. It comes with the custom version of **OpenNMT-py** that we are using. It is located at *OpenNMT-py/dataset/EuTrans*.

Here we can see an example of its content:

> *por favor, ¿nos puede dar la llave de la habitación?*

> *can you give us the key to the room, please?*

### Network description

The neural network that we are going to use for training the NMT system has the following configuration:

* Encoder and decoder are both Transformer with 64 neurons.
* 2 layers.
* Hidden Transformer feed-forward of size 64.
* 2 self-attention heads.
* Source word vector of size 64.
* Target word vector of size 64.

## Colab resources

* [Overview of Colaboratory](/notebooks/basic_features_overview.ipynb).
* [Guide to Markdown](/notebooks/markdown_guide.ipynb).
* [Importing libraries and installing dependencies](/notebooks/snippets/importing_libraries.ipynb).
* [Saving and loading notebooks in GitHub](https://colab.research.google.com/github/googlecolab/colabtools/blob/main/notebooks/colab-github-demo.ipynb).

## References

* Casacuberta, F., Ney, H., Och, F.J., Vidal, E., Vilar, J.M., Barrachina, S., García-Varea, I., Llorens, D., Hinarejos, C.D., & Molau, S. (2004). [Some approaches to statistical and finite-state speech-to-speech translation](https://doi.org/10.1016/S0885-2308(03)00028-7). Comput. Speech Lang., 18, 25–47.
* Klein, G., Kim, Y., Deng, Y., Senellart, J., and Rush, A. M. (2017). [OpenNMT: Open-Source Toolkit for Neural Machine Translation](https://www.aclweb.org/anthology/P17-4012). In *Proceedings of the Association for Computational Linguistics: System Demonstration*, 67–72.
