# Multitasking-in-Divided-Attention
### Attention
Attention, in psychology is the concentration of awareness on some phenomenon to the exclusion of other stimuli. Attention is best described as the sustained focus of cognitive resources on information while filtering or ignoring extraneous information.
#### Types of Attention
- Focused attention
- Sustained attention
- Selective attention
- Alternating attention
- Divided attention
## Divided Attention
Divided attention could be defined as our brain’s ability to attend to two different stimuli at the same time, and respond to the multiple demands of your surroundings. Divided attention is a type of simultaneous attention that allows us to process different information sources and successfully carry out multiple tasks at a time. When you divide your attention, the efficiency with which you do these actions is decreased, and you will almost certainly perform poorly. Interference is the term used to describe when a person has a hard time attending to two stimuli at a time. We see interference when the brain is only able to process a certain amount of information. However, cognitive training can help improve divided attention, and as a consequence, the ability to do more than one activity at a time.

### Attention Assessment
To measure divided attention,I attempt to formalize a method for analyzing one game which is designed to challenge player's ability to attend to multiple dimensions of stimuli simultaneously. I have created a game consisting of 3 tasks in which a user has to simultaneously response to all 3 tasks in a sequential order. This game runs for around 12 minutes.
In this test, given a randomly generated stimuli which keeps on changing and one to respond for the target stimuli. With help of this GUI, I have collected the data from several people.

In this work we have developed three distinct task which will have spatial identification test, color and number test (1.png), which will monitor the attention level by using visual effect and multi-tasking. 

#### Proposed Algorithm
To classify the divided attention in 3 category namely Low, Average and High divided attention, we have applied the following steps after collecting the data:
- Remove the inconsistent data from dataset.
- Label the data based on the mean and standard deviation of the attention score.
- Apply machine learning model to classify the attention type (Low, Average, High).
- Analyze the output and trends in academic performance and divided attention.

##### Labelling the dataset
- I have done the statistical analysis individually for each of the three cognitive tasks. I am using mean(μ) and standard deviation(σ) in order to differentiate between the three classes(high, average, low).
- Again we will do the statistical analysis but now for the combined cognitive task comprising of all the three tasks. The statistical parameters for this combined task are (μ, σ).
- Then, check for the consistency of the subject's performance in the combined cognitive task with the help of the performance of his individual tasks. By doing so all the inconsistent or irrelevant records(due to fatigue, boredom or habituation) will be filtered out.
- Then, categorize each record of the dataset in three classes of Divided Attention as follows :
1. High Divided Attention (results are above μ + σ)
2. Average Divided Attention (results are between μ
3. Low Divided Attention (result are below μ - σ)
Scatter plot of Task-1, Task-2 and task-3 are shown in Figure 3d.png, in which green bubble represent High attention score, red dot represent Average attention score, whereas blue bubble represent Low attention score.

Target Value Z (in DAttention.csv) is divided into 3 class namely -1, 0, 1 where,
- -1 corresponds to Low Divided Attention.
- 0 corresponds to Average Divided Attention.
- 1 corresponds to High Divided Attention.

### Classification of Divided Attention
I have applied Naive Bayes classifier, Support Vector Machine (SVM) and Random Forest Classifier to classify the dataset.
Also, studied the trends  in academic performance(trends.png). This analysis examines the association between student's divided attention performance and their academic functioning which tells whether a subject having high, low or average divided attention performs well or poorly in his academics.
