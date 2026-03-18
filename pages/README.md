## About

The North American Prodromal Synucleinopathy (NAPS) Consortium for REM Sleep Behavior Disorder is study investigating RBD as a prodromal symptom of neurodegenerative diseases characterized by synuclein pathology, collectively known as synucleinopathies. Funded by the National Institutes of Health (NIH), specifically the National Institute on Aging (NIA) and the National Institute of Neurological Disorders and Stroke (NINDS), the study aims to enable neuroprotective clinical trials to prevent or delay overt synucleinopathies like Parkinson's Disease (PD), dementia with Lewy bodies (DLB), and multiple system atrophy (MSA). 

NAPS began collecting longitudinal, comprehensive clinical data and biomarkers in 2018 on a large cohort of participants with polysomnogram-confirmed idiopathic RBD.

- NAPS1 focused on building a large, multi-center cohort, collecting standardized clinical assessments, and developing biofluid and neurophysiological biomarkers.
- NAPS2 expands on NAPS1 with a more extensive protocol and a core-based structure to support its aims. NAPS2 is a non-randomized, longitudinal natural history study that enrolls >300 participants with idiopathic RBD for annual evaluation and approximately 60 matched healthy controls.

The overarching goals of the NAPS Consortium are to enroll participants for the standardized collection of longitudinal data, analyze these data to develop biomarkers for designing clinical trials, share data and samples with the scientific community, and prepare for large-scale clinical trials.

