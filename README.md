# Public Diabetes Datasets with CGM and CSII

### Database Sources
This dataset review provides a comprehensive list of publicly available diabetes datasets including both continuous glucose monitoring (CGM) and continuous subcutaneous insulin infusion pump data (CSII). These two datatypes are deemed essential for computer modeling and simulation (CM&S).

We used the review by Del Giudice (2025)1 as the starting point because it is recent and applies eligibility criteria closely aligned with our objective of identifying openly accessible dynamic glycemic datasets. Some of the studies identified in the review by Del Guidice included datasets from the JAEB(2) and IrinaStatsLab Awesome-CGM(3) databases. These databases are well maintained but were not fiully included in the review by Del Guidice. We therefore screened both dataset databases, which led to both confirmation of previously identified studies and identification of additional datasets.

(1) Del Giudice, L.L., Piersanti, A., Göbl, C., Burattini, L., Tura, A., Morettini, M., 2025. Availability of Open Dynamic Glycemic Data in the Field of Diabetes Research: A Scoping Review. J Diabetes Sci Technol 19322968251316896. [https://doi.org/10.1177/19322968251316896](https://doi.org/10.1177/19322968251316896)
(2) https://public.jaeb.org/datasets/diabetes
(3) https://github.com/IrinaStatsLab/Awesome-CGM/wiki

### Inclusion Criteria
We are building on top of the eligibility criteria from Del Guidice:
>**Eligibility Criteria**  
>This review targeted scientific articles, websites, and clinical trials that provide free access to data sets including dynamic glycemic data (both human and animal). Both immediately downloadable data sets and data sets downloadable after completion of a request form were included.  
>
>**Exclusion Criteria**  
>This analysis excluded scientific articles, websites, and clinical trials: (1) that do not contain any type of data set; (2) that contain an unavailable data set or a data set available upon payment of subscription fees; (3) in which the data of interest are mainly expressed as a fasting glucose or glycated hemoglobin A1c (HbA1c) as a single value, being very often collected within a basic routine examination and also as secondary variables (ie, belonging to a data set whose primary aim is not collecting glycemic data useful for diabetesrelated research). This latter criterion was necessary to exclude data sets with some diabetes-related information but with limited usefulness for novel diabetes-related research, being them likely already exploited in the original studies for which they were collected.

We further narrowed the exclusion criteria:  
- Studies without both CGM and CSII data
- Nondiabetic and Animal studies
- In-clinic challenge studies (e.g. OGTT and IVGTT)
  - Table 1 from Del Guidice Review paper was excluded altogetehr from the search as it only included challenge tests.
- Parallel pharmacological intervention (e.g. parallel metformin intervention)
- CGM without regulatory approval (e.g. excluding studies using GlucoWatch G2) 

### Results
Across all sources n = 75 datasets were identified (Del Guidice: 20, JAEB: 38, IrinaStatsLab: 20). Out of these, 20 were identified as duplicates. 40 datasets were excluded for various reasons with the majority due to missing insulin (26), offline datasets (5), nondiabetic studies (4), parallel intervention (2).  15 datasets were identified as eligible and are listed below.

|**Dataset**|**Ref**|**Trial ID**|**Study**|**Year**|**N**|**Age (years)**|**Type**|**Duration**|**Patient Days**|**CGM**|**Pump**|
|---|---|---|---|---|---|---|---|---|---|---|---|
|[IOBP2 RCT Public Dataset.zip](https://public.jaeb.org/dataset/579)|[1]|NCT04200313|IOBP2|2022|440|6–71|Type 1|13 weeks|~40k|Dexcom G6|Minimed 670G, 780G; Tandem t:slim X2 Control-IQ; Insulet Omnipod; MDI|
|https://data.mendeley.com/datasets/3hbcscwz44/1|[2]|?|HUPA-UCM diabetes dataset|2024|25|40.50 ± 11.43; 37.63 ± 12.80|Type 1|14 days|~350|FreeStyle Libre 2|Medtronic; Roche|
|[Anderson et al.](https://public.jaeb.org/jdrfapp2/stdy/465)|[3]|NCT02137512|CTR3|2015|30|18+|Type 1|6–9 weeks|~1–2k|Dexcom G4 Platinum|Roche Accu-Chek|
|[Replace-BG Dataset.zip](https://public.jaeb.org/dataset/546)|[4]|NCT02258373|REPLACE-BG|2015|225|25–40|Type 1|6 months|~40k|Dexcom G4|Various|
|[PEDAP Public Dataset - Release 5](https://public.jaeb.org/dataset/599)|[5]|NCT04796779|PEDAP Trial|2024|150|2–6|Type 1|26 weeks–7 months|~30k|Dexcom G5, G6|Tandem t:Slim X2 Control-IQ|
|[FLAIRPublicDataSet.zip](https://public.jaeb.org/dataset/566)|[6]|NCT03040414|FLAIR|2020|113|19 ± 4|Type 1|28–36 weeks|~22k|Medtronic Guardian|Medtronic Guardian|
|[International Diabetes Closed Loop (iDCL) Trial](https://public.jaeb.org/dataset/573)|[7]|NCT03563313|iDCL Trial|2018|168|33 ± 16|Type 1|6 months|~30k|Dexcom G6|Tandem t:Slim X2 Control-IQ|
|[PSO4_Public_Dataset.zip](https://public.jaeb.org/dataset/578)|[8]|NCT01823341|PSO4|2013|82|4–14|Type 1|42 nights|~2k|Medtronic Enlite|MiniMed Paradigm Veo|
|[PSO3_Public_Dataset.zip](https://public.jaeb.org/dataset/577)|[9]|NCT01591681|PSO3|2012|45|15–45|Type 1|42 nights|~1k|Medtronic Enlite|MiniMed Paradigm Veo|
|[PSO1_Public_Dataset.zip](https://public.jaeb.org/dataset/576)|[10]|NCT01736930|PLOS1|2012|20|18–56|Type 1|21 nights|~200|Medtronic Guardian|MiniMed 670G|
|[CTR_Public_Dataset.zip](https://public.jaeb.org/dataset/580)|[11]|NCT01271023|CTR|2011|53|12–65|Type 1|2 days|106|Dexcom SEVEN Plus|Insulet OmniPod|
|[T1DEXIP DOI](https://public.jaeb.org/dataset/590)|[12]|?|T1DexiP|2021|255|14 ± 2|Type 1||10 days|~2.5k|MDI; Omnipod DASH; Tandem t:Slim X2; Medtronic 770G|
|[T1DEXI DOI](https://public.jaeb.org/dataset/589)|[13]|?|T1DEXI|2020|497|37 (18–70)|Type 1|4 weeks|~14k|Dexcom (89%), Medtronic, Abbott|Tandem; Medtronic; MDI|
|[Loop study public dataset 2023-01-31.zip](https://public.jaeb.org/dataset/560)|[14]|NCT03838900|Loop Observational Study|2019|558|1–71|Type 1|6 months|~100k|Dexcom; Medtronic|Medtronic; Insulet Omnipod|
|[DCLP5_Dataset_2022-01-20.zip](https://public.jaeb.org/dataset/535)|[15]|NCT03844789|iDCL Pediatric|2019|101|6–13|Type 1|16 weeks|~11k|Dexcom G6|Tandem t:Slim X2 Control-IQ|

**Dataset Original Publications**    
[1] Lynch J, Kanapka LG, Russell SJ, et al. The Insulin-Only Bionic Pancreas Pivotal Trial Extension Study: A Multi-Center Single-Arm Evaluation of the Insulin-Only Configuration of the Bionic Pancreas in Adults and Youth with Type 1 Diabetes. Diabetes Technol Ther. 2022;24(10):726-736. doi:10.1089/dia.2022.0341  
[2] Hidalgo JI, Alvarado J, Botella M, Aramendi A, Velasco JM, Garnica O. HUPA-UCM diabetes dataset. Data in Brief. 2024;55:110559. doi:10.1016/j.dib.2024.110559  
[3] Anderson SM, Raghinaru D, Pinsker JE, et al. Multinational home use of closed-loop control is safe and effective. Diabetes Care. 2016;39(7):1143-1150. doi:10.2337/dc152468.  
[4] Aleppo G, Ruedy KJ, Riddlesworth TD, et al. REPLACE-BG: a randomized trial comparing continuous glucose monitoring with and without routine blood glucose monitoring in adults with well-controlled type 1 diabetes. Diabetes Care. 2017;40(4):538-545. doi:10.2337/dc16-2482.  
[5] Wadwa RP, Reed ZW, Buckingham BA, et al. Trial of Hybrid Closed-Loop Control in Young Children with Type 1 Diabetes. N Engl J Med. 2023;388(11):991-1001. doi:10.1056/NEJMoa2210834  
[6] Bergenstal RM, Nimri R, Beck RW, et al. A comparison of two hybrid closed-loop systems in adolescents and young adults with type 1 diabetes (FLAIR): a multicentre, randomised, crossover trial. Lancet. 2021;397(10270):208-219. doi:10.1016/S0140-6736(20)32514-9  
[7] Brown SA, Kovatchev BP, Raghinaru D, et al. Six-Month Randomized, Multicenter Trial of Closed-Loop Control in Type 1 Diabetes. N Engl J Med. 2019;381(18):1707-1717. doi:10.1056/NEJMoa1907863  
[8] Buckingham BA, Raghinaru D, Cameron F, et al. Predictive Low-Glucose Insulin Suspension Reduces Duration of Nocturnal Hypoglycemia in Children Without Increasing Ketosis. Diabetes Care. 2015;38(7):1197-1204. doi:10.2337/dc14-3053  
[9] Maahs DM, Calhoun P, Buckingham BA, et al. A randomized trial of a home system to reduce nocturnal hypoglycemia in type 1 diabetes. Diabetes Care. 2014;37(7):1885-1891. doi:10.2337/dc13-2159  
[10] Buckingham BA, Cameron F, Calhoun P, et al. Outpatient safety assessment of an in-home predictive low-glucose suspend system with type 1 diabetes subjects at elevated risk of nocturnal hypoglycemia. Diabetes Technol Ther. 2013;15(8):622-627. doi:10.1089/dia.2013.0040  
[11] Chase HP, Doyle FJ 3rd, Zisser H, et al. Multicenter closed-loop/hybrid meal bolus insulin delivery with type 1 diabetes. Diabetes Technol Ther. 2014;16(10):623-632. doi:10.1089/dia.2014.0050  
[12] Riddell MC, Gal RL, Bergford S, et al. The Acute Effects of Real-World Physical Activity on Glycemia in Adolescents With Type 1 Diabetes: The Type 1 Diabetes Exercise Initiative Pediatric (T1DEXIP) Study. Diabetes Care. 2024;47(1):132-139. doi:10.2337/dc23-1548  
[13] Riddell MC, Li Z, Gal RL, et al. Examining the Acute Glycemic Effects of Different Types of Structured Exercise Sessions in Type 1 Diabetes in a Real-World Setting: The Type 1 Diabetes and Exercise Initiative (T1DEXI). Diabetes Care. 2023;46(4):704-713. doi:10.2337/dc22-1721  
[14] Lum JW, Bailey RJ, Barnes-Lomen V, et al. A Real-World Prospective Study of the Safety and Effectiveness of the Loop Open Source Automated Insulin Delivery System. Diabetes Technol Ther. 2021;23(5):367-375. doi:10.1089/dia.2020.0535  
[15] Breton MD, Kanapka LG, Beck RW, et al. A Randomized Trial of Closed-Loop Control in Children with Type 1 Diabetes. N Engl J Med. 2020;383(9):836-845. doi:10.1056/NEJMoa2004736  
