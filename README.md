#LIBSVM Example

In this example we guide readers how to use LIBSVM a popular library for the support vector machine classifier.

The file output_tr contains features set for real sensors in a water treatment plant. 

Specific details on which type of sensor those are and which brand those are kept hidden to safeguard the intellectual property.

However following are important things to note:

* Each sensor has  8 features
* Sensor which we want to identify, is label as 1 and rest of all as 0
* we can run cross validation to see the sensor detection accuracy: "svm-train -v 5 output_tr"
* -v 5 means 5 fold cross-validation. It means whole data is divided into 5 sections and each section is validated with other 4 and this is repeated for all the sections and average accuracy is reported
* Exercise: change cross validation "-v k" for different k to see the effects.