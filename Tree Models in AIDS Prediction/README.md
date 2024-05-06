The project uses a real dataset of AIDS patients in 1996, published in Kaggle. The dataset includes 22 independent features and 1 target:
- time: time to failure or censoring
- trt: treatment indicator (0 = ZDV only; 1 = ZDV + ddI, 2 = ZDV + Zal, 3 = ddI only)
- age: age (yrs) at baseline
- wtkg: weight (kg) at baseline
- hemo: hemophilia (0=no, 1=yes)
- homo: homosexual activity (0=no, 1=yes)
- drugs: history of IV drug use (0=no, 1=yes)
- karnof: Karnofsky score (on a scale of 0-100)
- oprior: Non-ZDV antiretroviral therapy pre-175 (0=no, 1=yes)
- z30: ZDV in the 30 days prior to 175 (0=no, 1=yes)
- preanti: days pre-175 anti-retroviral therapy
- race: race (0=White, 1=non-white)
- gender: gender (0=F, 1=M)
- str2: antiretroviral history (0=naive, 1=experienced)
- strat: antiretroviral history stratification (1='Antiretroviral Naive',2='> 1 but <= 52 weeks of prior antiretroviral therapy',3='> 52 weeks)
- symptom: symptomatic indicator (0=asymp, 1=symp)
- treat: treatment indicator (0=ZDV only, 1=others)
- offtrt: indicator of off-trt before 96+/-5 weeks (0=no,1=yes)
- cd40: CD4 at baseline
- cd420: CD4 at 20+/-5 weeks
- cd80: CD8 at baseline
- cd820: CD8 at 20+/-5 weeks
- infected (target): is infected with AIDS (0=No, 1=Yes)

This project evaluates 4 tree models and a voting classifier in AIDS prediction. In conclusion, bagging classifier shows the best performance with nearly 92% accuracy.

Citation :
https://classic.clinicaltrials.gov/ct2/show/NCT00000625
