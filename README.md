# Surface-Crack-detection

Web-application based on ML model to detect crack in an image.

## Description
The idea of the project is to detect the crack in the image for that we used two models exception and resnet and for ui we have used flask.

Datasets used in this project
*concret images-https://data.mendeley.com/datasets/5y9wdsg2zt/1/
*It consist of 40000 images 20000 as cracked one and 20000 no crack images.


## Getting Started

1) Change directory
    ```
    $ cd crack_detection
    ```

2) Install Requirements
    ```
    $ pip install -r requirements.txt
    ```
3) Train Model 
   
   Skip this step if you want to use pretrained model
   
   Tested with python 3.9
   ```
   $ python models/model.py
   ```
4) Run Server
   ```
   $ python app.py
   ``` 
5) Open http://127.0.0.1:5000/ in browser and use the UI to test concrete crack detection.

6) Try CURL requests
   ```
   $ curl -X POST -F file=@data/train/crack/15000_1.jpg http://127.0.0.1:5000/predict
   
   {"prediction":"crack"} 
   ```

## UI Screenshots
![2022-11-16 (3)](https://user-images.githubusercontent.com/67963861/202159907-8174b896-2044-48e6-b405-a4ee42a834ae.png)
![2022-11-16 (2)](https://user-images.githubusercontent.com/67963861/202159850-1ffbb5ff-dd16-41a0-b754-1b54800e02a5.png)
