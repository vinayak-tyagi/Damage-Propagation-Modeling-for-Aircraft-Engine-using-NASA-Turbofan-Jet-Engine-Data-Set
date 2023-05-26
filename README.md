# Damage Propagation Modeling for Aircraft Engine using NASA Turbofan Jet Engine Data Set

[Colab link](https://colab.research.google.com/drive/12FUmEwymqgzdM2jeV-AnM5zD6M4fTl8L?usp=sharing)

[Kaggle link](https://www.kaggle.com/code/vinayak123tyagi/damage-propagation-modeling-for-aircraft-engine)

[NASA Turbofan Jet Engine Data Set](https://www.kaggle.com/datasets/behrad3d/nasa-cmaps)

## About Dataset

### ***Description***

Prognostics and health management is an important topic in industry for predicting state of assets to avoid downtime and failures. This data set is the Kaggle version of the very well known public data set for asset degradation modeling from NASA. It includes Run-to-Failure simulated data from turbo fan jet engines.

Engine degradation simulation was carried out using C-MAPSS. Four different were sets simulated under different combinations of operational conditions and fault modes. Records several sensor channels to characterize fault evolution. The data set was provided by the Prognostics CoE at NASA Ames.
Prediction Goal

In this dataset the goal is to predict the remaining useful life (RUL) of each engine in the test dataset. RUL is equivalent of number of flights remained for the engine after the last datapoint in the test dataset.

### ***Experimental Scenario***

Data sets consists of multiple multivariate time series. Each data set is further divided into training and test subsets. Each time series is from a different engine i.e., the data can be considered to be from a fleet of engines of the same type. Each engine starts with different degrees of initial wear and manufacturing variation which is unknown to the user. This wear and variation is considered normal, i.e., it is not considered a fault condition. There are three operational settings that have a substantial effect on engine performance. These settings are also included in the data. The data is contaminated with sensor noise.

The engine is operating normally at the start of each time series, and develops a fault at some point during the series. In the training set, the fault grows in magnitude until system failure. In the test set, the time series ends some time prior to system failure. The objective of the competition is to predict the number of remaining operational cycles before failure in the test set, i.e., the number of operational cycles after the last cycle that the engine will continue to operate. Also provided a vector of true Remaining Useful Life (RUL) values for the test data.

The data are provided as a zip-compressed text file with 26 columns of numbers, separated by spaces. Each row is a snapshot of data taken during a single operational cycle, each column is a different variable. The columns correspond to:

1) unit number
2) time, in cycles
3) operational setting 1
4) operational setting 2
5) operational setting 3
6) sensor measurement 1
7) sensor measurement 2 <br>
....
26) sensor measurement 26

### ***Data Set Organization***

- Data Set: FD001 <br>
Train trjectories: 100 <br>
Test trajectories: 100 <br>
Conditions: ONE (Sea Level) <br>
Fault Modes: ONE (HPC Degradation) <br>

- Data Set: FD002 <br>
Train trjectories: 260 <br>
Test trajectories: 259 <br>
Conditions: SIX <br>
Fault Modes: ONE (HPC Degradation) <br>

- Data Set: FD003 <br>
Train trjectories: 100 <br>
Test trajectories: 100 <br>
Conditions: ONE (Sea Level) <br>
Fault Modes: TWO (HPC Degradation, Fan Degradation) <br>

- Data Set: FD004 <br>
Train trjectories: 248 <br>
Test trajectories: 249 <br>
Conditions: SIX <br>
Fault Modes: TWO (HPC Degradation, Fan Degradation) <br>

### ***Reference***

Reference: A. Saxena, K. Goebel, D. Simon, and N. Eklund, Damage Propagation Modeling for Aircraft Engine Run-to-Failure Simulation, in the Proceedings of the 1st International Conference on Prognostics and Health Management (PHM08), Denver CO, Oct 2008.

Alternatively the dataset can be downloaded from https://ti.arc.nasa.gov/tech/dash/groups/pcoe/prognostic-data-repository/
