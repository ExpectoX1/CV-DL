 ## Blood Cell Subtypes Classification

Dataset- Blood Cell Images This dataset contains 12,500 augmented images of blood cells with accompanying cell type labels . There are approximately 3,000 images for each of 4 different cell types grouped into 4 different folders (according to cell type). The cell types are Eosinophil, Lymphocyte, Monocyte, and Neutrophil. This dataset is accompanied by an additional dataset containing the original 410 images as well as two additional subtype labels and also bounding boxes for each cell in each of these 410 images. The folder 'dataset2-master' contains 2,500 augmented images as well as 4 additional subtype labels.

![image](https://user-images.githubusercontent.com/79239242/110826686-561a6e00-82bb-11eb-831c-6391b9e6d218.png)

## Model Summary
![image](https://user-images.githubusercontent.com/79239242/110826870-85c97600-82bb-11eb-9fad-d4bcdf1f924e.png)

The above Convolutional Neural Network classifies the 4 classes of blood cells- Eosinophils, Monocytes, Lymphocytes and Basophiles after training. This model has 6 convolution layers, 2 dense layers, 7 dropouts and approximately 220K parameters. It gives 80% and 79% accuracy for 20 epochs.


## Accuracy Incrementation

Following methods were using in the above model to increase accuracy: 
Increased the number of convolution layers from 2 to 6 which caused a significant increase in accuracy. 
Decreased the number of neurons in the convolution layers and connecting layers which led to a huge increase in accuracy % 
The model started overfitting so we added Dropouts to the convolution layers and decreased the Dropout values from 0.7 and 0.5 to values of 0.4 and 0.3 in the connecting layer.


## Model Evaluation

Accuracy

![image](https://user-images.githubusercontent.com/79239242/110827050-b3aeba80-82bb-11eb-8749-88e080047ff0.png)

Loss
![image](https://user-images.githubusercontent.com/79239242/110827131-c5905d80-82bb-11eb-9ddf-fb7915d1a15b.png)
