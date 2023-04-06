# Painting_Synthesis
Painting synthesis combining information retrieval and generative adversarial networks.
## Introduction
Generative Adversarial Networks are a recently introduced method for training generative models with neural networks. They follow an adversarial approach where two deep models gen- erator and discriminator compete with each other. They have been used for many applications especially for image synthesis because of their capability to generate high quality images. This project aims to implement a user-interactive Generative Adversarial Networks (GAN). Several im- provements are listed as follows:
* Implement Okapi BM25 model to do the image selection based on users’ queries.
* Mutli-taskCascadedConvolutionalNetworks(MTCNN)isusedtodothefaceextractionfor paintings whose genre is portrait.
* Modified VGG16 is used to act as the discriminator of the GAN model for paintings whose genre is landscape.
* Image interpolation is derived for latent points, where gradual changes from one image to another is visualized.
## Data Information
The data set is retrieved from Kaggle, which contains information for 11,175 paintings of many famous painters like Monet, Picasso, Van Gogh, and so on. There are seven attributes in- cluding Painter Name, Painting Name, Year painted, Genre, Style, Link for the image and 5 colors extracted from the image using Adobe Color. Genre and style are characteristics of paintings, which are categorical variables. Genres of paintings are either portrait or landscape, among which 6223 are portraits and 4952 are landscapes. Style includes Impressionism, Neo-Impressionism, Post-Impressionism, Realism, Cloisonnism, and Japonism.
