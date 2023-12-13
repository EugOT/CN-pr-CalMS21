# CN-pr-CalMS21

**Group Project: CalTech Social Mice Behavior Dataset (Neuroscience Seminar WS 2023, Vienna)**

For a quick overview of the project, check out our presentation [https://github.com/EugOT/CN-pr-CalMS21/blob/main/Mouse_behavior_presentation.pdf].

**Keywords:** social mouse behavior, pose tracking through body parts, annotation-bottleneck-problem, classification problem, prediction through machine learning, logistic regression, random forest, hist gradient boosting, PCA visualization, mean distance measure, SHAP method.

### The Problem: Social Mice Behavior & the Annotation Bottleneck Problem [https://github.com/EugOT/CN-pr-CalMS21/blob/master/SocMice_litSummaries.docx], [https://github.com/EugOT/CN-pr-CalMS21/blob/main/Mouse_behavior_presentation.pdf].

The overarching question is how the brain creates behavior. To exlore this question Scientists are exploring behavioral units(syllables) in mice to identify grammatical patterns using pose tracking divided into body parts. The goal is to make behavioral observations independent of human intuition while leveraging machine learning. However, the need for labels, especially accurate ones, creates the annotation bottleneck problem. Annotation is slow, time-consuming, and introduces variability in interpretation. A method to resolve this dilemma is crucial.

**Our Working Question:** Is machine learning prediction a useful method? And if so, which? If machine learning tools accurately predict labels, they become invaluable in solving the bottleneck problem, making annotation faster and more consistent.

### The Data: CalTech Dataset

We've adapted a notebook from the CalTech dataset, originally comprising 6 million frames of unlabeled tracked poses and 1 million frames with labeled poses. The labels used are "attack," "investigation," "mount," and "other," with variables such as nose, left_ear, right_ear, neck, left_hip, right_hip, and tail_base. Our dataset includes 70 sequences for training and 19 sequences for testing. A distribution check revealed a classification problem, with "attack" being a minority class.

### The Method: Prediction

1. **Prediction:** Is there a correlation between body parts and behavior? [https://github.com/EugOT/CN-pr-CalMS21/blob/main/Proj_Supervised_Learning.ipynb]
2. **Prediction:** Can ML Classification assist in annotating frames? [https://github.com/EugOT/CN-pr-CalMS21/blob/main/Proj_Supervised_Learning.ipynb]
3. **Prediction:** How do distances play into behavior? Can distances be used for prediction? [https://github.com/EugOT/CN-pr-CalMS21/blob/main/distanceBasedClassification.ipynb]
4. **Prediction:** How well does the prediction work for each behavioral label? [https://github.com/EugOT/CN-pr-CalMS21/blob/main/distanceBasedClassification.ipynb]
0. **Prediction:** Dive into the data with SHAP feature contributions to understand influencing factors and crucial features in the decision-making process of the decision tree model. [https://github.com/EugOT/CN-pr-CalMS21/blob/main/SHAP.ipynb]

### Bottom Line

For detailed findings, see the presentation [https://github.com/EugOT/CN-pr-CalMS21/blob/main/Mouse_behavior_presentation.pdf].

Several machine learning tools showed a correlation between body part and behavior. Machine learning can assist in annotating frames. Distances seemed to be a useful measure to predict a certain behavior. Nevertheless, one has to note that prediction works better for some labels than for others.

Consideration for future work: The project can be continued by using sequences with the meta-prediction algorithm.

