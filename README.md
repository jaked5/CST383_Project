# CST383_Project
By: Jake Horne, Hamdan Syed, Justin Nguyen

## Predicting Medical Student Mental Health

The purpose of this project is to ustilize a real world dataset, and compose a question based off of related varaibles. From this question, we hope to create a machine learning model to assist in accurately predicting a predetermined result with accuracy.

## Dataset Variables and Explanation

This specific dataset looks at the mental health of medical students in Switzerland, and looks at the mental health of these students at the time of this study. We want to create a machine learning model that looks at the well being of a student, and determines the relationship of key characteristics (of our choosing) to determine the emotional state of these individuals. From there, we want to discen if their are charactersitics that telegraph whether an individual is more susceptible to declining mental health or burnout, and to find these signs early to provide assistance for these students to minimize the adverse effects. The following attributes are used to determine the mental well being of these medical students:

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



By utilizing patterns with these characteristics, we hope to more accurately determine whether a particular individual is going through emotional decline or burnout, since the sooner these results are determined, less invasive procedures can be performed and students can minimize the negative consequences of mental stress.

&nbsp
Main characteristics we want to look further into are as follows:

1. <b>year</b> - different years have different workloads and stress
2. <b>stud_h</b> - health of students
3. <b>job</b> - balancing work and education, stress of limited time
4. <b>amsp</b> - less motivation could lead to more anxiety of falling behind
5. <b>health</b> - student is in an atmosphere of mental stress constantly
6. <b>psyt</b> - tangible level of stress
  

