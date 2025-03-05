<h1>Weather Recognition</h1>

<h2>Introduction</h2>
This project aims to develop an intelligent system for classifying images into four weather categories: sunrise, sunny, rainy, and cloudy. By analyzing images captured at popular tourist destinations, the system will provide real-time weather updates, helping travelers plan their trips more effectively and enhancing their overall experience.

To achieve this, the project is structured into three key phases:

- Dataset selection & model choice: Identifying a suitable dataset and selecting the most appropriate machine learning model.
- Model training: Training the model to accurately recognize weather conditions in images.
- Model evaluation: Assessing the model's performance to ensure reliability and effectiveness.
- 
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


<h2>CNN Model & parameters</h2>

- 4 Hidden Layers
         Our model is able to take more details into
         consideration. Overfitting is still under control.

- 10 Epochs 
          A lower number of epochs drastically decrease the
          accuracy of our model. Overfitting is something to
          keep an eye on, but it's correct in most training sessions 

- 32 batch
          That is to say approximatively 8 iteration in each epoch

- ReLu function
            The most suittable function for high dimenssional data
  
- 1 minute of training

Between 0.6 and 0.8 Accuracy
Between 0.6 and 0.9 Validation Loss
(These number change depending on the training session)

<h2>Results interpretation</h2>

Strength of our model

Almost all Sunny and Snowy pictures are captured by our model (Accuracy), so users may not miss good oportunities. Users can easily avoid Foggy places (usefull for driving especially).

- Sunny: Accuracy : 92% ; Recall : 94 %
- Snowy: Accuracy : 93%  ; Recall : 88 %
- Foggy: Accuracy : 95% ; Recall : 100 %

Room for improvement
Users may trustfully avoid places labbeled as Rainy and Cloudy (Accuracy). Unfortunately users will eventually discover Cloudy or Rainy places (Recall) in other places. In the future we could train our model with more Cloudy pictures or eventually remove this class.

- Rainy: Accuracy : 88% ; Recall : 59 %
- Cloudy: Accuracy : 81% ; Recall : 30 %

<h2>Conclusion</h2>

This project developed an AI-based weather classification system to enhance tourism planning. We use a CNN model trained on Rome’s weather images, it achieved high accuracy for sunny, snowy, raineand foggy conditions but faced challenges with cloudy and rainy classifications. Future improvements could enhance recall by expanding the dataset. This work demonstrates AI’s potential in tourism and offers a solid foundation for further development.

