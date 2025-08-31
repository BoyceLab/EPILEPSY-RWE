# ILAE Common Data Models Task Force OHDSI Pilot Study Proposal

Our present goal is to further validate and demonstrate the feasibility of common data model methods for the reliable identification and study of patients with epilepsy and, in particular, drug resistant epilepsy (DRE) across clinical settings and data sources. The Observational Medical Outcomes Partnership (OMOP) Common Data Model¹ (CDM) is a standard that normalizes the structure and content of observational medical data across data sources. OMOP CDM is used across the OHDSI open network of participating sites and databases with over 800 million patients in 82 repositories and 17 countries.¹ Our recent work characterized unexplained variability in treatment pathways for patients with epilepsy.²,³ We then validated computable phenotype algorithms to identify patients with drug resistance in electronic health record (EHR) and administrative data⁴ and identified demographic and clinical factors associated with neurodiagnostic evaluation in our EHR-derived cohort and the broader US population.⁵

The proposed network study will validate and compare phenotype algorithms to identify patients meeting criteria for epilepsy and DRE in multiple OHDSI databases, characterize treatment pathways, and identify rates and predictors of presurgical evaluation among patients with DRE in these longitudinal data.

---

## Aim 1
Implement, characterize and systematically compare computable phenotype algorithms for (a) new onset epilepsy and (b) drug resistant epilepsy (DRE) using the OMOP common data model across multiple OHDSI databases. Using multiple OHDSI databases from participating sites, we will characterize and compare epilepsy and DRE cohort characteristics. We will use established phenotypes and compare incidence rates and cohort characteristics across data sources. Where linked data is available, we will determine positive predictive value (precision) against electronic health record manual chart review and sensitivity (recall) against prospectively maintained epilepsy disease registries (e.g. the CANOE registry).

---

## Aim 2
Characterize variability in pharmacotherapy treatment pathways for new onset epilepsy.

We will conduct a descriptive retrospective observational study to examine use of antiseizure medications across the OHDSI network. Prevalence in use of antiseizure medications (ASMs) will be calculated over time. We will construct sunburst plots to demonstrate the proportion of patients treated with each sequence of antiseizure medications. Treatment pathways will be compared across centers, over time, and on the basis of age, sex and epilepsy type.

---

## Aim 3
Identify the rate and predictors of care use among patients with (a) new onset epilepsy and (b) drug resistant epilepsy.

### 3a. New Onset Epilepsy
We will determine the rate and predictors of (i) EEG, (ii) MRI brain and (iii) visit types (OP, IP, ED; epilepsy and non-epilepsy).

### 3b. Drug Resistant Epilepsy
We will determine the rate and predictors of (iii) neurodiagnostic evaluation and (iv) epilepsy surgery in the 2 years following drug resistance.

We will identify demographic and clinical predictors of all outcomes, comparing results across sites.

---

This work will establish common data model methodology and best practices for future multi-institutional, multi-database studies of epilepsy and drug-resistance across the OHDSI network. These initial studies will also provide new information about unexplained treatment variability and addressable barriers to appropriate care for patients with epilepsy.

---

## Aim 1

**Time window for all data:** 2005-01-01 to 2025-01-01

### Inclusion Criteria — Epilepsy Cohort
Patients who fulfilled one of the following 3 criteria between 2010-01-01 and 2024-01-01:

1. A first occurrence of an epilepsy diagnosis during an inpatient hospitalization or emergency department (ED) visit \[25], \[26].
2. At least 2 outpatient epilepsy diagnoses within 2 years that are at least 30 days apart \[26].
3. At least 1 epilepsy or convulsion/seizure diagnosis **AND** a first ASM exposure within 2 years \[27], \[28], \[29].

- **Index date:** the first date on which any of the above inclusion criteria are met.  
- **Look back requirement:** At least 1 year of observation in the database before the index date.

### Inclusion Criteria — Drug Resistant Epilepsy cohort
Patients who fulfill one of the following criteria between 2010-01-01 and 2024-01-01 (censor Columbia data prior to 3/2020):

