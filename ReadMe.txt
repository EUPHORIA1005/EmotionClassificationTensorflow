PAFEW dataset

------------------------

This experiment is designed by Prof Tom Gedeon (Tom.gedegon@anu.edu.au), developed by Mr Zi Jin(zi.jin@anu.edu.au) and conducted by Ms Jessica Rahman (jessica.rahman@anu.edu.au), Ms Yang Liu (yang.liu3n@anu.edu.au) and Mr Shouxu Lin(u5898871@anu.edu.au). 

In this experiment, we displayed a series of clips to the participants, some physiological signals were monitored and collected by E4 watches and Eyetribes. 
In total, 773 movie clips from the training set of AFEW and 383 movie clips from the validation set of AFEW with 7 categories of emotions are used in this experiment. 

Each subject viewed around 80-90 video clips mixed up with all 7 categories. To keep them focused, they need to answer ‘How does this expression presented in the video look to you?’ (1 is completely fake, 5 is completely real), “Have you seen this video before” and  “How do you rate your confidence level” (1 is week while 5 is strong) after each video. There are 57 subjects participated in the experiment.
	
------------------------

The 'train' folder contains the EDA data corresponding to the movie clips from the training set of AFEW.
The 'val' folder contains the EDA data corresponding to the movie clips from the validation set of AFEW.

In each person's folder, there are two files, 'EDA.csv' and 'log.txt'.

'EDA.csv' is the EDA data of this person. The first line is the start time and the second line is the sample rate. For example, our E4 wristband works at a sample rate of 4Hz.

'log.txt' contains the information below:
1) The first line contains a subject’s Name, Age, Gender, Ethnicity and Primary Language;
2) The second line contains the fields of the following data;
3) From the third line, each line contains the Video index, Video start time, Video name and Video end time for each video. 
   For example, in '1;1583391351.7529519;Happy010232120.mp4;1583391379.1217537', '1' is the index of this video, '1583391351.7529519' and '1583391379.1217537' are the start time and end time of watching the video and answering the first question ‘How does this expression presented in the video look to you?’. 'Happy010232120.mp4' is the video name and the 'Happy' is the emotion label of this video. For the videos from the training set of AFEW, the names do not contain '_', like 'Happy010232120.mp4'. However, for those from the validation set of AFEW, the names contain '_' like 'Sad_011823760.mp4'. 

The 'preprocess_data.py' file shows an example of preprocessing this dataset. You can use your features and filters to substitute those in this file.

Since our dataset has been expanded, the result of the baseline might be different from the result shown in the baseline paper.

------------------------

If you have any questions about this dataset or experiment, please contact Yang Liu (yang.liu3@anu.edu.au)
