## Dog Breed Identification using Pre-trained models: AlexNet, ResNet, VGG

**This is my first capstone project submitted by me for AI programming with Python Nano Degree Program on Udacity.**
- The main tasks of this project is to use the Python skills that I learned, and implement image classification algorithm not only for classifying images as "dogs" or "not dogs", but also to identify the breed if the image is classified as "dog".
- The *classifier function* `classifier.py` have been originally provided, and this function allows us to used deep CNNs pre-trained models/architectures; *AlexNet*, *VGG*, *ResNet*.  These different architectures are used to classify the images, and the classified results for each related architecture are later compared.
- It is also important to implement the required tasks (6 related python scripts/function) which can be seen in `check_images.py`, and these were done by using the Python conceps of Data Structure, Control Loop and so on.

**Finally, classification of images are taken on the provided "pet_images" and custom "uploaded_images" folders by running `check_images.py`**
```
python check_images.py --dir [<image-folder-name/] --arch [architecture-type] --dogfile dognames.txt
```

### Classfication Results

**classification on 'pet_images' folder**
|                |    |
| -------------  | -- |
|  Total Images  | 40 |
|   Dog Images   | 30 |
| Not Dog Images | 10 |

| CNN Model Architecture | % Not Dog Correct | % Dog Correct | % Breeds Correct | % Match Labels |
| ------ | -------- | -------- | ------------ | ------------ |
| **ResNet** |     90.0%     |     100.0%     |     90.0%        |       82.5%       |
| **AlexNet** |     100.0%     |      100.0%    |      80.0%      |        75.0%      |
| **VGG**    |  100.0 %     |     100.0%     |    93.3%     |   87.5%   |


**Tasks Questions and its answer regarding (uploaded_images) Classification:**

1. Did the three model architectures classify the breed of dog in Dog_01.jpg to be the same breed? If not, report the differences in the classifications.
      - Answer: 
        The two model architectures, 'vgg' and 'resnet' classified as rottweiler which is the SAME breed with the breed of dog in Dog_01.jpg. The 'alexnet'       model architecture classified as tibetan mastff which is NOT the same breed with original dog breed in Dog_01.jpg. So, the model architectures can       classify the SAME breed are 'vgg' and 'resnet'.



2. Did each of the three model architectures classify the breed of dog in Dog_01.jpg to be the same breed of dog as that model architecture classified Dog_02.jpg? If not, report the differences in the classifications.

      - Answer: 
        The 'resnet' model architecture classified both Dog_01.jpg and Dog_02.jpg as rottweiler, therefore, the 'resnet' model classified as the same             breed for this two images. The classified breed is also the same with original breed in images.

        The 'alexnet' model architecture did NOT classify as the same breed for the two images, because 'alexnet' classify Dog_01.jpg as tibetan mastiff          and Dog_02.jpg as kelpie, and not even same with original breed.  

        Since the 'vgg' model architecture classify Dog_01.jpg as rottweiler and Dog_02.jpg as miniature pinscher, 'vgg' model did NOT classify as the            same breed for the two images. But the model classified Dog_01.jpg as the same with original dog breed.



3. Did the three model architectures correctly classify Animal_Name_01.jpg and Object_Name_01.jpg to not be dogs? If not, report the misclassifications.

      - Answer: All the three model architectures classify Cat_01.jpg and Medicine_bottle_01.jpg with ClassLabelDog value '0' and also their                      pct_correct_notdogs is 100%. Therefore, the three models correctly classified Cat_01.jpg and Medicine_bottle_01.jpg to not dogs.



4. Based upon your answers for questions 1. - 3. above, select the model architecture that you feel did the best at classifying the four uploaded images. Describe why you selected that model architecture as the best on uploaded image classification.

      - Answer: Based on my answers above, I found that the 'resnet' model architecture is the best. The 'resnet' model classified both Dog_01.jpg and          Dog_02.jpg as rottweiler which is also the same breed with original breed in images. The model can also classified not-dog-images to be not dogs.         I also found the total runtime of the model is 0:0:0 which is quite fast. These are the reasons why I selected 'resnet' as the best model                 architecture for uploaded image classification.
