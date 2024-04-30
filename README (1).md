# Big-Data-Security-and-Privacy-in-NYC-Taxi-Trip-Data
This project explores security and privacy issues in big data and cloud computing, focusing on the New York City Taxi Trip dataset from 2013. Through RSA encryption/decryption and anomaly detection, we demonstrate critical techniques for maintaining data integrity and confidentiality.

About the Dataset
The dataset comprises NYC Taxi trip records from 2013, released under The Freedom of Information Law and made public by Chris Whong. It includes detailed trip information such as pickup and dropoff times, locations, distances, fares, and payment types.

Size: 93 MB compressed, 384 MB uncompressed
Source: Chris Whong's Data Repository
Setting Up the Environment
Prerequisites
Python 3.x
Pandas
Numpy
Scikit-learn

Installation
Install the required Python packages using pip:
pip install pandas numpy scikit-learn

Importing Libraries
import pandas as pd
import numpy as np

Usage
Loading the Data
file_path = "/path/to/taxi-data-sorted-small.csv"
df = pd.read_csv(file_path)

RSA Encryption/Decryption
Generate RSA Key Pair: Create a private and a public key for encryption and decryption.
Encrypt Data: Use the public key to encrypt sensitive columns in the DataFrame.
Decrypt Data: Use the private key to decrypt the encrypted values.

Anomaly Detection with Isolation Forest
Feature Selection: Choose fare_amount and trip_distance for anomaly detection.
Model Training: Train an Isolation Forest model on the selected features.
Detect Anomalies: Identify records that significantly deviate from typical patterns.

Results
RSA Encryption/Decryption: Demonstrated how to securely encrypt and decrypt sensitive information in the dataset.
Anomaly Detection: Detected 19,911 anomalies out of 1,999,998 records, highlighting unusual taxi trips based on fare and distance.

Conclusion
This project showcases practical approaches to addressing privacy and security challenges in big data through encryption techniques and anomaly detection. By applying these methods to the NYC Taxi Trip dataset, we emphasize the importance of data security and privacy preservation in the era of big data and cloud computing.