Only polysomnography (PSG) data from NAPS is being made available to the National Sleep Research Resource (NSRR). For information about data that have been collected, or to request additional data, please use the request form on the [NAPS website (naps-rbd.org)](https://naps-rbd.org/). Baseline characteristic and protocol are available in the referenced publications.

## Methods

### PSG collection

For NAPS1, retrospective clinical PSG data were obtained in EDF format for RSWA analysis. During NAPS2, attended in-lab polysomnography was performed on all RBD and control participants in a controlled, secure environment with continuous technologist monitoring. RBD participants underwent PSG twice (approximately two to three years apart), while controls had a single PSG. The total recording time was advised to be at least 7-8 hours, with an effort to capture at least 5 minutes of artifact-free REM sleep. Digital video and audio were required for all studies.

A variety of digital PSG recording systems were used across the sites, including Natus SleepWorks, Compumedics Grael, Nihon Kohden PSG-1100, and Phillips Alice 6 LDE. PSGs were uploaded to a secure server in EDF format for centralized analysis by the PSG Core. The recommended sampling rate was 500 Hz (minimum 200 Hz).

 The minimum suggested PSG montage included the following channels: 
- EEG (6 channels): F3-M2, F4-M1, C3-M2, C4-M1, O1-M2, O2-M1
- EOG (2 channels): LOC-M2, ROC-M1 
- EMG (Mentalis/Submentalis): Bipolar chin electrodes 
- EMG (Anterior Tibialis): Left and right leg electrodes 
- EMG (Flexor Digitorum Superficialis): Left and right arm electrodes
- ECG: Lead II 
- Snoring: Audio sensor 
- Airflow: Nasal/oral thermistor and nasal pressure transducer 
- Respiratory Effort: Chest and abdominal excursion (e.g., RIP bands) 
- Oximetry: Finger pulse oximeter 
- Body Position: Sensor or technologist observation 

### PSG scoring

All sleep scoring was performed centrally at the Mayo Clinic PSG Core Central Laboratory. Scoring rules for events like apneas or hypopneas were guided by AASM standards for scoring sleep and associated events. Accurate notation of the recording period details including time of lights out, and time of lights on was particularly important using the Technologist Log. Additional technologist log entries during the course of recording included any parasomnias, position, timing of breaks in recording and reasons for the interruptions.

## Data de-identification

All personally identifiable information (PII) was removed from the data files by the NSRR team.

## Data overview

### Covariate/phenotype datasets (CSV) 

The [covariate dataset files](:files_path:/datasets) **naps-dataset-0.1.0.csv** and **naps-harmonized-dataset-0.1.0.csv** contain 138 rows each. The first column ([nsrrid](:variables_path:/nsrrid)) is the unique NAPS subject identifier that can be linked with PSG signal filenames. 

The dataset columns are described in the accompanying data dictionary files. The **variables** data dictionary file [naps-data-dictionary-0.1.0-variables.csv](:files_path:/datasets/naps-data-dictionary-0.1.0-variables.csv) includes folder names (id), labels (display names), descriptions, and other metadata. Categorical variables also include an associated “domain” (e.g., 1=male, 2=female), which are described in the **domains** data dictionary file ([naps-data-dictionary-0.1.0-domains.csv](:files_path:/datasets/naps-data-dictionary-0.1.0-domains.csv) ). 

The history of the covariate dataset and data dictionary files have been tracked on GitHub (https://github.com/nsrr/naps-data-dictionary). 

The harmonized dataset **naps-harmonized-dataset-0.1.0.csv** contains the most frequently used demographic variables available in the NAPS dataset. These variables were curated by the NSRR team to allow ready inter-operability with other NSRR datasets. Key harmonized variables include:

|  |  |
|------------------------------------|------------------------------------|
| **Variable** | **Label** |
| [nsrr_age](:variables_path:/nsrr_age) | Subject age |
| [nsrr_sex](:variables_path:/nsrr_sex) | Subject sex |

### PSG signal files (EDF)

[Raw polysomnography data (.edf) and sleep staging annotations (30-second epochs, .txt)](:files_path:/polysomnography) are available for 138 NAPS1 participants. 

## Access and usage restrictions

The NAPS dataset is only available for non-commercial use.

## Citation and acknowledgments

When using this dataset, users must cite the following publication: 

> [Zhang GQ, Cui L, Mueller R, Tao S, Kim M, Rueschman M, Mariani S, Mobley D, Redline S. The National Sleep Research Resource: towards a sleep data commons. J Am Med Inform Assoc. 2018 Oct 1;25(10):1351-1358. doi: 10.1093/jamia/ocy064. PMID: 29860441; PMCID: PMC6188513.](https://pubmed.ncbi.nlm.nih.gov/29860441/)
>
> [Elliott JE, Lim MM, Keil AT, Postuma RB, Pelletier A, Gagnon JF, St Louis EK, Forsberg LK, Fields JA, Huddleston DE, Bliwise DL, Avidan AY, Howell MJ, Schenck CH, McLeland J, Criswell SR, Videnovic A, During EH, Miglis MG, Shprecher DR, Lee-Iannotti JK, Boeve BF, Ju YS; North American Prodromal Synucleinopathy (NAPS) Consortium. Baseline characteristics of the North American prodromal Synucleinopathy cohort. Ann Clin Transl Neurol. 2023 Apr;10(4):520-535. doi: 10.1002/acn3.51738. Epub 2023 Feb 8. PMID: 36751940; PMCID: PMC10109527.](https://pubmed.ncbi.nlm.nih.gov/36751940/)
>
> [Lim MM, Neilson LE, Elliott JE, Hoang-Dang B, Locke JR, Cunningham H, Brewer J, Dennis L, Dovek L, Pelletier A, St Louis EK, McCarter SJ, Miyagawa T, Davis AA, McLeland JS, Criswell S, Howell MJ, Schenck CH, Avidan AY, Trotti LM, Bliwise DL, Huddleston DE, Videnovic A, Miglis MG, Sum-Ping O, Lee-Iannotti JK, Shprecher DR, Duff K, Ferman TJ, Campbell MC, Fields JA, Gagnon JF, Kotzbauer P, Singer W, Gan-Or Z, Ross OA, Kantarci K, Lowe VJ, Hu XP, Ehgoetz Martens KA, Hu MT, Xiong C, Postuma RB, Boeve BF, Ju YS; NAPS Consortium for RBD. The North American Prodromal Synucleinopathy study: protocol for a multi-site, longitudinal, observational study of idiopathic/isolated rapid eye movement sleep behavior disorder. Sleep Adv. 2026 Jan 19;7(1):zpag007. doi: 10.1093/sleepadvances/zpag007. PMID: 41725984; PMCID: PMC12920605.](https://pmc.ncbi.nlm.nih.gov/articles/PMC12920605/)
 
Users must include the following text in any Acknowledgements section: 

> Data collection and dissemination of the data presented in this manuscript were supported by the NAPS Consortium (R34 AG056639 and U19 AG071754 funded by the National Institutes of Health). The authors acknowledge the invaluable contributions of the participants in NAPS Consortium as well as the assistance of the support staffs at each of the participating sites.

> The National Sleep Research Resource was supported by the U.S. National Institutes of Health, National Heart Lung and Blood Institute (R24 HL114473, 75N92019R002). 6. References The sources do not provide a list of external links or references

## References
- Study on the National Sleep Research Resource (NSRR): http://sleepdata.org/datasets/naps/
- Additional NAPS data at ClinicalTrials.gov (NCT05826457): https://clinicaltrials.gov/study/NCT05826457
- NAPS Consortium for REM Sleep Behavior Disorder: https://www.naps-rbd.org
- NSRR NAPS GitHub Documentation: https://github.com/nsrr/naps-documentation
- NSRR NAPS GitHub Data Dictionary: https://github.com/nsrr/naps-data-dictionary
