# jacob huang animal detector

Simply detects five different types of animals.

>>> demonstrates the output after running the model >>> <img width="1109" height="679" alt="imageTesting" src="https://github.com/user-attachments/assets/0baa9c5a-6139-48a2-b08c-d7e18b03c3ac" />


## The Algorithm

The algorithm is a trained image-detection resnet18 model. You send the model an image, the model processes it, and it outputs a "Class" (the name of the animal) with a percentage of confidence.

## Running this project

cd jacob-huang/huangfolder
NET=models/animals
DATASET=data/animals
sudo imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$DATASET/labels.txt $DATASET/path/of/your/file.jpg outputname.jpg

## you really dont have to do that much in terms of running it, but i suggest you import a few images from the web to see how they work with them.

>>> demonstrates how to use the detector >>> https://github.com/user-attachments/assets/c83ecad3-c4a6-4d4e-8d52-d8c4e377c7ea



