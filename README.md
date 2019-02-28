# CarND-T3-Prediction-NaiveBayes
Udacity CarND Term3 3. Prediction exercise implementing naive Bayes. 

# Status report:
```
 X_train number of elements 750
 X_train element size 4
 Y_train number of elements 750
 X_test number of elements 250
 X_test element size 4
 Y_test number of elements 250
 **You got 84.80000 correct**
```

# Features extracted:
- Feature 1: even occuring probability:
```

```
- Feature 2: offset from road center. Notice keep deviation is really small besides its small offset.
```

```
- Feature 3: d_dot be negative/left, almost zero/keep, positive/right.
```

```

# Theory
- Prediction can be done using Gaussian Naive Bayes method.
* Wikipedia has a very good example of sex classification here:
   https://en.wikipedia.org/wiki/Naive_Bayes_classifier#Gaussian_naive_Bayes
* The theoretcal explanation is also good:
   https://en.wikipedia.org/wiki/Naive_Bayes_classifier#Parameter_estimation_and_event_models

- Use Gaussian distribution to emulate the probability. Need to get u and sigma of each feature.
```
    //      u = average over all same labelled data
    //      sigma^2 = sum((x_i - u)^2)/N
```