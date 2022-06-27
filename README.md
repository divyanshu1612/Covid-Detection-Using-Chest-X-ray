# covid-detection
Detecting if a lung x-ray is of covid positive person or of a normal person

![download (1)](https://user-images.githubusercontent.com/87748321/176020788-26b35dc5-ecdf-4372-b734-790189c6b2ba.png)

- Covid and normal images are loaded in grayscale and rescaled to (256,256) and then saved into a main directory inside respective sub-directories according to class names.
Data is divided into 70% ,15%, 15% for training, validation and testing resp.
Image masks are used to make only lung region visible and rest area black.

- Model is build having 3-Conv2D layers followed by Maxpooling and Dropouts to resist overfitting. 

- ImageDataGenerators are used to load trainging and validation data at training time.

- Trainging is done for 30 epochs and 89.3 % accuracy obtained on finally on testing data.

Dataset is taken from Kaggle names covid19-radiography-database available at following link :- https://www.kaggle.com/datasets/tawsifurrahman/covid19-radiography-database.

- M.E.H. Chowdhury, T. Rahman, A. Khandakar, R. Mazhar, M.A. Kadir, Z.B. Mahbub, K.R. Islam, M.S. Khan, A. Iqbal, N. Al-Emadi, M.B.I. Reaz, M. T. Islam, “Can AI help in screening Viral and COVID-19 pneumonia?” IEEE Access, Vol. 8, 2020, pp. 132665 - 132676. [Paper link](https://ieeexplore.ieee.org/document/9144185)
- Rahman, T., Khandakar, A., Qiblawey, Y., Tahir, A., Kiranyaz, S., Kashem, S.B.A., Islam, M.T., Maadeed, S.A., Zughaier, S.M., Khan, M.S. and Chowdhury, M.E., 2020. Exploring the Effect of Image Enhancement Techniques on COVID-19 Detection using Chest X-ray Images. [Paper Link](https://www.sciencedirect.com/science/article/pii/S001048252100113X?via%3Dihub)