1. At least 1 intractable epilepsy diagnosis **AND** 2 or more unique non–gabapentinoid antiseizure medication exposures (each with ≥90-day drug era) \[ref]  
2. ≥3 distinct antiseizure medication exposures within 3 years **OR** acute hospital visit with epilepsy/convulsions following fillings of prescriptions for two distinct ASMs \[ref]  
3. Drug-resistant epilepsy diagnosis \[ref]

- **Index date:** the first date on which any of the above inclusion criteria are met.  
- **Look back requirement:** At least 1 year of observation in the database before the index date (part of initial inclusion criteria).

### Analysis
- Cohort characteristics and other OMOP phenotype validation tools will be used in all databases to compare the performance of the different phenotypes.  
- PPV and sensitivity for epilepsy and DRE will be calculated against validated cohorts in the CANOE registry.

---

## Aim 2 (Details)

We will conduct a descriptive retrospective observational study to examine use of antiseizure medications across the OHDSI network. Prevalence in use of antiseizure medications (ASMs) will be calculated over time. The numerator will be the number of people dispensed a particular antiseizure medicine each month. The denominator will be the number of persons in the same strata, estimated using the database population figure. Prevalence will be expressed as number of people dispensed the ASM per 1000 population. Persistence with treatment will be investigated to identify usage patterns.

We will construct sunburst plots to demonstrate the proportion of patients treated with each sequence of antiseizure medications. Treatment pathways will be compared across centers, over time, and on the basis of age, sex and epilepsy type. The duration of time from treatment initiation to subsequent switch to alternative prophylactic treatment, treatment augmentation, treatment discontinuation and or treatment re-initiation with the antiseizure medicine after discontinuation will be investigated. Persistence will be defined as the continuous refilling of their antiseizure medicine with a time interval equivalent to or fewer than **XX** days. Patients are considered persistent during the study period if there are no gaps of more than **XX** days.

**Treatment pattern measures to report:**
- Time from index date to switching within study period (in days)
- Time from index date to treatment augmentation within study period (in days)
- Time from index date to discontinuation within study period (in days)
- Time from treatment discontinuation to re-initiation within study period (in days)

Treatment discontinuation will be defined as when patients cease the initiated antiseizure medicine without evidence of another refill of the antiseizure medicine after **XX** days. Treatment switching will be identified as when patients discontinuing treatment with the index antiseizure medicine and then fills a prescription for another antiseizure medicine following the **XX** days. Treatment re-initiation is identified when patients start on one antiseizure medicine, switch to another and then re-initiates the first antiseziure medicine. The standard Kaplan-Meier survival analysis will be used to estimate persistence to determine cumulative duration of all antiseizure medicines with and without treatment breaks. A Kaplan-Meier survival curve with the y-axis showing the proportion of persistent persons and x-axis showing the time will be plotted.

_Add ASM pathways antecedent to (a) video EEG and (b) surgery. Reverse sunburst plot or river plot._

---

## Aim 3 (Details)

### Rates of epilepsy care use

#### Aim 3a. Among patients with new onset epilepsy and at least 2 years of observation after the index date
We will determine the proportion of patients having the following care (a) within 2 years before and 2 years after the index date, and (b) within 2 years before and all time after the index date:

- ≥1 **Any EEG:** `4181917`  
- ≥1 **MRI brain:** `37311324`  
- ≥2 **non-emergency epilepsy visits:** Inpatient or outpatient — Visit type `[9201, 9202, 8756]` with diagnosis `[380378]`

#### Aim 3b. Among patients with DRE and at least 2 years of observation after the index date (denote in table and censor)
We will determine the proportion of patients having the following care (a) within 2 years before and 2 years after the index date, and (b) within 2 years before and all time after the index date:

- ≥1 **video EEG:** `[4100787, 4102081, 2314150]`  
  **For CUIMC (codes provided by BY):**  
  - **SNOMED:** `27808002, 252738008`  
  - **CPT4:** `95951, 95718, 95720, 95722, 95724, 95726`  
  - **ICD-9:** `89.19`
