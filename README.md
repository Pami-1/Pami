# Pami: A Two-step Purification Approach for Machine Learning-based Vulnerability Detection
The framework of Pami is shown in Fig. 2 which consists
of four main phases: Data Preprocessing, Slice Purification,
Feature Extraction, and Classification. The input of Pami is
the source code of the target function, and the output is the
vulnerability detection results and its interpretation.<br>
• Data Preprocessing: For the source code of the target
function, we first perform code normalization on it and
then conduct program slicing to generate its slices.
• Slice Purification: For slices, we implement a two-step
filtering method, including hash filtering and anomaly
detection filtering, to filter out the slices within the
function that are irrelevant to the vulnerability.
• Feature Extraction: For target function, we first extract
the feature representations of the its slices and then use
them to construct the features of the function.
• Classification: For the feature vector of the function, we
feed it into a machine learning model for training and
detection and infer its vulnerability type from its feature
vector to interpret the vulnerability detection results.
