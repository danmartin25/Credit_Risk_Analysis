# Credit Risk Analysis

## Overview

Jill has asked us to used imbalanced-learn and scikit-learn libraries to evaluate different machine learning models using resampling. We will be using data from LendingClub. In total, there will be 6 different models we will be making: oversampling, SMOTE oversampling, undersampling, a combination of over and under sampling, Balanced Random Forest Classifier, and Easy Ensemble Classifier.

## Results

- Oversampling model
  - Balanced Accuracy Score: 0.657
  - Precision Score:
    - High Risk: 0.01
    - Low Risk: 1.00
    - Avg: 0.99
  - Recall Score:
    - High Risk: 0.71
    - Low Risk: 0.60
    - Avg: 0.60

  - Image:

![model 1](https://user-images.githubusercontent.com/91795475/153735994-f56d3cbc-f6b9-4eee-9759-af2b9baf14f8.png)


- SMOTE Oversampling model
  - Balanced Accuracy Score: 0.662
  - Precision Score:
    - High Risk: 0.01
    - Low Risk: 1.00
    - Avg: 0.99
  - Recall Score:
    - High Risk: 0.63
    - Low Risk: 0.69
    - Avg: 0.69

  - Image:

![model 2](https://user-images.githubusercontent.com/91795475/153735997-0dc97ad6-2a82-4375-9d0d-ad06cf3c429f.png)


- Undersampling model
  - Balanced Accuracy Score: 0.545
  - Precision Score:
    - High Risk: 0.01
    - Low Risk: 1.00
    - Avg: 0.99
  - Recall Score:
    - High Risk: 0.69
    - Low Risk: 0.40
    - Avg: 0.40

  - Image:

![model 3](https://user-images.githubusercontent.com/91795475/153736002-0e49dc6b-37e0-4311-b413-754091d3a61e.png)


- Combination model
  - Balanced Accuracy Score: 0.688
  - Precision Score:
    - High Risk: 0.01
    - Low Risk: 1.00
    - Avg: 0.99
  - Recall Score:
    - High Risk: 0.80
    - Low Risk: 0.57
    - Avg: 0.57

  - Image:

![model 4](https://user-images.githubusercontent.com/91795475/153736032-9607e359-a117-4440-9514-4cba44429bf1.png)


- Balanced Random Forest Classifier Model
  - Balanced Accuracy Score: 0.788
  - Precision Score:
    - High Risk: 0.03
    - Low Risk: 1.00
    - Avg: 0.99
  - Recall Score:
    - High Risk: 0.70
    - Low Risk: 0.87
    - Avg: 0.87

  - Image:

![model 5](https://user-images.githubusercontent.com/91795475/153736053-e731550b-2fc4-4df3-b495-2b160a8a1587.png)


- Easy Ensemble Classifier Model
  - Balanced Accuracy Score: 0.932
  - Precision Score:
    - High Risk: 0.09
    - Low Risk: 1.00
    - Avg: 0.99
  - Recall Score:
    - High Risk: 0.92
    - Low Risk: 0.94
    - Avg: 0.94

  - Image:

![model 6](https://user-images.githubusercontent.com/91795475/153736055-e1eab647-a7a8-46f6-b51b-35b275131430.png)


## Summary

Of the 6 models, the Easy Ensemble Classifier Model does the best in each of the categories of Accuracy, Precision, and Recall when compared to the other models. This model is the best out of the 6 we tested. My reccomendation for the use of this model depends on what the purpose is. The accuracy, precision, and recall (sensitivity) scores are all high, except for the high risk precision score. This means that a significant amount of loans classified as high risk are actually low risk. I would theorize that this actually helps the credit card company. They will charge higher interest rates because they think the risk is high, but the risk is actually lower and the customer is more likely to pay it back than projected. This theory assumes that the credit card company wants their payments on time and in full rather than hoping customers run late with payments and pay extra charges, so a lot of the benefit would depend on their revenue source. A possible hidden effect from the low precison score for high risk could be that customers will choose competitors that offer them better interest rates because they are actually low risk loans. The high accuracy score makes us think that this effect will not be that large, but again it depends on what the main sources of revenue are for the credit card company. Our reccommendation would be that although this model is relatively accurate and sensitive, it can be used as long as the questions that come from the low precision score for high risk loans are answered.
