# Painting_Synthesis
Painting synthesis combining information retrieval and generative adversarial networks.
## Introduction
Generative Adversarial Networks are a recently introduced method for training generative models with neural networks. They follow an adversarial approach where two deep models generator and discriminator compete with each other. They have been used for many applications especially for image synthesis because of their capability to generate high quality images. This project aims to implement a user-interactive Generative Adversarial Networks (GAN). Several improvements are listed as follows:
* Implement Okapi BM25 model to do the image selection based on users’ queries.
* Mutli-task Cascaded Convolutional Networks (MTCNN) is used to do the face extraction for paintings whose genre is portrait.
* Modified VGG16 is used to act as the discriminator of the GAN model for paintings whose genre is landscape.
* Image interpolation is derived for latent points, where gradual changes from one image to another is visualized.
## Data Information
The data set is retrieved from Kaggle, which contains information for 11,175 paintings of many famous painters like Monet, Picasso, Van Gogh, and so on. There are seven attributes in- cluding Painter Name, Painting Name, Year painted, Genre, Style, Link for the image and 5 colors extracted from the image using Adobe Color. Genre and style are characteristics of paintings, which are categorical variables. Genres of paintings are either portrait or landscape, among which 6223 are portraits and 4952 are landscapes. Style includes Impressionism, Neo-Impressionism, Post-Impressionism, Realism, Cloisonnism, and Japonism. 
![pic](https://github.com/InCaseIDontCU/Painting_Synthesis/blob/main/截屏2023-04-06%2022.59.16.png)  
We also scatch the word cloud for our data containing relative information. 
![pic](https://github.com/InCaseIDontCU/Painting_Synthesis/blob/main/截屏2023-04-06%2022.59.45.png)  
## Algorithms
We apply MTCNN and GAN as our main algorithms, which could be found in our report. We take the image and resize it to different scales in order to build an image pyramid, which is the input of the three-staged cascaded network. Then we design the structure of GAN suitable for image synthesis.  
![pic](https://github.com/InCaseIDontCU/Painting_Synthesis/blob/main/截屏2023-04-06%2023.00.02.png)  
## Results
We show a brief demonstration of synthesis result here. You can also find image interpolation in our report.  
![pic](https://github.com/InCaseIDontCU/Painting_Synthesis/blob/main/截屏2023-04-06%2023.00.19.png)  
##Authors