- ≥1 **MRI brain:** `[37311324]`
- ≥1 **advanced brain imaging:** `[4083104, 36713060, 2212017, 45887655, 4134007, 2314156]`
- ≥1 **neuropsychological evaluation:** `[4163403, 4217207, 4061974, 4264103, 2007705, 2314185, 2314189, 2314192, 2314194, 2314195, 2314196, 927172, 927173, 927174, 927175]`
- **Epilepsy surgery: intracranial monitoring or therapeutic surgery:**  
  `2110457, 2110458, 40479988, ​​2110543, 40479650, 3655808, 2000126, 4200691, 4232246, 4218537, 2110459, 2110462, 2110463, 2110464, 2110465, 2110481, 2110482, 2110466, 2000125, 36905041, 2722695, 2110468, 4031033, 42873047, 2000236, 40757131, 42734019, 4262290, 2110554, 2110555, 2110557, 2110558, 2110559, 2110560, 40756794, 2000158, 2723316, 2723319, 2723322, 608574, 1389720, 1389721, 40756779, 2791323, 2791327`

**Composite outcome (comprehensive evaluation):** (i) **AND** (ii **OR** iii) **AND** (iv)  
_Same time window as the constituent outcomes and order does not matter._

### Time to Event Analysis
We will construct a Cox proportional hazards model to analyze association of the below covariates with the time to:
- **(3a)** MRI and any EEG among those with new onset epilepsy, and
- **(3b)** video EEG and surgery among those with DRE.

**Pre-index events** will be modeled as events at time = 0.  
We will conduct a sensitivity analysis in which patients with pre-index events are excluded from the analysis.

### Covariates

**Demographic variables**
- Age at the index date
- Sex
- Observation time before the index date
- Observation time after the index date
- Race — to the extent available in each data source
- Ethnicity — to the extent available in each data source

**Epilepsy**
- **Focal:** ≥1 focal epilepsy diagnosis and 0 generalized epilepsy diagnoses in the year preceding the index date
- **Generalized:** ≥1 generalized epilepsy diagnosis and 0 focal epilepsy diagnoses in the year preceding the index date

**Co-morbidities**  
_Table 1.3 specifies codes and lookback (see tables below)._

**Care patterns**
- Number of each visit type (emergency department, inpatient, and outpatient) with a diagnosis of epilepsy or seizure within 1 year preceding the index date (categorized as 0, 1, or ≥2).
- Procedures included a computed tomography scan of the head within 1 year before the index date.
- Drug variables included the number of unique non–gabapentinoid antiseizure medication exposure eras of at least 90 days’ duration any time preceding the index date (categorized as 2, 3, 4, or ≥5).

---

# Appendix. Observational Health Data Sciences and Informatics (OHDSI) Standardized Vocabularies Concept Codes
_Available at_ <https://athena.ohdsi.org>.

## 1.1. Antiseizure medication (ASM) Exposures by RxNorm Active Pharmaceutical Ingredients

| Ingredient | Concept ID | Concept Code |
|---|---:|---|
| **Non-Gabapentinoid ASM** |  |  |
| Brivaracetam | 35604901 | 1739745 |
| Cannabidiol | 1510417 | 2045371 |
| Carbamazepine | 740275 | 2002 |
| Cenobamate | 37497998 | 2265690 |
| Clobazam | 19050832 | 21241 |
| Clonazepam | 798874 | 2598 |
| Eslicarbazepine | 44507780 | 1482502 |
| Ethosuximide | 750119 | 4135 |
| Ethotoin | 21604398 | N03AB01 |
| Ezogabine | 40239995 | 1112990 |
| Felbamate | 795661 | 24812 |
| Lacosamide | 19087394 | 623400 |
| Lamotrigine | 705103 | 28439 |
| Levetiracetam | 711584 | 114477 |
| Mephobarbital | 702685 | 6758 |
| Methsuximide | 759401 | 47858 |
| Oxcarbazepine | 21604418 | N03AF02 |
| Perampanel | 42904177 | 1356552 |
| Phenobarbital | 734275 | 8134 |
| Phenytoin | 740910 | 8183 |
| Primidone | 751347 | 8491 |
| Rufinamide | 19006586 | 69036 |
| Stiripentol | 35200286 | 2054968 |
| Tiagabine | 715458 | 31914 |
| Topiramate | 742267 | 38404 |
| Valproate | 745466 | 40254 |
| Vigabatrin | 19020002 | 14851 |
| Zonisamide | 21604437 | N03AX15 |
| **Gabapentinoid ASM** |  |  |
| Gabapentin | 713192 | 72236 |
| Pregabalin | 734354 | 187832 |

