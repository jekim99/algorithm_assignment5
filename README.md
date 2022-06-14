# Algorithm_03
대학원 컴퓨터공학과 2022120214 김재은
## Model 1

```
Model: "sequential"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv2d (Conv2D)              (None, 26, 26, 32)        320       
_________________________________________________________________
max_pooling2d (MaxPooling2D) (None, 13, 13, 32)        0         
_________________________________________________________________
flatten (Flatten)            (None, 5408)              0         
_________________________________________________________________
dense (Dense)                (None, 10)                54090     
=================================================================
Total params: 54,410
Trainable params: 54,410
Non-trainable params: 0
_________________________________________________________________
```
Trained for 5 epochs
### Test Accuracy
| Test loss | Test accuracy |
|:---------:|:-------------:|
|  0.110045 |    0.973100   |

### Success images
![1_succ](https://user-images.githubusercontent.com/11512879/173494260-3c7c03e9-8d70-449d-b9d3-04fbb13b94fa.png)

### Error images
![1_error](https://user-images.githubusercontent.com/11512879/173494272-05c40025-4a78-4657-bae3-51d0af98c6bc.png)

---
## Model 2
```
Model: "sequential_1"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv2d_1 (Conv2D)            (None, 26, 26, 32)        320       
_________________________________________________________________
max_pooling2d_1 (MaxPooling2 (None, 13, 13, 32)        0         
_________________________________________________________________
conv2d_2 (Conv2D)            (None, 11, 11, 64)        18496     
_________________________________________________________________
max_pooling2d_2 (MaxPooling2 (None, 5, 5, 64)          0         
_________________________________________________________________
flatten_1 (Flatten)          (None, 1600)              0         
_________________________________________________________________
dense_1 (Dense)              (None, 10)                16010     
=================================================================
Total params: 34,826
Trainable params: 34,826
Non-trainable params: 0
_________________________________________________________________
```
Trained for 5 epochs
### Test Accuracy
| Test loss | Test accuracy |
|:---------:|:-------------:|
|  0.062855 |    0.984500   |

### Success images
![2_succ](https://user-images.githubusercontent.com/11512879/173494435-803ab9da-3186-471f-a06a-788545f86b70.png)

### Error images
![2_error](https://user-images.githubusercontent.com/11512879/173494450-6e2bb107-0cb2-4dd0-90a0-15546e0135e4.png)

---
## Model 3
```
Model: "sequential_1"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv2d_2 (Conv2D)            (None, 26, 26, 32)        320       
_________________________________________________________________
max_pooling2d_2 (MaxPooling2 (None, 13, 13, 32)        0         
_________________________________________________________________
conv2d_3 (Conv2D)            (None, 11, 11, 64)        18496     
_________________________________________________________________
conv2d_4 (Conv2D)            (None, 9, 9, 64)          36928     
_________________________________________________________________
max_pooling2d_3 (MaxPooling2 (None, 4, 4, 64)          0         
_________________________________________________________________
conv2d_5 (Conv2D)            (None, 2, 2, 128)         73856     
_________________________________________________________________
flatten_1 (Flatten)          (None, 512)               0         
_________________________________________________________________
dense_1 (Dense)              (None, 10)                5130      
=================================================================
Total params: 134,730
Trainable params: 134,730
Non-trainable params: 0
_________________________________________________________________
```
Trained for 5 epochs

### Test Accuracy
| Test loss | Test accuracy |
|:---------:|:-------------:|
|  0.038928 |    0.987300   |

### Success images
![3_succ_5](https://user-images.githubusercontent.com/11512879/173494591-469fa23f-e40e-4a15-81ba-d5d6d44e0af2.png)

### Error images
![3_error_5](https://user-images.githubusercontent.com/11512879/173494612-c15c9dd9-677a-48f7-9ba9-8d3d1294f939.png)

