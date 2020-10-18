# Sentence verification

Below are the results obtained for the sentence verification problem.

NOTE: In the notebook there is a more detailed explanation of each step taken along the process and the final conclusions.

Within the types of BERT architectures, XLM-RoBERTa [1] is selected, since is a promising multilingual language model that has been pretrained on one hundred languages. During the training phase techniques such as AdamW [2] and OneCycleLR [3] are used to provide a way to reach results as fast as possible.

<img src="https://github.com/jaime-cespedes-sisniega/sentence_verification/blob/main/img/train_val_phase.png">

<p align="center">
  <img src="https://github.com/jaime-cespedes-sisniega/sentence_verification/blob/main/img/val_pr_curve.png" width="600" height="400">
</p>

<p align="center">
  <img src="https://github.com/jaime-cespedes-sisniega/sentence_verification/blob/main/img/test_pr_curve.png" width="600" height="400">
</p>

<p align="center">
  <img src="https://github.com/jaime-cespedes-sisniega/sentence_verification/blob/main/img/confusion_matrix.png" width="470" height="350">
</p>

| Model | Precision | Recall | Average precision | F1-score |
| :---: | :---: | :---: | :---: | :---: |
| XLM-RoBERTa [1] (base) | 0.3824  | 0.6075 | 0.4797 | 0.4693|


## References

[1] Conneau, Alexis, et al. "Unsupervised cross-lingual representation learning at scale." arXiv preprint arXiv:1911.02116 (2019).

[2] Loshchilov, Ilya, and Frank Hutter. "Decoupled weight decay regularization." arXiv preprint arXiv:1711.05101 (2017).

[3] Smith, Leslie N., and Nicholay Topin. "Super-convergence: Very fast training of neural networks using large learning rates." Artificial Intelligence and Machine Learning for Multi-Domain Operations Applications. Vol. 11006. International Society for Optics and Photonics, 2019.