**Exclusions:** Diazepam, lorazepam, and midazolam were excluded as these medications are typically used as short-acting rescue medication. Fosphenytoin was excluded as it is only available in intravenous form and therefore unlikely to be included in a chronic disease treatment pathway.

---

## 1.2. Epilepsy Diagnoses

**Core concepts**

| Concept | Coding System | Code | OMOP Concept ID |
|---|---|---|---:|
| Epilepsy | SNOMED | 84757009 | 380378 |
| Seizure | SNOMED | 91175000 | 377091 |
| Intractable epilepsy diagnosis code | ICD-9-CM | 345.01, 345.11, 345.41, 345.51, 345.61, 345.71, 345.81, 345.91 | — |
|  | ICD-10-CM | G40.011, G40.019, G40.111, G40.119, G40.211, G40.219, G40.311, G40.A11, G40.B11, G40.B19, G40.411, G40.419, G40.803, G40.804, G40.813, G40.814, G40.823, G40.824, G40.911, G40.919 | — |

**Focal epilepsy**  
≥1 focal epilepsy diagnosis and 0 generalized epilepsy diagnoses, where focal epilepsy includes:

| Coding System | Codes |
|---|---|
| ICD-9-CM | 345.4, 345.5, 345.7 |
| ICD-10-CM | G40.0, G40.1, G40.2 |

**SNOMED Concepts (Focal epilepsy)**

| Concept | OMOP Concept ID |
|---|---:|
| Focal epilepsy | 374915 |
| Benign infantile focal epilepsy with midline spikes and waves during sleep | 36674783 |
| Epilepsy co-occurrent and due to mesial temporal sclerosis | 37110674 |
| Epilepsy due to Rasmussen syndrome | 37166916 |
| Epilepsy due to intracranial tumor | 37110524 |
| Epilepsy of infancy with migrating focal seizures | 37118656 |
| Infant epilepsy with migrant focal crisis | 37110163 |
| Malignant migrating partial seizures of infancy | 37205067 |
| Scar epilepsy | 3657974 |

**Generalized epilepsy**  
≥1 generalized epilepsy diagnosis and 0 focal epilepsy diagnoses where generalized epilepsy includes:

| Coding System | Codes |
|---|---|
| ICD-9-CM | 345.0, 345.1, 345.2, 345.3 |
| ICD-10-CM | G40.3, G40.A, G40.B, G40.4 |

**SNOMED Concepts (Generalized epilepsy)**

| Concept | OMOP Concept ID |
|---|---:|
| Generalized epilepsy | 4055361 |
| Atypical absence epilepsy | 43530704 |
| Benign adult familial myoclonic epilepsy | 37397175 |
| Cryptogenic late-onset epileptic spasms | 36680607 |
| Developmental and epileptic encephalopathy | 37168142 |
| Epileptic encephalopathy | 36716897 |
| Familial infantile myoclonic epilepsy | 37205064 |
| Progressive myoclonic epilepsy | 4147501 |
| Tonic-clonic epilepsy | 4232071 |

**Complete list:** SNOMED codes which “Epilepsy” subsumes: <https://athena.ohdsi.org/search-terms/terms/380378>

---

## 1.3. Co-morbidity Diagnoses  
_*Visit diagnoses only (exclude “problem list”)*_

| Concept | Included Concept Codes | OMOP Concept ID(s) | Lookback period |
|---|---|---|---|
| Anxiety | SNOMED: 197480006 | 442077 | 1 year prior |
| Depression | SNOMED: 35489007 | 440383 | 1 year prior |
| Headache disorder | SNOMED: 230461009 | 375527 | 1 year prior |
| Intracranial neoplasm | SNOMED: 254935002 (Includes ICD-9-CM: 191.x, 192.1, 198.3, 225.0, 225.1, 225.2, 228.02, 237.5, 237.6, 239.6; ICD-10-CM: C70.0, C71.x, C72.4, C72.5, C79.3, D32.0, D32.9, D33.0, D33.1, D33.2, D33.3, D42.0, D42.9, D43.0, D43.1, D43.2, D43.3, Q85.1) | 4116092, 36768862 | Any time prior |
| Lesion of brain | SNOMED: 301766008 | 4200516 | Any time prior |
| Dementia | SNOMED: 52448006 | 4182210 | Any time prior |
| Tuberous sclerosis | SNOMED: 7199000 | 380839 | Any time prior |
| Traumatic Brain Injury | SNOMED: 127295002 | 4132546 | Any time prior |

