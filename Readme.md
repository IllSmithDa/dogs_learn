# Goal

  1. Create a learning language model that can take an image of a dog and predict the correct breed of dog.

  2. Create a simple summary of the dog breed.

  3. Use this project to explore torch, torchvision, and other related libraries, including huggingface

  4. Explore and utilize existing image databases on sites like Kaggle

  5. Automate the process of downloading the data set and cleaning the data if necessary.

  6. Explore how decreasing learning rate, increasing epochs, and different pretrained models affect performance, memory usage

  7. Push the project into a repository and build a simple full-stack application based on the model

       - client: https://github.com/IllSmithDa/animal-client
       - server: https://github.com/IllSmithDa/fast-server

# Important Notes

  * The right learning rate was between 0.0001 and 0.00005. Any higher learning rate decreased the consistency of the validation data set and causes possible overfitting. 

      - This is reminder for me that a learning rate that is too high can causes overfitting and will causes the model to struggle to handle new data

      - https://www.baeldung.com/cs/ml-underfitting-overfitting

  * While the graph does say test loss and accuracy, its is actually the validation loss and accuracy. 

  * It is important to keep the transforms configuration mostly the same (apart from from horzontal flips) when training and using the model in real world application

  * Hive AI has been used for handling the generation of random dog facts. The Llama 3.2 1B Instruct model has been chosen specifically for its low cost while still being effective for the simple task. 

# Project Status

  * The project has mostly been completed by successfully training a model using the Efficient_B1 pretrained model using a learning rate of 0.00005 and 8 epochs.

    - Model 4 and graph 4

  * The quality of the dataset could be better, and as a result, the accuracy, especially during the test phase, will rarely rise above 83 percent.

  * The model has been consumed by a full-stack application built by me

      - https://illsmithda.github.io/animal-client/