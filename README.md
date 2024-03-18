# PAWSOME CONCIERGE - CAREGIVER SELECTION
## Project Summary

Pawsome Concierge, a Montreal-based startup, specializes in personalized pet care services, including boarding, sitting, dog walking, and Pet First Aid & CPR classes. Currently, the caregiver selection process involves a manual assessment through a Google Forms questionnaire prior interviewing the candidate. Pawsome aims to enhance this process by incorporating AI to predict caregiver suitability based on questionnaire responses and additional features.

## Research questions

<ul>
  <li>Can we predict the suitability of candidates for hire Using a data classification model?</li>
  <li>Can we unveil latent patterns within the dataset, grouping individuals based on similarities in their responses?</li>
</ul>

## Dataset and its Main Characteristics

The dataset for Pawsome Concierge, is limited, comprising around 100 caregiver candidates. Acknowledging this constraint, we are actively augmenting the dataset to enrich its diversity.  The dataset encapsulates both personal details, including names, contact information, and addresses, and in-depth questionnaire responses that probe into candidates' reactions to diverse pet-related scenarios. The questionnaire, consisting of 10 multiple-choice scenarios, addresses crucial aspects of caregiving, encompassing “how would you react”-like questions, experience with pets, behavioral issues, health emergencies, and situational management. This questionnaire asks the potential caregiver about experience with pets and “how would you react”-like questions.

Each caregiver is subsequently categorized into one of three classes: "Candidate fails to pass," "Human Revision is Required," or "Candidate Pass." 

- **Province**: Categorical Binary
- **Birth date**: Date/Time
- **How did you hear about PAWSOME Concierge?**: Categorical Ordinal (Website, Colleague or Friend, Search)
- **Which companion animals are you interested in working with?**: Categorical Ordinal (Dogs, Cats, Both)
- **How would you describe your level of experience with Dogs?**: Categorical Ordinal (Beginner, Intermediate, Expert)
- **How would you describe your level of experience with Cats?**: Categorical Ordinal (Beginner, Intermediate, Expert)
- **Services you would like to offer?**: Categorical Nominal (Boarding, Sitting, Walking)

**MCQs:** 
- **Answer1-10**: Categorical Nominal (A, B, C, D)

## Algorithm to be used

We propose a multifaceted approach, utilizing Support Vector Machines (SVM) and K-Nearest Neighbors (KNN) for classification tasks, and CARMA (Clustering and Association Rule Mining Algorithm) for clustering. 

Recognizing the strengths of each algorithm, SVM excels in discerning complex relationships within the dataset, providing robust discrimination between caregiver suitability classes.
 
In contrast, KNN, with its simplicity and adaptability, considers the immediate neighbors of candidates, contributing valuable insights. 
CARMA performs association rule mining, extracting meaningful insights within each cluster. 

## Conclusion

The project's ultimate assessment will pivot on the efficiency and performance of the developed models. Metrics such as accuracy, precision, recall, and F1-score will evaluate the classification models. 

This comparative analysis evaluates the individual performance and appropriateness of SVM and KNN in predicting caregiver suitability, considering questionnaire responses and additional features.

The integration of both Classification algorithms and CARMA enables a holistic decision-making process, leveraging categorization and grouping patterns. Through this comprehensive model design, we aim to provide a robust and nuanced solution that advances the efficiency and effectiveness of caregiver selection.
