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
![2022-11-16 (2)](https://user-images.githubusercontent.com/67963861/202162058-70a52063-9834-4191-b22f-a1e2827cd4a9.png)
![e195de1a-7a82-426b-9e44-7652e5989cbd](https://user-images.githubusercontent.com/67963861/202162095-b6f19536-8ce7-4a4f-9f66-17efa5876074.jpg)

