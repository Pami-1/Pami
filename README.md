# Pami: A Two-step Purification Approach for Machine Learning-based Vulnerability Detection
The framework of Pami consists
of four main phases: Data Preprocessing, Slice Purification,
Feature Extraction, and Classification. The input of Pami is
the source code of the target function, and the output is the
vulnerability detection results and its interpretation.<br>
• Data Preprocessing: For the source code of the target
function, we first perform code normalization on it and
then conduct program slicing to generate its slices.<br>
• Slice Purification: For slices, we implement a two-step
filtering method, including hash filtering and anomaly
detection filtering, to filter out the slices within the
function that are irrelevant to the vulnerability.<br>
• Feature Extraction: For target function, we first extract
the feature representations of the its slices and then use
them to construct the features of the function.<br>
• Classification: For the feature vector of the function, we
feed it into a machine learning model for training and
detection and infer its vulnerability type from its feature
vector to interpret the vulnerability detection results.
The training phase of Pami consists of two parts: data
preprocessing and slice purification. The input to the training
part is the vulnerable function, which aims to retain the
vulnerable slices by discarding the slices without vulnerabilities. Its goal is to generate a vulnerability anomaly detection
model and cluster the remaining vulnerable slices to generate
vulnerability patterns. The detection phase of Pami includes
data preprocessing, feature extraction, and classification. For
the target function, Pami detects it with the help of anomaly
detection models and vulnerability patterns generated in the
training phase to generate feature vectors of the function.
