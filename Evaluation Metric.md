# Evaluation Metric    
Assembled by Sohyeon Yim (2020-06-28)   

## 👀  Regression Model의 경우    
### MSE   
### RMSE    
### MAE   
### MAPE   
### R sqaured   
### Adujusted R squared   

## 👀  Classification Model의 경우 -> Confusion Matrix    
### Accuracy(정확도)   

### Precision(정밀도)      
* 모델이 1이라고 분류해낸 그룹 A가 있을 때, 모델이 얼마나 믿을 만한 정도로 A를 만들어 냈는지 평가   

### Recall(재현도)      
* 모형의 실용성과 관련된 척도   

### F beta Measure   
![fb score](https://user-images.githubusercontent.com/44013936/85926952-cd4ed400-b8dd-11ea-946d-6c41af678041.JPG)
* general formula for positive real β, where recall is considered β times as important as precision   
* 실무에서는 F1-measure보다 F-beta measure를 더 많이 쓴다. precision이나 recall에 가중치를 주고 싶을 때, 이 식을 사용하면 된다. precision에 가중치 3을 주고 싶으면 β에 1/3을 대입하면 된다. 한편 recall에 가중치 3을 주고 싶으면 β에 3을 대입하면 된다.    

#### F1-Measure (beta = 1.0)   
* Balance the weight on precision and recall   
![image](https://user-images.githubusercontent.com/44013936/85926656-d3dc4c00-b8db-11ea-8bcc-27d1285d66f7.png)

#### F0.5-Measure (beta = 0.5)      
* more weight on precision, less weight on recall    

#### F2-Measure (beta = 2.0)   
* less weight on precision, more weight on recall    

### Sensitivity(민감도)    
### Specificity(특이도)   

## 👀  Object Detection Model의 경우    
### AP   
### mAP   
### IoU  
### AR   
### FPS   



## Reference & Additional Resources    
[A Gentle Introduction to the Fbeta-Measure for Machine Learning](https://machinelearningmastery.com/fbeta-measure-for-machine-learning/)
