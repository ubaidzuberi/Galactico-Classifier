# Galactico-Classifier
Facial recognition software made using ML classification algorithms. This project used the pywavelet library and haarcascade files to recognise the faces.

## Final Deployed Product:
Default page:
<img width="1437" alt="Screenshot 2022-10-14 at 01 06 34" src="https://user-images.githubusercontent.com/113924862/196003463-5fe856b7-796b-4dbe-8c96-5f93dfd8cb59.png">
Output:
<img width="1440" alt="Screenshot 2022-10-14 at 01 08 49" src="https://user-images.githubusercontent.com/113924862/196003508-96d5ad38-7e23-4b04-b94a-56d638317d25.png">
Edge case (fails to identify):
<img width="1440" alt="Screenshot 2022-10-14 at 01 09 16" src="https://user-images.githubusercontent.com/113924862/196003535-1fbaa152-6679-446f-abfe-361c024a1cf8.png">

## Model:
This folder contains:
- A notebook which outlines the entire data cleaning, model builidng and validation process. The notebook is heavily annotated so it should be simple to follow
- A requirements.txt file which contains the names of the libraries that need to be installed for this project
- A folder called "dataset", this should contain subfolders that are named after the people that you are trying to recognise. Each folder should ideally contain atleast 100 high resolution images of that person

The program will first identify the faces and crop them. A folder called cropped will automatically be made in the dataset folder and it will contain         the cropped images in the correctly named subfolders. At this point, you will have to manually clean cropped folders because the sopftware may have made errors and we don't want to train the model with incorrect data.

## Server:
This folder contains:
- A folder called artifacts which contains the saved model
- A server.py which is the flask server
- The util.py file contains all the routines that have to be performed
- A folder called opencv which contains the relevent haarcascade files for this project
- A wavelet.py file which stores the code to perform the wavelet transform

## UI:
This contains:
- This folder contains the javascript, html and css files which were used to make the website
- It also contains dropzone files in css and js. These were used to create the image uploading option
- The images folder contains the images that were used in thee website
- As my foucs is on model building, the website isn't as aesthetic as it could be
