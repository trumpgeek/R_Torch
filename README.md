This is more of a notes to self, to make me recall what I did to execute a simple DL exercise using torch and luz R packages.

The inspiration for this is from the video of Dr Bharatendra Rai using R and Keras. I am doing the same but using torch+luz. Here we use a Cardio dataset which I think originally comes from here. I am not familiar with the features and we are just going to use the last column (NSP) to predict but the other columns before that, as predictors. Here is an example of the data and note that NSP is actually a category data though it is numericcally represented by 1, 2, 3 as we see here.
<img width="1226" height="116" alt="image" src="https://github.com/user-attachments/assets/4f0bacb6-fa99-4f5c-a6ef-e692290c9071" />

Here is the distribution of the NSP variable
<img width="988" height="543" alt="image" src="https://github.com/user-attachments/assets/ead4446e-4e78-48d7-8451-83ae07370032" />
Here is how we see the loss function decreasing as we go through the epochs. Looks like it can be further improved by increasing it more than 40.
<img width="988" height="544" alt="image" src="https://github.com/user-attachments/assets/a0d2e971-f007-4c67-91ad-0cee5ed29644" />
The confusion matrix we get. Not bad, about 87% accuracy. It can be improved by increasing the epoch size etc.
<img width="266" height="84" alt="image" src="https://github.com/user-attachments/assets/344f2979-a3e9-4c8e-9afb-9135189650ad" />

There it is. It complies with the data distribution of NSP, a good validation sanity check.
