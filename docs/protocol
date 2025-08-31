# ILAE Common Data Models Task Force OHDSI Pilot Study Proposal

Our present goal is to further validate and demonstrate the feasibility of common data model methods for the reliable identification and study of patients with epilepsy and, in particular, drug resistant epilepsy (DRE) across clinical settings and data sources. The Observational Medical Outcomes Partnership (OMOP) Common Data Model¹ (CDM) is a standard that normalizes the structure and content of observational medical data across data sources. OMOP CDM is used across the OHDSI open network of participating sites and databases with over 800 million patients in 82 repositories and 17 countries.¹ Our recent work characterized unexplained variability in treatment pathways for patients with epilepsy.² ³ We then validated computable phenotype algorithms to identify patients with drug resistance in electronic health record (EHR) and administrative data⁴ and identified demographic and clinical factors associated with neurodiagnostic evaluation in our EHR-derived cohort and the broader US population.⁵  

The proposed network study will validate and compare phenotype algorithms to identify patients meeting criteria for epilepsy and DRE in multiple OHDSI databases, characterize treatment pathways, and identify rates and predictors of presurgical evaluation among patients with DRE in these longitudinal data.

---

## Aim 1
Implement, characterize and systematically compare computable phenotype algorithms for:  
(a) new onset epilepsy and  
(b) drug resistant epilepsy (DRE)  

using the OMOP common data model across multiple OHDSI databases. Using multiple OHDSI databases from participating sites, we will characterize and compare epilepsy and DRE cohort characteristics. We will use established phenotypes and compare incidence rates and cohort characteristics across data sources. Where linked data is available, we will determine positive predictive value (precision) against electronic health record manual chart review and sensitivity (recall) against prospectively maintained epilepsy disease registries (e.g. the CANOE registry).

---

## Aim 2
Characterize variability in pharmacotherapy treatment pathways for new onset epilepsy.  

We will conduct a descriptive retrospective observational study to examine use of antiseizure medications across the OHDSI network. Prevalence in use of antiseizure medications (ASMs) will be calculated over time. We will construct sunburst plots to demonstrate the proportion of patients treated with each sequence of antiseizure medications. Treatment pathways will be compared across centers, over time, and on the basis of age, sex and epilepsy type. 

---

## Aim 3
Identify the rate and predictors of care use among patients with:  
(a) new onset epilepsy and  
(b) drug resistant epilepsy  

### 3a. New Onset Epilepsy
We will determine the rate and predictors of:  
1. EEG  
2. MRI brain  
3. Visit types (OP, IP, ED; epilepsy and non-epilepsy).  

### 3b. Drug Resistant Epilepsy
We will determine the rate and predictors of:  
1. Neurodiagnostic evaluation  
2. Epilepsy surgery in the 2 years following drug resistance.  

We will identify demographic and clinical predictors of all outcomes, comparing results across sites.

---

This work will establish common data model methodology and best practices for future multi-institutional, multi-database studies of epilepsy and drug-resistance across the OHDSI network. These initial studies will also provide new information about unexplained treatment variability and addressable barriers to appropriate care for patients with epilepsy.

---

# Aim 1 Details

**Time window for all data:** 2005-01-01 to 2025-01-01  

### Inclusion Criteria – Epilepsy Cohort
Patients who fulfilled one of the following 3 criteria between 2010-01-01 and 2024-01-01:  

1. A first occurrence of an epilepsy diagnosis during an inpatient hospitalization or emergency department (ED) visit [25], [26].  
2. At least 2 outpatient epilepsy diagnoses within 2 years that are at least 30 days apart [26].  
3. At least 1 epilepsy or convulsion/seizure diagnosis **AND** a first ASM exposure within 2 years [27], [28], [29].  

- **Index date** = the first date on which any of the above inclusion criteria are met.  
- **Look back requirement:** At least 1 year of observation in the database before the index date.

### Inclusion Criteria – Drug Resistant Epilepsy Cohort
Patients who fulfill one of the following criteria between 2010-01-01 and 2024-01-01 (censor Columbia data prior to 3/2020):  

1. At least 1 intractable epilepsy diagnosis **AND** 2 or more unique non–gabapentinoid antiseizure medication exposures (each with ≥90-day drug era) [ref].  
2. ≥3 distinct antiseizure medication exposures within 3 years **OR** acute hospital visit with epilepsy/convulsions following fillings of prescriptions for two distinct ASMs [ref].  
3. Drug-resistant epilepsy diagnosis [ref].  

- **Index date** = the first date on which any of the above inclusion criteria are met.  
- **Look back requirement:** At least 1 year of observation in the database before the index date (part of initial inclusion criteria).  

### Analysis
- Cohort characteristics and other OMOP phenotype validation tools will be used in all databases to compare the performance of the different phenotypes.  
- PPV and sensitivity for epilepsy and DRE will be calculated against validated cohorts in the CANOE registry.

---

# Aim 2 Details

We will conduct a descriptive retrospective observational study to examine use of antiseizure medications across the OHDSI network. Prevalence in use of antiseizure medications (ASMs) will be calculated over time.  

