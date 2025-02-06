# Dataset Download Instructions

This repository requires the dataset hosted on Zenodo to function properly.

This dataset was developed for and used in the paper titled "Fault Detection for Agents in Power Grid Topology Optimization: A Comprehensive Analysis" by Malte Lehna, Mohamed Hassouna, Dmitry Degtyar, Sven Tomforde, and Christoph Scholz, presented at the Workshop on Machine Learning for Sustainable Power Systems (ML4SPS), part of ECML PKDD 2024. While the paper is pending formal publication, a preprint version is available on arXiv.

The dataset contains structured training, validation, and test data comprising failure and survival events observed in transmission power grid simulations. These were generated using Grid2Op with the WCCI 2022 L2RPN environment. Each data instance is labeled with one of four classes, representing survival or impending failure in 1, 3, and 5 timesteps. This dataset was used to train, validate and test machine learning models that predict grid agent failures in topology optimization tasks. 

 Follow the steps below to download and organize the data correctly.

## 1. Download the Dataset

The dataset is available at the following Zenodo link:

https://zenodo.org/records/13948340

Download all required files from the "Files" section on the Zenodo page.

## 2. Organize the Data

After downloading, create a folder named data in the root directory of this repository and move the downloaded files into it.

mkdir -p data
mv /path/to/downloaded/files/* data/

Ensure that the structure looks like this:

repository_root/

├── data/
│   ├──  full_obs_data_train.npz
│   ├──  full_obs_data_val.npz
│   ├──  full_obs_data_test.npz
├── *.py
├── README.md

## 3. Verify the Setup

Before running any scripts, verify that the data exists in the correct location by listing the files:

ls data/

If the files are correctly placed, you can proceed with running the scripts in the repository.