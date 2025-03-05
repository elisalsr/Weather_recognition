<h1>Weather Recognition</h1>

<h2>Introduction</h2>
This project aims to develop an intelligent system for classifying images into four weather categories: sunrise, sunny, rainy, and cloudy. By analyzing images captured at popular tourist destinations, the system will provide real-time weather updates, helping travelers plan their trips more effectively and enhancing their overall experience.

To achieve this, the project is structured into three key phases:

- Dataset selection & model choice: Identifying a suitable dataset and selecting the most appropriate machine learning model.
- Model training: Training the model to accurately recognize weather conditions in images.
- Model evaluation: Assessing the model's performance to ensure reliability and effectiveness.

This approach ensures a robust and efficient weather classification system tailored for tourism applications.

<br />


<h2>Description</h2>

Images from Rome during 5 different weather conditions.

50 images for each class:
- Sunny
- Rainy
- Cloudy
- Foggy
- Snowy


<h2>CNN Model & Parameters</h2>
         
- 4 Hidden Layers
The model captures intricate details while maintaining control over overfitting.

- 10 Epochs
Fewer epochs significantly reduce accuracy, while too many risk overfitting. Most training sessions maintain a good balance.

- Batch Size: 32
This results in approximately 8 iterations per epoch.

- ReLU Activation Function
The most suitable function for handling high-dimensional data.

Training Time: ~1 Minute

- Performance Metrics:

Accuracy: 0.6 – 0.8
Validation Loss: 0.6 – 0.9
(Values may vary across training sessions.)

<h2>Results interpretation</h2>

Strengths
Our model effectively captures Sunny and Snowy images with high accuracy, ensuring users don’t miss good weather opportunities. Additionally, it excels at identifying Foggy conditions, which is particularly useful for drivers.

- Sunny: Accuracy 92% | Recall 94%
- Snowy: Accuracy 93% | Recall 88%
- Foggy: Accuracy 95% | Recall 100%
  
Areas for Improvement
While users can reliably avoid locations labeled as Rainy or Cloudy based on accuracy, the recall scores indicate that some rainy and cloudy conditions may go undetected. To improve this, we could expand the training dataset with more Cloudy images or consider refining/removing this class.

- Rainy: Accuracy 88% | Recall 59%
- Cloudy: Accuracy 81% | Recall 30%

<h2>Conclusion</h2>

This project developed an AI-based weather classification system to enhance tourism planning. We use a CNN model trained on Rome’s weather images, it achieved high accuracy for sunny, snowy, raineand foggy conditions but faced challenges with cloudy and rainy classifications. Future improvements could enhance recall by expanding the dataset. This work demonstrates AI’s potential in tourism and offers a solid foundation for further development.

