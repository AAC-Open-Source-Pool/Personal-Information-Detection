# <p align="center">Personal Information Detection</p>

<p align="center">This project scans for any personal information in images that you wouldn't want out in the internet (like phone numbers, credit card numbers, names, addresses, IP addresses, etc) by using Optical Character Recognition, Natural Language Processing, Regular Expressions and object detection systems.</p>

Personal Information in images is often overlooked, especially when posting to sites like Instagram where everyone can see the pictures you upload. People seldom check if there is any information in the background of their pictures that might leak personal information on a public site. My project tries to automate this process by checking the image for information that can be harmful if leaked in the public.

## Requirements
|||
|--|--|
|[python 3.10.12](https://www.python.org)|<img src="https://imgur.com/5U1Qas4.png" width="130px" height="30px"></a><br>|
|[flair 0.12.2](https://github.com/flairNLP/flair)|<img src="https://i.imgur.com/4fOVzrO.png" width="130px" height="30px"></a><br>|
|[streamlit 1.27.1](https://streamlit.io)|<img src="https://i.imgur.com/KUaORTO.png" width="130px" height="30px"></a><br>|
|[easyocr 1.7.1](https://pypi.org/project/easyocr/)|<img src="https://imgur.com/prDaufp.png" width="130px" height="30px"></a><br>|
|[matplotlib 3.8.0](https://matplotlib.org)|<img src="https://imgur.com/u5TmBrV.png" width="130px" height="30px"></a><br>|
|[opencv 4.8.1.78](https://pypi.org/project/opencv-python/)|<img src="https://imgur.com/jEJpm7H.png" width="130px" height="30px"></a><br>|
|[numpy 1.26.0](https://numpy.org)|<img src="https://imgur.com/bQ6fhnn.png" width="130px" height="30px"></a><br>|
|[regex 2023.8.8 ](https://docs.python.org/3/library/re.html)|<img src="https://i.imgur.com/xQ8Kvmu.png" width="130px" height="30px"></a><br>|

## Installation and usage
- Clone the repository
- If you have a supported GPU, download CUDA and CUDNN on your system for faster running of the detection algorithm
- Install [Darknet](https://github.com/AlexeyAB/darknet) for object detection by following the instructions [here](https://github.com/AlexeyAB/darknet#how-to-compile-on-linux-using-make)
- Download and unzip darknetconfig.zip from the releases tab
- place the files from darknetconfig.zip in the following directories:
    `./darknet/cfg/yolov4-obj.cfg`
    `./darknet/data/obj.data`
    `/darknet/yolov4-obj_best.weights`
- Run `pip install -r requirements.txt` to download all necessary dependencies
- Run `streamlit run pii.py` to run the detection algorithm, and upload the picture to the website opened.

