# javaMachineLearning

This project aims to be an easy and reusable way to use supervised machine learning techniques.

To generate a knowledge model it is required to choose your machine learning technique then you'll have to have an .arff file and specify its path in the constructor method just as the index of the predictive class.

```
ClassifierInterface hepatitisClassifier = new ClassifierInterface(ClassifierInterface.Type.NAIVEBAYES, "HepatitisDataSet", 0);
```

Then if you want to classify a new register to obtain a prediction of its class you'll use the classifier method, its parameter is a List of Objects which has to contain the features of your new register

```
String hepatiteClass = hepatitisClassifier.classifier(Arrays.asList(40,"1","1","2","1","2","2","2","1","2","2","2","2",0.60f,62,166,4.0f,63,"1"));
```

## information about the data

* [More dataSets like this](http://archive.ics.uci.edu/ml/datasets.html) - The Data of HepatitisDataSet bay be found here
* [Used dataSet](http://archive.ics.uci.edu/ml/datasets/Hepatitis) - More information specifically about the used dataSet
* [data](http://archive.ics.uci.edu/ml/machine-learning-databases/hepatitis/hepatitis.data) - The data itself may be found here
* the data of "plantas" dataset was collected from my backyard garden :)
