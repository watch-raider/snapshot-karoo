# Dataset - Snapshot Karoo
The Karoo National Park is a wildlife reserve in the Great Karoo area of the Western Cape, South Africa near Beaufort West. This semi-desert area covers an area of 750 square kilometres.

The Karoo National Park is a sanctuary for herds of springbok, gemsbok (or Oryx),black wildebeest Cape mountain zebra, red hartebeest, black rhinoceros, eland, kudu, klipspringer, bat-eared foxes, black-backed jackal, ostriches, and, since fairly recently, lions.

This data set contains 14889 sequences of camera trap images, totaling 38074 images, from the Snapshot Karoo project, part of the Snapshot Safari network.

Labels are provided for 38 categories, primarily at the species level (for example, the most common labels are gemsbokoryx, hartebeestred, and kudu). Approximately 83.02% of images are labeled as empty.

Link to dataset [Snapshot Karoo dataset](https://lila.science/datasets/snapshot-karoo).

# Motivation
We are now in the middle of what conservation biologists are calling the sixth mass extinction. This refers to the fact that many species of organisms are now going extinct at the fastest rate since the dinosaurs disappeared.

The problem of biodiversity loss is already in an alarming state and only getting worse year after year due to human activities and climate change itself. Their protection and restoration of biodiversity will be accomplished through policies enacted by governments that can lead to significant shifts in industry practices and cultural norms. In order to move towards these future policies, it's critical that we take steps now to monitor biodiversity across a wide range of ecosystems and to quantify the current impacts of human activities and climate change and identify opportunities to move the needle in the opposite direction.
Project This project will involve feeding images from the Karoo dataset into a CNN model in order to effectively classify animals pictured in images from the Camera Traps located in the Karoo national park. This will help researchers assess the biodiversity in the Karoo national park and track it over time. If successful, this model can then be used to assess biodiversity of other national parks around the world.

# Major Tasks
### Data Selection, Loading
The dataset contains images totaling 42GB which is too large to manage. The dataset has provided ways of only downloading only certian folders. The folders correspond to which Camera Trap the image was taken by. Therefore, a team member is needed to select how much and which parts of the dataset should be used for the project.
Next task is to load the dataset using Python, including the images and the annotations, so that it can be passed into the model. 
Images are available via Azure Blob Storage or Google Cloud Storage
### Visualisation
Some visualisation will then need to be performed in order to understand the dataset that has been selected.
This may include visualising how many images there are of each species and what kind of imagery each Camera Trap has taken.
### Data Cleaning
After understanding the dataset better, some data cleaning will be required in order to balance it better. 
For example, most of the images from these camera traps are empty so elimination of some empty images might be required in order to have a more balanced dataset.
Outliers might also have to be removed such as certain species who have very few images available.
### Build, Train, and Test SVM Classifier Model
Next step is to build SVM model to perform the Classification task
### Analyse and Visualise Results
Final step is to assess the accuracy of the model and visualise its performance. 

# Results

The model acheived an accuracy of 76%, which is a decent performance for an SVM model on a challenging image dataset such as this one. A lot of the species look very similar and are difficult even for a human
to classify. Therefore, an improvement on this project would be to use a CNN model instead which can handle more features. I encourage you to checkout the SnapshotKaroo.ipynb notebook to view the code and more detailed results.

