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
After training the model with `100 epochs`
|  Total Images  | 40 |
|   Dog Images   | 30 |
| Not Dog Images | 10 |