- **Numerator:** number of people dispensed a particular antiseizure medicine each month.  
- **Denominator:** number of persons in the same strata, estimated using the database population figure.  
- **Prevalence:** number of people dispensed the ASM per 1000 population.  

Persistence with treatment will be investigated to identify usage patterns.

### Treatment Pattern Measures
- Time from index date to switching within study period (in days)  
- Time from index date to treatment augmentation within study period (in days)  
- Time from index date to discontinuation within study period (in days)  
- Time from treatment discontinuation to re-initiation within study period (in days)  

Treatment discontinuation, switching, and re-initiation will be defined precisely (with XX days thresholds to be determined).  

Kaplan-Meier survival analysis will be used to estimate persistence. Kaplan-Meier survival curve:  
- **Y-axis:** proportion of persistent persons  
- **X-axis:** time  

Add ASM pathways antecedent to (a) video EEG and (b) surgery. Reverse sunburst plot or river plot.

---

# Aim 3 Details

### Rates of Epilepsy Care Use

#### Aim 3a. New Onset Epilepsy
Among patients with new onset epilepsy and at least 2 years of observation after the index date, we will determine the proportion of patients having the following care:  
(a) within 2 years before and 2 years after the index date  
(b) within 2 years before and all time after the index date  

- ≥1 Any EEG: `4181917`  
- ≥1 MRI brain: `37311324`  
- ≥2 non-emergency epilepsy visits: Inpatient or outpatient  
  - Visit type `[9201, 9202, 8756]` with diagnosis `[380378]`  

#### Aim 3b. Drug Resistant Epilepsy
Among patients with DRE and at least 2 years of observation after the index date (denote in table and censor), we will determine the proportion of patients having the following care:  
(a) within 2 years before and 2 years after the index date  
(b) within 2 years before and all time after the index date  

- ≥1 video EEG: `[4100787, 4102081, 2314150]`  
  - CUIMC (codes by BY):  
    - SNOMED: `27808002, 252738008`  
    - CPT4: `95951, 95718, 95720, 95722, 95724, 95726`  
    - ICD-9: `89.19`  
- ≥1 MRI brain: `[37311324]`  
- ≥1 advanced brain imaging: `[4083104, 36713060, 2212017, 45887655, 4134007, 2314156]`  
- ≥1 neuropsychological evaluation: `[4163403, 4217207, 4061974, 4264103, 2007705, 2314185, 2314189, 2314192, 2314194, 2314195, 2314196, 927172, 927173, 927174, 927175]`  
- Epilepsy surgery (intracranial monitoring or therapeutic surgery):  
  - Codes: `2110457, 2110458, 40479988, ​​2110543, 40479650, 3655808, 2000126, 4200691, 4232246, 4218537, 2110459, 2110462, 2110463, 2110464, 2110465, 2110481, 2110482, 2110466, 2000125, 36905041, 2722695, 2110468, 4031033, 42873047, 2000236, 40757131, 42734019, 4262290, 2110554, 2110555, 2110557, 2110558, 2110559, 2110560, 40756794, 2000158, 2723316, 2723319, 2723322, 608574, 1389720, 1389721, 40756779, 2791323, 2791327`  

**Composite outcome (comprehensive evaluation):**  
- (i) AND (ii OR iii) AND (iv)  

Same time window as constituent outcomes; order does not matter.

---

## Time to Event Analysis
- **Model:** Cox proportional hazards model  
- Outcomes:  
  - (3a) MRI and any EEG among those with new onset epilepsy  
  - (3b) Video EEG and surgery among those with DRE  

**Pre-index events:** modeled as events at time = 0.  
**Sensitivity analysis:** exclude patients with pre-index events.  

---

## Covariates
- **Demographics:**  
  - Age at index date  
  - Sex  
  - Observation time before/after index date  
  - Race (if available)  
  - Ethnicity (if available)  

- **Epilepsy classification:**  
  - Focal: ≥1 focal epilepsy diagnosis and 0 generalized epilepsy diagnoses in the year preceding index date  
  - Generalized: ≥1 generalized epilepsy diagnosis and 0 focal epilepsy diagnoses in the year preceding index date  

- **Comorbidities:** See **Table 1.3** codes and lookback  
- **Care patterns:** Number of ED, IP, OP visits with epilepsy/seizure diagnosis (categorized as 0, 1, ≥2)  
- **Procedures:** CT scan within 1 year before index date  
- **Drugs:** Unique non–gabapentinoid ASM exposure eras of ≥90 days (categorized as 2, 3, 4, ≥5)  

---

