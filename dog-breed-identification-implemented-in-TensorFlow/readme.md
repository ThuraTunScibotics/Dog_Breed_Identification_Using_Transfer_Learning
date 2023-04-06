## Dog Breed Identification
This notebook is about implementation of identifiying the breed of dog by transfer learning using MobileNetV2. The whole end-to-end multi-class image classifier is implemented with TensorFlow 2.0 and TensorFlowHub.
The dataset that is used for this is from Kaggle dog-breed-identification competition, please check the link: https://www.kaggle.com/c/dog-breed-identification/data
We have to predict the probabilities for each image of different breed in the test set. We can also predict on our own custom image.

End-to-end multi-class Dog Breed Classification is implemented in [dog_vision.ipynb](https://github.com/ThuraTunScibotics/Dog_Breed_Identification_Using_Transfer_Learning/blob/main/dog-breed-identification-implemented-in-TensorFlow/dog_vision.ipynb). The workflow steps are;
   1. Getting `images` and `labels`
   2. `Training` and `Validation` Split
   3. Turning images into `tensor` & resize the shape into (224, 224)
   4. Turning the images/data into `batches`
   5. Create a Model
   6. Add `TensorBoard_Callback` to save training log & `Early Stopping` to prevent overfitting
   7. Training the model both on `subset of data` & `full data` for results-comparisons
   8. Evaluate prediction using the trained model
   9. Save & Load the model
   10. Making the prediction on the `Test` dataset
   11. Create `CSV` file containing prediction probability for each breed for kaggle submission
   12. Prediction on Custom images
