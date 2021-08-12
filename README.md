# Large-scale integrative analysis of soybean transcriptome using an unsupervised autoencoder model
===
# AutoEncoder for Data Compression
![](https://github.com/LingtaoSu/SoyMeta/blob/master/AutoEncoder.jpg)
We used one hidden layer for all the AE models, with the size set as half sample number, which results in a 50%-dimension reduction. The minibatch size is set to 12, and we trained the model with the Adam optimizer using a learning rate of 0.0001.  We used the ReLU activation to all layers except the last layer, where we applied softplus activation.

# Adversarial Deconfounding Autoencoder 
## Introduced by Paul G. Allen School of Computer Science & Engineering, University of Washington, Seattle
The ADAE (Adversarial Deconfounding AutoEncoder) approach to deconfound the gene expression latent spaces. The model consists of two neural networks: (i) an autoencoder to generate an embedding that can successfully reconstruct the original measurements and (ii) an adversary that is trained to predict the confounder from the embedding. The idea is to jointly train the networks to generate embeddings that can encode as much information as possible while not being able to predict the confounders. By applying AD-AE to two distinct gene expression datasets, we show that our model can (1) generate embeddings that do not encode confounder information, (2) conserve the biological signals present in the original space, and (3) generalize successfully across different confounder domains. We demonstrate that AD-AE can outperform standard autoencoder as well as other deconfounding approaches.
![](https://github.com/LingtaoSu/SoyMeta/blob/master/Pipeline.jpg)

