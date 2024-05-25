# Minerva-OSN

Official repository of the paper "Elephant in the Room: Surveying (and Rescuing) Online Social Network Research". 

In this repo, you can find:

  - The MINERVA-OSN dataset, which is compressed in a zip file
  - A copy of the survey we shared among OSN researchers.

##  Minerva-OSN  info
This repository contains the Minerva-OSN dataset. 
In the dataset, you can find scientific articles metadata such as *Title, Year, Venue, Authors, Abstract* that are related to Online Social Networks. 
Starting from 1 million articles gathered by Computer Science and Engineering Venues (conferences and journals) published after 2006, we looked for OSN (e.g., Facebook, Twitter) mentioned in the Abstract.
The Minerva-OSN dataset is the result of this process, and it contains all those scientific articles with **at least one mention**.
We highlight that, therefore, each paper in Minerva-OSN is linked with **one or more Online Social Networks**.

**NOTE**: we do not guarantee that our heuristic for gathering OSN scientific articles is perfect, and, therefore some articles might be missing or, vice-versa, we might include articles not relevant to the scope of this research.
Two experts manually evaluated the heuristic by inspecting the retrieved articles: this process allowed us to spot and address pitfalls such as false friends (the name of OSN might have multiple meanings -- like Faces). 
Therefore, the manual inspection phase reduced the introduction of erroneous articles in our dataset, making our contribution more robust. 

## Reproducibility
You can find the code to reproduce the topic modeling (*ipynb*). 
We executed the code in the following machine:
 - OS: Ubuntu 22.04 LTS
 - Machine Model: DELL ALIENWARE AURORA R15
 - Processor: 13th Gen Intel(R) Core(TM) i7-13700F   2.10 GHz
 - GPU: NVIDIA GeForce RTX 4070 Ti

The code can be executed in approximately 10 minutes. 
Note that we utilize LLAMA-2, to which you need to get access through HuggingFace. 
(https://huggingface.co/docs/transformers/main/model_doc/llama2)

**NOTE**: all our analyses involves *unsupervised machine learning* techniques. The various *hyperparameters* involved have been set by looking at state-of-the-art techniques and with manual analyses of two experts in the field.

