# predective-maintenance-analysis
this project predict the failure of machine with sensors reading using machine learning 

## overview
Predictive maintenance techniques are designed to help anticipate equipment failures to allow for advance scheduling of corrective maintenance, thereby preventing unexpected equipment downtime, improving service quality for customers, and also reducing the additional cost caused by over-maintenance in preventative maintenance policies. Many types of equipment—e.g., automated teller machines (ATMs), information technology equipment, medical devices, etc.—track run-time status by generating system messages, error events, and log files, which can be used to predict impending failures.

### goal
The dataset is in kind of time series, consisting of log message and failure record of 984 days.
The problem is to predict which day is a failure day in advance (e.g. 1-day in advance prediction) based on the features (constructed from log file of error messages before the predicted day).


### Data
Feature: the log data of the target machine.
There are MANY different error types when machine running.
Each types of error has a number id (for example: 136088194).
The feature file is a collection of basic statistics of each error.
count: how many times the error occurs in that day.
min: tick of the first time the error occurs in that day (seconds).
for example, min = 3600 means this error first occurs at 01:00 (3600 seconds in day).
max: tick of the last time the error occurs in that day.
mean: mean of tick the error occurs.
std: standard deviation of tick the error occurs.
Label: failure record of the target machine.
0: the machine is OK in that day.
1: machine break down for some reasons in that day.



