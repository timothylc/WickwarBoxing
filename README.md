# Assignment7

### The goal of the project is to analyze the career of Len Wickwar - the boxer who fought the most professional boxing fights in history.

### Original data pulled from here: https://en.wikipedia.org/wiki/Len_Wickwar

### For this project, I utilized the python libraries BeautifulSoup, Pandas, Matplotlib, and Requests. The links to the documentation are listed below:

#### BeautifulSoup: https://beautiful-soup-4.readthedocs.io/en/latest/
#### Pandas: https://pandas.pydata.org/docs/
#### Matplotlib: https://matplotlib.org/stable/index.html
#### Requests: https://requests.readthedocs.io/en/latest/

### My data has a CC-0 and the source data has a CC BY-SA license, so you can copy and modify the data.

### In the final processed data set, I had eight attributes:

#### 1. No. - has a data type of int (integer), the order of fights Len had (1 was his first fight, while 473 is his 473th fight), kept this attribute in because the indices were imported with his most recent fights first.
#### 2. Opponent - has a str (string) data type, it is the name of the opponent that he fought in a boxing match.
#### 3. Type - has a str (string) data type, states how the result of the fight was decided, there was a knockout (KO), total knockout (TKO), if the winner was determined by the amounts accumulated (PTS), if there was a disqualification (DQ), and if a fight quits (RTD)
#### 4: Year - has a int (integer) data type, it is the year that the boxing match occurred in
#### 5: Result_Draw: has a integer data type (boolean represented by binary), 0 means it was not the result, 1 means the result was a draw
#### 6: Result_Loss: has a integer data type (boolean represented by binary), 0 means it was not the result, 1 means the result was a loss
#### 7: Result_NC: has a integer data type (boolean represented by binary), 0 means it was not the result, 1 means the result was a no count
#### 8: Result_Win: has a integer data type (boolean represented by binary), 0 means it was not the result, 1 means the result was a win

#### Result was an categorical attribute that was split into 4 using one-hot encoding to help with one of the graphs

### One potential issue was that the data was taken from Wikipedia, where anyone could edit it; this could yield inaccurate results and insights. Also, I realized after using get_dummies on Result that it was not necessary, so the data has more attributes than it actually needs.