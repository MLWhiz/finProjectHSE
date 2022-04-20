
# Project Description:
In this project we will create a simple object detection model and deploy it using FastAPI, Docker and Streamlit. 
The final output would look like:
[](final_output.png)

The final design looks like:
[](design.jpg)

# Dataset and Model:
We use a Pytorch pre-trained fasterrcnn_resnet50_fpn detection model from the torchvision.models for object detection, which is trained on the COCO dataset. 

# Run Instructions:

1. We need to start the fastAPI using Docker:

```
sudo apt-get update
sudo apt install docker.io

sudo service docker start
sudo service docker start

sudo docker build -t myimage .
sudo docker run -d --name mycontainer -p 80:80 myimage
```

2. Run streamlit app using:
```
streamlit run streamlitapp.py
```

3. Pass on a URL or a local image from your laptop to get predictions 
[](final_output.png)

