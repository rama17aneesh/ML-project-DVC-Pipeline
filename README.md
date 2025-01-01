# ML-project-DVC-Pipeline

** DVC is just like GIT. In GIT we will track our code, but in DVC we will track changes made to our data.
** In order to start versioing our data, we need to be in a git respository. the reason is because DVC also uses GIT in order to  version the information about our data.
** DVC stores information about files, their hashes and their locations. we need to store the data somewhere. DVC does not store images, DVC only keeps track of the imges, whenever new images are added DVC has the information about this Images.
** It is Data versioning, which keeps information about the changes in our dataset.
# Most ML projects consist of multiple stages
(i) Data pre-processing
(ii) Feature Extraction
(iii) Training
(iv) Evaluation
** DVC pipeline make it easy to run stages of an ML pipeline.
** DVC automatically determines which parts of a project need to be run. IT USES Directed Acylic Graph(DAG).
** In the graph, we have nodes from "train data" to "train and evaluate the data". Each node has its own dependencies. For example:- to process data we need raw data and toprepare feature extraction we neeed to have a dependency from process data.
** Using DVC, you can create these nodes and also specify input and output dependencies as well as parameter dependencies of our pipeline.
** So, what Dvc does is it automatically determines which parts of a project needs to be run and its caches runs and the result to avoid unneccessary re-runs.
