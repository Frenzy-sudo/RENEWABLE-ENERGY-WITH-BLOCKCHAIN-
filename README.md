# RENEWABLE-ENERGY-WITH-BLOCKCHAIN-
Secure Renewable Energy Microgrid  in a 6G-powered microgrid using blockchain technology

## Project Objective
To study and analyze how renewable energy (solar, wind) can be integrated securely into a microgrid system powered by 6G communication, using blockchain technology to ensure data integrity, transparency, and secure energy transactions.

##  Goal
*  Analyze blockchain transaction data for secure energy trading patterns.
*  Provide insights for designing resilient, secure, and efficient microgrid systems leveraging 6G and blockchain.

## Tools & Technologies Used
**Programming Language**: Python 3.11.5

**IDE**: Anaconda / VS Code

**Libraries**:
*  Pandas
*  NumPy
*  Matplotlib
*  Seaborn
*  Scikit-learn

## Context
The dataset includes hourly data capturing multiple dimensions of a smart microgrid over one month:
-  Energy generation and consumption metrics
-  IoT sensor data (smart meters)
-  Blockchain transaction records related to energy trading
-  Cybersecurity event logs detecting potential attacks
-  Network slicing performance metrics (latency, packet loss)

##   Key Project Areas
-  Renewable Energy Forecasting & Optimization
Using solar/wind generation and storage data to optimize energy distribution and reduce reliance on the grid.
-  IoT Sensor Data Analytics
Monitoring voltage, current, power factor to detect anomalies or failures in energy delivery.
-  Blockchain-based Secure Energy Trading
Analyzing P2P transactions to ensure transparency and reduce fraud or tampering in decentralized energy markets.
-  Cybersecurity in Microgrids
Detecting cyberattacks using logs of blockchain integrity checks and cybersecurity events.
-  Network Performance for Energy Systems
Studying network slicing data to maintain reliable, low-latency communication essential for real-time microgrid management.
-  Anomaly Detection & Machine Learning
Using the target column "Anomaly_Detected" to build models that detect abnormal energy or security events in the microgrid.

 ## Project Flow 

| Step | Action                                                    |
| ---- | ------------------------------------------------------    |
| 1    | Displays basic info                                       |
| 2    | Removes columns with too many missing values              |
| 3    | Removes rows with missing values                          |
| 4    | Droping  duplicates                                       |
| 5    | Strips whitespace from column names                       |
| 6    | Converting data types (like datetime)                     |
| 7    | Removes unwanted columns                                  |
| 8    | Filters rows based on rules (e.g. non-negative values)    |
| 9    | Resets the index for a clean DataFrame                    |
| 10   | Compute correlation matrix and plotting  heatmap          |
| 9    | Creating box plot for comparison                          |

###  Challenges Faced
Graph Plotting ; It Only Displayed 2 Graphs due to them meeting the dataset plotting conditions ,Meaning other graphs did not.

### Insights from the Box Plot

* Large outliers in **Solar_Radiation_Wm2, Battery_Storage_kWh, and Grid_Supply_kWh.** ,These might indicate unusual spikes in solar input or backup energy usage.

* **Battery_Storage_kWh** has high variation suggests fluctuating storage behavior.

* Variables like **Power_Factor, Blockchain_Verified, and Anomaly_Detected** are close to binary or small-scale,having low range features.

### Insights from the Correlation Heatmap
*  Most variables have low(weak) correlations (< 0.3) , suggesting many independent systems in operation.

*  There's Strong Positive Correlation **Between Battery_Storage_kWh and Grid_Supply_kWh**  possibly related to load balancing.

*  **Energy_Demand_kWh** has weak correlation with generation values this could imply reliance on grid backup.

* Target Correlation **Anomaly_Detected** has a 0.30 correlation with Cyberattack Detected thus suggesting  that cyberattacks are often involved in anomalies.
