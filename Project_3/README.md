## Immunosuppression and COVID-19: Is There Increased Mortality Risk?

### Description
Does immunosuppression represent greater risk for COVID mortality?  Does it represent greater risk for ventilation or for intensive critical care?  

### Features and Target Variables
Targets:
mortality (represented by `date_died`)
ICU admission
intubation

Features:
* Age
* Sex
* COVID test result
* COVID exposure
* Co-morbidities:
  * pneumonia
  * cardiovascular disease
  * hypertension
  * asthma
  * chronic obstructive pulmonary disease (COPD)
  * diabetes
  * obesity
  

### Data Used
Dataset including ~550,000 patients in Mexican hospitals, collected by the government of Mexico.  

### Tools Used
SKLearn

Seaborn

Matplotlib


### Possible impacts
As of the date of this writing, neither the American College of Rheumatology nor the British College of Rheumatology have issued specific guidance to immunosuppressed patients regarding their risk of mortality should they contract COVID-19.  It remains an open question as to whether immunosuppression as a factor impacts mortality for this particular infection.

While some small pilot studies exist, and limited self-reported data exists regarding rheumatological and other illnesses and COVID-19, there is not yet any aggregated data nor any overview studies detailing what additional risk immunosuppressive medications might pose in light of this pandemic. 

Fortunately, the dataset aggregated by the government of Mexico, including ~500,000 COVID patients, does track immunosuppression as a feature of COVID patients being treated at Mexican hospitals.  Along with the highest-risk comorbidities (hypertension, cardiovascular disease, asthma, COPD), this dataset also tracks immunosuppression and an aggregated category of 'other diseases'.  

Most of the existing controlled trials have n of 200-800, and so represent small samples.  This aggregated data, including ~9000 immunosuppressed individuals, can provide greater insight into the relationship between immunosuppression, ICU care, intubation, and mortality risk.
