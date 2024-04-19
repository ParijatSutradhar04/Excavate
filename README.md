# Excavate
Prediction of the diameter of metallic glass

### Scenario
Predicting how well a metallic alloy will form a glass can be a slow, trial-and-error process. AI
and data science are changing that. By analysing datasets of existing metallic glasses,
machine learning models can predict the glass-forming ability of new alloys, reducing the
need for extensive experimentation. This not only saves time and resources, but can also
lead to the discovery of entirely new glass compositions with superior properties.

### Problem
Design and implement a machine learning model to predict the glass forming ability (GFA) of
metallic glass, expressed as Dmax (in mm), the target variable. It is theorised that GFA
depends on several intrinsic parameters like total electronegativity (TEN), atomic size
difference (d), average atomic volume (VA), mixing entropy (Sm), glass-transition
temperature (Tg), onset crystallisation-temperature (Tx), and liquidus temperature (Tl).
Develop an robust and accurate predictive model that can predict the Dmax of a metallic
glass sample, given the input features

### Approach
In order to address the issue of a small dataset and having only a single input for some
Dmax values, we have employed various data augmentation methodologies, so as to have
sufficient data to train our model and to accurately give the required result. Further, we
employ Exploratory Data Analysis(EDA) to obtain an understanding of the data, and
Principal Component Analysis(PCA), to plot the data into graphs, to realise the potential of
the dataset. A comprehensive approach was adopted, after trying multiple regression
models, the XGBoost model was used to implement regression on the data, and obtain a
precise estimation. The mean squared error(MSE) has been used as a yardstick to
determine the effectiveness of different models. We have implemented regression through
six models, determining training and testing MSEs for each one of them. Using this selection
criteria, we have arrived at the conclusion that XGBoost is the best model among them all.