---

## 1.4. Visits

| Concept | Included Concept Codes | OMOP Concept ID(s) |
|---|---|---|
| **Emergency visit** | Emergency Room Visit: ER; Emergency Room and Inpatient Visit: ERIP; Emergency Room – Hospital: CMS 23 | 9203 OR 262 OR 8870 |
| **Non-emergency inpatient visit** | Inpatient Visit: IP | 9201 |
| **Outpatient visit** | Outpatient Visit: OP; Outpatient Hospital: CMS 22 | 9202 OR 8756 OR 581477 |

---

## 1.5. Phase 1 Diagnostic Procedures

| Concept | Coding System / Notes | Codes | OMOP Concept ID(s) |
|---|---|---|---|
| Any EEG | SNOMED (includes routine, video and other long-term EEG codes below) | 54550000 | 4181917 |
| **Video EEG** | SNOMED; CPT4; ICD-9; ICD-10-PCS | SNOMED: 27808002, 252738008; CPT4: 95951, 95718, 95720, 95722, 95724, 95726; ICD-9: 89.19; ICD-10-PCS: 4A1034Z, 4A1074Z, 4A1084Z, 4A10X4Z | 4100787, 4102081, 2314150 _(incomplete)_ |
| **Routine EEG** | CPT | 95812, 95813, 95816, 95819, 95822 | NA |
| **Other long-term EEG** | CPT | 95827, 95830, 95950, 95953, 95956 | NA |
| Computed Tomography (CT) head | SNOMED | 303653007 | 4125350 |
| Magnetic Resonance Imaging (MRI) brain | SNOMED (includes CPT, ICD-9, ICD-10-PCS) | SNOMED: 816077007; CPT: 70551, 70552, 70553; ICD-9: 88.91; ICD-10-PCS: B030ZZZ, B030YZZ, B030Y0Z | 37311324 |
| **Advanced brain imaging** |  |  |  |
| — Positron emission tomography (PET) | OHDSI (includes CPT4) | 241435001; CPT4: 78608 | 4083104 |
| — Single-Photo Emission Computed Tomography (SPECT) | SNOMED; CPT4 | SNOMED: 16548951000119100; CPT4: 78607 | 36713060, 2212017 |
| — Functional MRI (fMRI) | CPT4 | 70554, 70555 | 45887655 |
| — Wada test | SNOMED; CPT4 | SNOMED: 262275002; CPT4: 95958 | 4134007, 2314156 |
| Neuropsychological Evaluation | SNOMED; ICD-9CM; CPT4 | SNOMED: 45392008, 72657008, 1999007, 36338000; ICD-9CM: 94.0, 94.01, 94.02, 94.03, 94.08, 94.09; CPT4: 96101, 96110, 96116, 96118, 96119, 96120, 96132, 96133, 96136, 96137 | 4163403, 4217207, 4061974, 4264103, 2007705, 2314185, 2314189, 2314192, 2314194, 2314195, 2314196, 927172, 927173, 927174, 927175 |

---

## 1.6. Surgical Procedures

