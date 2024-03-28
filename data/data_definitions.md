**table: participants**

**Column Name**|**Data Type**|**Description**
:-----:|:-----:|:-----:
ParticipantID|Integer|A unique identifier for each trial participant.
Age|Integer|The participant's age in years.
Gender|String|The participant's gender (e.g., Male, Female, Other).
Ethnicity|String|The participant's self-identified ethnicity.
Weight|Integer|The participant's weight in kilograms at the start of the trial.
Height|Integer|The participant's height in centimeters at the start of the trial.
MedicalHistory|String|A summary of the participant's medical history relevant to the study.
BaselineVitals|String|A description of the participant's vital signs at baseline. Could be detailed further if necessary.
InclusionCriteriaMet|Boolean|Whether the participant met all the inclusion criteria for the trial.
ExclusionCriteriaMet|Boolean|Whether the participant met any exclusion criteria for the trial.
Accepted|Boolean|Indicates whether the participant was accepted into the trial.
Started|Boolean|Indicates whether the participant started the trial.
Finished|Boolean|Indicates whether the participant completed the trial.

**table: doses**

**Column Name**|**Data Type**|**Description**
:-----:|:-----:|:-----:
DoseID|Integer|A unique identifier for each dose administered during the trial.
ParticipantID|Integer|The unique identifier for the trial participant receiving the dose. Links to the Participants table.
DoseNumber|Integer|The sequence number of the dose for the participant.
AdministrationDate|Date|The date when the dose was administered.
AdverseEvents|String|Description of any adverse events observed after administering the dose.
SeverityOfAdverseEvents|String|The severity of the adverse events (None, Low, Medium, High).
DurationOfAdverseEvents|Integer|The duration of the adverse events in days.
VitalsPostDose|String|A description of the participant's vital signs post-dose.
LabResultsPostDose|String|A description of the participant's laboratory test results post-dose.

