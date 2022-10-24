# image-creation-from-text-
<h3> Le but de ce projet est de former un réseau antagoniste génératif pour générer des images à partir d'une description textuelle.  </h3>
• Construction de modèles génératifs en utilisant des réseaux antagonistes génératifs (DCGAN)
• Construction d'un modèle discriminateur (Discriminator model)
• Développement d'un algorithme de training, qui crée les images, calcule la perte et ajuste les gradients.

The notebook has 5 parts:
<h3> - Data Pre-processing: </h3>
    - Converting the images into numpy arrays based on the pre-set pixel size and storing them.
    - Converting the image description into embeddings and storing them.
    - Sotring the captions in a csv file.
<h3>- Loading and Combining:</h3>
    - Loading all the images' numpy arrays and appending it to form the image data.
    - Loading the image description embedding numpy array.
<h3>- Data modeling: </h3>
    - Creating the discrimintor and generator networks.
    - Functions for calculating the discriminator and generator loss.
    - Setting the optimizer and learning rate.
<h3>- Training:</h3>
    - Function for the train step, that creates the images, calculates the loss and adjusts the gradients.
    - Function for the train, it fetches the batch data and passes it to train_step and collects all the metrics.
<h3>- Results:</h3>
    - Function for testing the output from the generator given an input noise and a caption