| Concept | Coding System(s) | Codes | OMOP Concept ID(s) |
|---|---|---|---|
| **Intracranial monitoring (Phase 2)** | Subdural grid — CPT; SNOMED. Depth electrodes (SEEG) — CPT; SNOMED | Subdural grid CPT: 61531 (strip/burr), 61533 (grid/craniotomy); SNOMED: 441617000. SEEG CPT: 61760; SNOMED: 441597006 (Placement of depth electrode into brain for electroencephalography), 870257001 (Stereoelectroencephalography) | 2110457, 2110458, 40479988, ​​2110543, 40479650, 3655808 |
| **Resection (epilepsy specific)** | ICD-9; SNOMED; CPT | ICD-9: 01.53 (lobectomy of brain); SNOMED: 53423001, 439493007, 39667005; CPT: 61534, 61536, 61537, 61538, 61539, 61540, 61566 | 2000126, 4200691, 4232246, 4218537, 2110459, 2110462, 2110463, 2110464, 2110465, 2110481 |
| **Resection (nonspecific; may or may not include depending on goals)** | ICD-9; ICD-10 | ICD-9: 01.59 (Other excision or destruction of lesion or tissue of brain); ICD-10: 00500ZZ, 00570ZZ, 00B00ZZ, 00B60ZZ | — |
| Multiple subpial transections | CPT | 61567 | 2110482 |
| Corpus callosotomy | CPT | 61541 | 2110466 |
| Hemispherectomy / hemispherotomy | ICD-9; ICD-10; CPT; SNOMED | ICD-9: 01.52; ICD-10: 00B70ZZ; CPT: 61543; SNOMED: 14247003, 451040005 | 2000125, 36905041, 2722695, 2110468, 4031033, 42873047 |
| Vagus nerve stimulation (VNS) | ICD-9; CPT | ICD-9: 04.92; CPT: 64568 (active), 64573 (deprecated 2011) | 2000236, 40757131, 42734019 |
| Intracranial Neuromodulation (DBS/RNS) | SNOMED; CPT; ICD-9; ICD-10 | SNOMED: 35797001; CPT: 61850, 61860, 61863, 61864, 61867, 61868; ICD-9: 01.20, 02.93; ICD-10: 00H00MZ, 00H03MZ, 00H04MZ | 4262290, 2110554, 2110555, 2110557, 2110558, 2110559, 2110560, 40756794, 2000158, 2723316, 2723319, 2723322 |
| Insertion/replacement of pulse generator | CPT; ICD | CPT: 61885, 61886, 61889; ICD: 01.20 | — |
| Laser interstitial thermal therapy (LITT) | SNOMED; CPT; ICD-9; ICD-10 | SNOMED: 1362401000000106; CPT: 61736, 61737 (active since 1/1/2022 only); ICD-9: 17.61; ICD-10: D0Y0KZZ, D0Y1KZZ (deprecated 2024); CPT: 61735 (stereotactic lesion) — may have been used pre-2022; CPT 64999 (unlisted procedure) — may have been used pre-2022 | 608574, 1389720, 1389721, 40756779, 2791323, 2791327 |

---

## References

1. Hripcsak G, Duke JD, Shah NH, Reich CG, Huser V, Schuemie MJ, Suchard MA, Park RW, Wong ICK, Rijnbeek PR, van der Lei J, Pratt N, Norén GN, Li YC, Stang PE, Madigan D, Ryan PB. **Observational Health Data Sciences and Informatics (OHDSI): Opportunities for Observational Researchers.** *Stud Health Technol Inform.* 2015;216:574–578. PMCID: PMC4815923  
2. Spotnitz M, Ostropolets A, Castano VG, Natarajan K, Waldman GJ, Argenziano M, Ottman R, Hripcsak G, Choi H, Youngerman BE. **Patient characteristics and antiseizure medication pathways in newly diagnosed epilepsy: Feasibility and pilot results using the common data model in a single-center electronic medical record database.** *Epilepsy Behav.* 2022 Apr;129:108630. PMID: 35276502  
3. Terman SW, Youngerman BE, Choi H, Burke JF. **Antiseizure medication treatment pathways for US Medicare beneficiaries with newly treated epilepsy.** *Epilepsia.* 2022 Jun;63(6):1571–1579. PMCID: PMC9314094  
4. Castano VG, Spotnitz M, Waldman GJ, Joiner EF, Choi H, Ostropolets A, Natarajan K, McKhann GM, Ottman R, Neugut AI, Hripcsak G, Youngerman BE. **Identification of patients with drug-resistant epilepsy in electronic medical record data using the Observational Medical Outcomes Partnership Common Data Model.** *Epilepsia.* 2022 Nov;63(11):2981–2993. PMID: 36106377  
5. Spotnitz M, Ekanayake CD, Ostropolets A, McKhann GM, Choi H, Ottman R, Neugut AI, Hripcsak G, Natarajan K, Youngerman BE. **Use of Recommended Neurodiagnostic Evaluation Among Patients With Drug-Resistant Epilepsy.** *JAMA Neurol.* 2024 Apr 1; e240551. PMCID: PMC10985618
