# Music-Genre-Classification

Classification of the music genres is one of the most challenging tasks in the real world. In this paper, we classify the music based on its genres by using deep learning techniques. Music has a prominent place in this world. Music is an emotional experience. People play music based on their situation and genre. Music taste varies from person to person. Categorising music files consistent with their genre is a difficult project within the area of track information retrieval (MIR). In this project, we take a look at the performance of deep learning techniques. First, convert the music audio to a spectrogram by using **librosa**. The second is a combinatorial approach of finetuning and classification model education to the model to predict the genre label entirely using its spectrogram by using **keras** and **tensorflow**. We trained six deep learning classifiers with those capabilities and compared their overall performance.

Audio to Spectogram

![image](https://github.com/Vedavathi-nalla/Music-Genre-Classification/assets/68542087/205add81-1ced-46a4-b896-af897521b3ab)

In order to make training resources and time efficient, deep learning algorithms are used for integrating data from existing neural networks into a new neural network model. This can improve the accuracy of the new neural networks.  An already trained model can be tweaked or fine-tuned to perform a second, similar task after it has already been trained for the first. The input for a neural network is similar to a pre-trained model, it becomes an easy task to program a new model based on a pre-existing model. The first step is loading the ImageNet data for the pre-trained model. The second step is to remove the output layer of the pre-existing neural network as it will give the output for the ImageNet. If we continue without removing the output layer then we will get the output as ImageNet not as music genre we are removing the output layer for the pre-existing neural network. The third step depends upon the similarities of both of the models. In this we will add or remove the layers depending on the similarity of the two models. Once we added or removed then we froze the layers in the new model. Freezing the layer means the layer does not need to be modified of the data contained in them. The weights in them will not be updated when we train it. The final step is training the new model on the music genre data. The input layer is modified to get the output as classification of music. The weights of all other layers are the same; only the input layer is trained for the classification of music. The output layer displays the classification of the music genres.

**Result Analysis:**

All models used spectrogram images as input which means amplitude provides the information about intensity and how loud audio is, the frequency provides information about the sound and frequency varies with respect to time. Every model runs up to 50 epochs which took long time but we got good accuracies for every model except DenseNet.

![image](https://github.com/Vedavathi-nalla/Music-Genre-Classification/assets/68542087/f7b4d6d2-909c-4b5b-9025-efa7819d5e54)

From the above figure we can say that ResNet has the highest accuracy which means for the classification of music genres we can use ResNet50 to get the maximum perfection in classification of music genres.

![image](https://github.com/Vedavathi-nalla/Music-Genre-Classification/assets/68542087/133b9a4b-03c4-457b-843b-463b04e39c73)

The above diagram describes about the Depth of each and every model. DenseNet has the highest Depth because in this we take input as all previous layers feature map and depth also increased. 

In this project we learnt how to classify the music genre from the audio file which is a challenging task. We proposed two steps to classify the music genres from audio files that is first step convert the audio into spectrogram images, second step is executing the all the classification algorithms and comparing them with their accuracies. We can see that ResNet50 has the highest accuracy to classify the music genres In ResNet we used the Residual Blocks and we used the shortcut connections which can skip the 3 layers and also, we use the 1*1 convolutional layer added to it.
