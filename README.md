# CST383_Project
By: Jake Horne, Hamdan Syed, Justin Nguyen

## Predicting Medical Student Mental Health

The purpose of this project is to ustilize a real world dataset, and compose a question based off of related varaibles. From this question, we hope to create a machine learning model to assist in accurately predicting a predetermined result with accuracy.

## Dataset Variables and Explanation

This specific dataset looks at the mental health of medical students in Switzerland, and looks at the mental health of these students at the time of this study. We want to create a machine learning model that looks at the well being of a student, and determines the relationship of key characteristics (of our choosing) to determine the emotional state of these individuals. From there, we want to discen if their are charactersitics that telegraph whether an individual is more susceptible to declining mental health or burnout, and to find these signs early to provide assistance for these students to minimize the adverse effects. The following attributes are used to determine the mental well being of these medical students:
</br>

<i>
  
* age: Age of the participant. (Integer)

* year: Year of study of the participant. (Integer)

* sex: Gender of the participant. (String)

* glang: Language spoken by the participant. (String)

* job: Job of the participant. (String)

* stud_h: Hours of study per week of the participant. (Integer)

* health: Self-reported health status of the participant. (String)

* psyt: Psychological distress score of the participant. (Integer)

* jspe: Job satisfaction score of the participant. (Integer)

* qcae_cog: Cognitive empathy score of the participant. (Integer)

* qcae_aff: Affective empathy score of the participant. (Integer)

* amsp: Academic motivation score of the participant. (Integer)

* erec_mean: Empathy rating score mean of the participant. (Integer)

* cesd: Center for Epidemiologic Studies Depression scale of the participant. (Integer)

* stai_t: State-Trait Anxiety Inventory scale of the participant. (Integer)

* mbi_ex: Maslach Burnout Inventory-Exhaustion scale of the participant. (Integer)

* mbi_cy: Maslach Burnout Inventory - Cynicism Scale of the participant. (Integer)

* mbi_ea: Maslach Burnout Inventory - Professional Efficacy Scale of the participant. (Integer)
</i>

</br>

By utilizing patterns with these characteristics, we hope to more accurately determine whether a particular individual is going through emotional decline or burnout, since the sooner these results are determined, less invasive procedures can be performed and students can minimize the negative consequences of mental stress.
</br>
</br>

Main characteristics we want to look further into are as follows:

1. <b>year</b> - different years have different workloads and stress
2. <b>stud_h</b> - health of students
3. <b>job</b> - balancing work and education, stress of limited time
4. <b>amsp</b> - less motivation could lead to more anxiety of falling behind
5. <b>health</b> - student is in an atmosphere of mental stress constantly
6. <b>psyt</b> - tangible level of stress

The main functions we will be using are rmse (root mean squared error), mse (mean squared error), as well as accStatement (used to determine accuracy of model. Using these, we have a metric to determine if our final model is able to predict accurately the mental well being of students not just in our sample, but in future use cases.

## Preprocessing

For our 886 participants, there were no values that were null of void that could lead to discrepancies within the dataset. As such, no columns had to be deleted or removed to account for this. We use describe to have a quick gloss through of the data and keep in mind that the planned value for prediction, or what our machine learning model is centered around is cesd, or the Center for Epidemiologic Studies Depression scale of the participant measured as an integer. This metric is well researched and defined, so we can cross reference to this standard to determine the well being of an individual with a tangible metric.


## Graphing

Initially, we got a general view of all our variable variables by using scatterplots, to verify any trends that were not blatantly obvious or initially perceived. Overall, there was no insightful information gleened from these so we fined tuned our models further by grouping variables we were interested in and looking at the relationship between them, as well as the strength of this relationship. 

In our barplots, we found that as the years in medical school increased, the general trend of mental health within students decreased. Now, we wanted to compare these findings with the quantitative emotional values, or our cesd values that are provided externally. The higher the cesd value, the more severe the depression of an individual. We wanted to mask these values onto our previous barplot where we looked at the relationship between years and mental well being so a few changes had to be made to ensure there was no drastic overexaggeration of features:

* CESD is from 0-60, but was formatted to be between 0-4 to have a similar appearance to our previous graph
* Count and Year axes were preserved

By adhering to these self imposed construct, we wanted to keep the integrity of the data while being able to determine the relationship between our target variables that we felt related strongly to cesd.

## Training
