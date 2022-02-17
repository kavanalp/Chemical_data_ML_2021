# mlclass_proj_f2021

Repository of TBA group project for Applied Machine Learning course. </br>

Fatemeh Saberi Khomami

Arash Sadeghi Bablan

Kavan Alipanahi

Parham Mohammad Panahi


Dataset: https://github.com/hhaji/Applied-Machine-Learning/tree/master/Projects/Projects-Fall-2021/Data

QM9 data after preprocessing as .npy and csv (compressed and otherwise) (there are both 32 and 64 bit version of data): https://drive.google.com/drive/folders/1KaFlD8dsaVFWoLW7p4-TLDlwFa2PUWKN?usp=sharing

Tox21 feutures after preprocessing as csv: https://drive.google.com/file/d/1-2M05lQiuzdUjScfVr4Jtc9YDcRQYCGu/view?usp=sharing </br>
Tox21 label(NR-AR task) after preprocessing as csv: https://drive.google.com/file/d/1-3KaYohG9Dosxjfung76xSjrvNDN2CXk/view?usp=sharing



## TOXCAST
#### Prerocessing Steps
1. picked one task based on lowest label Null value and highest class balance
2. Dropped rows with Null values
3. Dropped Constant Columns
4. Renamed columns to non-negative integers
5. Dropped columns highly correlated with other columns (80%)

#### Selected Task
1. TOX21_TR_LUC_GH3_Antagonist


## Tox21
#### Prerocessing Steps
  1. Renamed features to natural numbers
  2. Dropped Constant Columns
  3. Picked the task with the lowest NA rate (Task : NA-NR)
  4. Filled some of the NA values of the chosen task by a similar Task named "NR-AR-LBD" (Also Correlation Matrix showed that this task was the most relevant to NA-NR)
  5. 
  6. Dropped rest of the NA rows because it was a negligible portion of data 
 
#### Selected Task
1. NR-AR


## QM9
#### Prerocessing Steps
  1. There was no row with Null value
  2. Dropped Constant Columns
  3. There was no label with Null value
 
#### Selected Task
1. GAP (for single task models)
2. all tasks (for multitask models)
