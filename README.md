# MolDesigner \[NeurIPS 2020 Demo\]

#### Live website: [deeppurpose.sunlab.org](deeppurpose.sunlab.org).
#### DeepPurpose GitHub repo: [link](https://github.com/kexinhuang12345/DeepPurpose)

Authors: Kexin Huang, Tianfan Fu, Dawood Khan, Ali Abid, Ali Abdalla, Abubakar Abid, Lucas M. Glass, Marinka Zitnik, Cao Xiao, Jimeng Sun

The efficacy of a drug depends on its binding affinity to the therapeutic target and pharmacokinetics. Deep learning (DL) has demonstrated remarkable progress in predicting drug efficacy. We develop MolDesigner, a human-in-the-loop web user-interface (UI), to assist drug developers leverage DL predictions to design more effective drugs. A developer can draw a drug molecule in the interface. In the backend, more than 17 state-of-the-art DL models generate predictions on important indices that are crucial for a drug's efficacy. Based on these predictions, drug developers can edit the drug molecule and reiterate until satisfaction. MolDesigner can make predictions in real-time with a latency of less than a second.

This repository hosts a public code version of MolDesigner. In the official release, there is a molecule interface but it is a private module from the Gradio team. Thus, we are not able to release it. However, in this repository, we replace the molecule module with the SMILES string input as an example on how to use DeepPurpose and Gradio to design a powerful web UI. 

### Installation
```
conda install -c conda-forge rdkit
Pip install torch
pip install scikit-learn
pip install git+https://github.com/bp-kelley/descriptastorus
pip install pandas-flavor
pip install subword-nmt
pip install wget
pip install lifelines
pip install prettytable
pip install --upgrade ipykernel
pip install gradio
```

### Run

Checkout the jupyter notebook file in the repo and simply run the cell to generate the UI interface.

### Cite

If you find this useful, please cite us:

```
@article{huang2020moldesigner,
  title={MolDesigner: Interactive Design of Efficacious Drugs with Deep Learning},
  author={Huang, Kexin and Fu, Tianfan and Khan, Dawood and Abid, Ali and Abdalla, Ali and Abid, Abubakar and Glass, Lucas M and Zitnik, Marinka and Xiao, Cao and Sun, Jimeng},
  journal={arXiv preprint arXiv:2010.03951},
  year={2020}
}
```
