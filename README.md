# Gesture_VQ-VAE
In Sign language, there exists no straighforward relationship between words and gestures, which makes it difficult to analyze and synthesize. In this project, the aim was to create a latent sign language embedding using a Vector Quantized Variational
AutoEncoder (VQ-VAE) to find new underlying structures to represent relevant gestures in sign language. The model was tuned and evaluated based on the Fréchet distance, perplexity, average jerk, and average acceleration metrics. The architecture of the VQ-VAE was largely based on the architecture of a VQ-VAE proposed in 'Bailando: 3d dance generation by actor-critic gpt with choreographic memory' [1].

## File overview

### Gesture_VQ-VAE.ipynb

This file contains the main components of the project, which are the model architecture, the training loop, and the evaluation metric calculations and visualizations of both the latent space and the output of the decodet of our model. It works based on the landmark data that was created in landmark_extraction.ipynb.

### landmark_extraction.ipynb

The funciton of this file is to create data for trianing the VQ-VAE, namely by extracting hand landmark data from sign-language image frames and storing them in .json files.

### architecture.pdf

This file contains a brief description and visualization of the model architecture of the VQ-VAE.


## References

[1] Li Siyao et al. “Bailando: 3d dance generation by actor-critic gpt with choreographic memory”. In: Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. 2022, pp. 11050–11059.
