# LanguageRecognition

Build an RNN model to recognize 17 language types including: 'Arabic', 'Danish', 'Dutch', 'English', 'French', 'German', 'Greek', 'Hindi', 'Italian', 'Kannada', 'Malayalam', 'Portuguese', 'Russian', 'Spanish', 'Swedish', 'Tamil', and 'Turkish'. The data is obtained from https://www.kaggle.com/datasets/basilb2s/language-detection/data.

The initial training data is as follows:
![image](https://github.com/tungheidiie/LanguageRecognition/assets/170008056/09d97433-155a-4513-a82c-0049599f09fe)

A chart of the number of samples for each language class.
![image](https://github.com/tungheidiie/LanguageRecognition/assets/170008056/56e1da9a-0327-4b47-9558-5ddbc0e8f632)

Split the data into 70% train, 20% validation, 10% test.

After the data is encoded through TextVectorization. The RNN model is constructed as follows:
![image](https://github.com/tungheidiie/LanguageRecognition/assets/170008056/849cf6a3-2e53-4810-b11a-fa1069e12677)

After training with 5 epochs:
![image](https://github.com/tungheidiie/LanguageRecognition/assets/170008056/64b13d58-8a34-4def-8bbd-7842f1f4ff84)

A chart of accuracy and loss over 5 epochs for the training and validation sets.
![image](https://github.com/tungheidiie/LanguageRecognition/assets/170008056/13abbce8-47ba-4880-93b0-312cc525a241)

Testing with the test data:
![image](https://github.com/tungheidiie/LanguageRecognition/assets/170008056/1e6be8fe-be46-4c27-b127-ba31e2f12cc9)

Testing with a text sample gives the result:

Language of 'En un hermoso día soleado, decidí salir a caminar por el parque cercano a mi casa, disfrutando de la brisa fresca y escuchando el canto de los pájaros en los árboles.': Spanish

Save the model to a file: language_recognition.keras
