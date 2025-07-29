# EEG_procesing
In this work we trained an AI to recognize artifacts in electroencephalograms (EEG) and search for synchronization in the brain through the Kuramoto model.

An electroencephalograms (EEG) is a measurement of the level of brain activity and consists of 24 diodes around the head, where each one measures the electrical activity in this region and the difference between 2 diodes is called a "channel" wich also is a time serie. The problem is that during the EEG there are some "errors" in the measurement due to involuntary movements of the patient, such as flickers, eye movements, masseter muscle movement, etc. This errors are called "artifacts" and it's necessary an experienced doctor to detect an artefact in a EEG, because of that we decided to develop an AI that can detect it automatically.

So, for this work we achieved to get a very large database containing hundreds of EEG of more than 1400 seconds of measurement, with his artifacts marked by a qualified doctor, then the first step was to match, normalize and clean the data and then we chose a Long Short Term Memory (LSTM) as our neuronal network and used Optuna to optimize our hyperparameters and make the neuronal network's training, getting the next performance:


Additionaly, we use the Kuramoto model to made a short analysis looking for synchronization between channels to track impulses along the brain during a artefact but we didn´t find anything relevant.
