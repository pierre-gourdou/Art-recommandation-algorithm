The goal of this project is to create the recommandation algorithm for a web application that allows users to find art they truly like !
The app will work in 2 steps : 
 1) The user swipes through a dozen of art pieces 
 2) The application recommands art pieces tailored to their taste

### Dataset :
The dataset used for this project is a subset of the wikiart dataset (https://www.kaggle.com/datasets/steubk/wikiart). This subset contains 15133 pieces and the number of pieces per genre shown below : 

| Genre | # of Artworks |
|----------|----------|
| Baroque  | 4220  |
| Art Nouveau Modern  | 4125  |
| Abstract Expressionism  | 2592 |
| Cubism  | 2139  |
| Color Field Painting  | 1576  |
| Contemporary Realism  |  481 |

### Technical approach
The first step will be to embed all the artworks into a vector space using CLIP Model and the second will be to compute similarity search on those vectors. The objective is to build a function that returns the top 10 most similar artworks when given an artwork as entry.

### Embedding 
The embedding is made using CLIP, a powerful pre-trained autoencoder. 
![Texte alternatif](/assets/embedding.png "Titre de l'image")
