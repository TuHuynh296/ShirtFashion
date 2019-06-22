# ShirtFashion
Using Single Shot Multibox Detector (SSD) to detect person and upper of body and then classify each upper clothes with Convolution Neural Network (CNN) to predict multiple label with type and color of upper clothes. There are a total of 10 classes with 3 shirt classes (shirts, t-shirts, jackets) and 7 color classes (black, white, red, gray, yellow, green, blue) equivalent to 2 labels are type and color.

## Folder Structer
    .
    ├── loss                                    # the localization loss for bounding box offset prediction and the classification
    ├── models                                 
       ├── upper.h5                             # model detect upper body
       ├── person.h5                            # model detect person
       ├── upper clothes.h5                     # model classify shirt of upper 
    ├── ShirtFashion.ipynb                      # Combine models to detect and classify shirts
    ├── Train_Clothes.ipynb                     # create model upper clothes with CNN
    ├── detect person and upper.ipynb           # create two models detect person and upper with SSD
    ├── lablebin.pickle                         # multiple lables for model "upper clothes"
    └── README.md


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

```
Python 3.x
Keras
Tensorflow
Single Shot Multibox Detector With Keras - by author pierluigiferrari
```

### Installing

A step by step series of examples that tell you how to get a development env running

Install from PyPI
* [python3.x](https://www.python.org/downloads/)
* pip install keras
* pip install tensorflow
* [ssd_keras](https://github.com/pierluigiferrari/ssd_keras) - by author pierluigiferrari

## Running the tests
```
*Steps: 
1. Clone ssd_keras to your computer: !git clone https://github.com/pierluigiferrari/ssd_keras
2. Place files of this project to folder ssd_keras after cloned
3. Run file ShirtFashion.ipynb to review summary of models

```
### Examples

![example1](https://github.com/leavin296/ShirtFashion/blob/master/example/example1.png?raw=true)
![example2](https://github.com/leavin296/ShirtFashion/blob/master/example/example2.png?raw=true)
![example3](https://github.com/leavin296/ShirtFashion/blob/master/example/example6.png?raw=true)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

