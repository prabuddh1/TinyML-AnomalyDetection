# TinyML (Tiny Machine Learning) Anomaly Detection Application

Using Autoencoders for Anomaly Detection, the model detects detect anomalies on the [ECG5000 dataset](http://www.timeseriesclassification.com/description.php?Dataset=ECG5000) of the ECGs. Around 10% of training set is anomalies, the labels are not available at training time. This is to reflect a truely unsupervised scenario.

### Training & Inference

> The autoencoder is trained using the combined training data which is primarily normal ECGs with some anomalies mixed in. The model classify an ECG as anomalous if the reconstruction error is greater than one standard deviation from the normal training examples.

> ROC and AUC Metrics:
The Receiver Operating Characteristic (ROC) plots allows us to visualize the tradeoff between predicting anomalies as normal (false positives) and predicting normal data as an anomaly (false negative). Normal rhythms are labeled as `1` in this dataset but we have to flip them here to match the ROC curves expectations.
The ROC plot now has threshold values plotted on their corrispoinding points on the curve to aid in selecting a threshold for the application.