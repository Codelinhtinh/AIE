# Project Name
🌟Image Object Detection🌟

## Description
This is a FastAPI-based web service that accepts an image upload and performs object detection on the image using a pre-trained model Yolov5m. It returns the annotated image with the detected objects.

## Table of Contents
- [Installation](#installation)
- [Features](#features)
- [Usage](#usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)

## Installation
1. Clone the repository: 
```bash
git clone https://github.com/Codelinhtinh/AIE.git
```
2. Install project dependencies:
```bash
pip install -r requirements.txt
```
## Features
✨This code is a FastAPI application that provides an API endpoint for performing predictions on uploaded images.

✨ It uses a pre-trained model to detect objects in images. 

✨ Uploaded images are processed and resized to a specific image size defined in the CFG class. 

✨ The final results are visualized on the original image using the visualize function.

✨The processed and visualized image is saved to a temporary file and returned as a response to the API request.
## Usage
1. Run the FastAPI server in makefile:
```bash
uvicorn api:api --port 8000
```

2. Open your browser and navigate to `http://localhost:8000/docs` to check prediction.
![Alt Text](https://github.com/Codelinhtinh/Exercises-AIO/blob/main/sample/api.gif)

4. Start the streamlit app in makefile:
```bash
streamlit run app.py
```
4. Import image and wait:
![Alt Text](https://github.com/Codelinhtinh/Exercises-AIO/blob/main/sample/Usage.gif)

## Configuration
You can modify the configuration parameters of the model by updating the CFG class in the configs.py file. The available configuration options are:

**image_size**: The size of the input image for prediction.

**conf_thres**: The confidence threshold for object detection.

**iou_thres**: The IoU (Intersection over Union) threshold for non-maximum suppression.

Feel free to adjust these parameters according to your requirements.


## Contributing
🤝 Contributions are welcome! Please follow these guidelines when contributing to the project:
1. Fork the repository.
2. Create a new branch: 
```bash
git checkout -b feature/your-feature
```
3. Commit your changes: 
```bash
git commit -m 'Add your feature'
```
4. Push to the branch: 
```bash
git push origin feature/your-feature
```
5. Create a pull request.

## License
📝 This project is open source
