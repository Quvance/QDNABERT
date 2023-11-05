# QDNABERT

This repository implements a transformer (DNABERT2) quantum hybrid. The BERT layers of the pretrained model are frozen and only the VQC layer is trained (fine-tuned).

Python 3.8, Ubuntu and CUDA 12 are required. A clean Anaconda/Conda environment is essential. Refer to setup instructions and QDNABERT2_env.yaml file.

Pennylane dependencies: https://docs.pennylane.ai/en/stable/development/guide/installation.html

Transfer example: https://pennylane.ai/qml/demos/tutorial_quantum_transfer_learning

A working BERT implementation can be found here (one line needs to be updated to make this work: q_out_elem = torch.hstack(quantum_net(elem, self.q_params)).float().unsqueeze(0)

Github link to the repo: https://github.com/sikfeng/quantum-transfer-learning-with-bert

The goal is to run this model on the GUE dataset which must be in the same directory as the finetuning folder (for details refer to classical DNABERT2 setup in this repo).

I have also uploaded a yml file, so you can see my Anaconda environment. My machine has a GForce RTX3070 GPU and Ubuntu is the OS