# Appendix
Observational Health Data Sciences and Informatics (OHDSI) Standardized Vocabularies Concept Codes (available at [athena.ohsi.org](https://athena.ohdsi.org))  

## 1.1 Antiseizure Medication (ASM) Exposures by RxNorm Active Pharmaceutical Ingredients

| Ingredient       | Concept ID | Concept Code |
|------------------|------------|--------------|
| **Non-Gabapentinoid ASM** | | |
| Brivaracetam     | 35604901   | 1739745      |
| Cannabidiol      | 1510417    | 2045371      |
| Carbamazepine    | 740275     | 2002         |
| Cenobamate       | 37497998   | 2265690      |
| Clobazam         | 19050832   | 21241        |
| Clonazepam       | 798874     | 2598         |
| Eslicarbazepine  | 44507780   | 1482502      |
| Ethosuximide     | 750119     | 4135         |
| Ethotoin         | 21604398   | N03AB01      |
| Ezogabine        | 40239995   | 1112990      |
| Felbamate        | 795661     | 24812        |
| Lacosamide       | 19087394   | 623400       |
| Lamotrigine      | 705103     | 28439        |
| Levetiracetam    | 711584     | 114477       |
| Mephobarbital    | 702685     | 6758         |
| Methsuximide     | 759401     | 47858        |
| Oxcarbazepine    | 21604418   | N03AF02      |
| Perampanel       | 42904177   | 1356552      |
| Phenobarbital    | 734275     | 8134         |
| Phenytoin        | 740910     | 8183         |
| Primidone        | 751347     | 8491         |
| Rufinamide       | 19006586   | 69036        |
| Stiripentol      | 35200286   | 2054968      |
| Tiagabine        | 715458     | 31914        |
| Topiramate       | 742267     | 38404        |
| Valproate        | 745466     | 40254        |
| Vigabatrin       | 19020002   | 14851        |
| Zonisamide       | 21604437   | N03AX15      |
| **Gabapentinoid ASM** | | |
| Gabapentin       | 713192     | 72236        |
| Pregabalin       | 734354     | 187832       |

Exclusions: Diazepam, lorazepam, midazolam (short-acting rescue); fosphenytoin (IV only).

---

## 1.2 Epilepsy Diagnoses
- **Epilepsy:** SNOMED `84757009` (OMOP: `380378`)  
- **Seizure:** SNOMED `91175000` (OMOP: `377091`)  
- **Intractable epilepsy diagnosis code:** ICD-9/ICD-10 listed; custom OMOP concept set  

Focal and generalized epilepsy codes listed.  
Complete SNOMED subsumption list: [Epilepsy 380378](https://athena.ohdsi.org/search-terms/terms/380378)  

---

## 1.3 Co-morbidity Diagnoses
(Full table with SNOMED, ICD codes, lookback windows — included in source text.)

---

## 1.4 Visits
Definitions of ED, IP, OP visit OMOP codes.  

---

## 1.5 Phase 1 Diagnostic Procedures
Includes EEG (routine, video, long-term), CT head, MRI brain, PET, SPECT, fMRI, Wada test, neuropsychological evaluation, with SNOMED/ICD/CPT/OMOP mappings.  

---

## 1.6 Surgical Procedures
Intracranial monitoring, resections, transections, callosotomy, hemispherectomy, vagus nerve stimulation, intracranial neuromodulation, pulse generator insertion, LITT, with SNOMED/ICD/CPT/OMOP codes.  

---

# References
1. Hripcsak G, Duke JD, Shah NH, Reich CG, Huser V, Schuemie MJ, Suchard MA, Park RW, Wong ICK, Rijnbeek PR, van der Lei J, Pratt N, Norén GN, Li YC, Stang PE, Madigan D, Ryan PB. *Observational Health Data Sciences and Informatics (OHDSI): Opportunities for Observational Researchers.* Stud Health Technol Inform. 2015;216:574–578. PMCID: PMC4815923  
2. Spotnitz M, Ostropolets A, Castano VG, Natarajan K, Waldman GJ, Argenziano M, Ottman R, Hripcsak G, Choi H, Youngerman BE. *Patient characteristics and antiseizure medication pathways in newly diagnosed epilepsy: Feasibility and pilot results using the common data model in a single-center electronic medical record database.* Epilepsy Behav. 2022 Apr;129:108630. PMID: 35276502  
3. Terman SW, Youngerman BE, Choi H, Burke JF. *Antiseizure medication treatment pathways for US Medicare beneficiaries with newly treated epilepsy.* Epilepsia. 2022 Jun;63(6):1571–1579. PMCID: PMC9314094  
4. Castano VG, Spotnitz M, Waldman GJ, Joiner EF, Choi H, Ostropolets A, Natarajan K, McKhann GM, Ottman R, Neugut AI, Hripcsak G, Youngerman BE. *Identification of patients with drug-resistant epilepsy in electronic medical record data using the Observational Medical Outcomes Partnership Common Data Model.* Epilepsia. 2022 Nov;63(11):2981–2993. PMID: 36106377  
5. Spotnitz M, Ekanayake CD, Ostropolets A, McKhann GM, Choi H, Ottman R, Neugut AI, Hripcsak G, Natarajan K, Youngerman BE. *Use of Recommended Neurodiagnostic Evaluation Among Patients With Drug-Resistant Epilepsy.* JAMA Neurol. 2024 Apr 1;e240551. PMCID: PMC10985618  

