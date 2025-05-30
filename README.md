# Analýza odchodovosti zákazníkov v telekomunikáciách

## Popis projektu  
Tento projekt bol realizovaný ako súčasť bakalárskej práce so zameraním na dátovú analytiku. Cieľom bolo analyzovať správanie zákazníkov v oblasti telekomunikácií a klasifikovať pravdepodobnosť ich odchodu (churn), čo je kľúčové pre znižovanie finančných strát podnikov.

### Dataset
V tejto práci sme používali dataset dostupný na tomto linku: https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data?select=WA_Fn-UseC_-Telco-Customer-Churn.csv.

### Abstrakt práce
V tejto práci sme riešili odchodovosť zákazníkov v telekomunikáciach. Zamerali sme sa na túto problematiku, keďže spôsobuje finančné straty podnikom, a preto je dobré vedieť analyzovať správanie zákazníkov. Cieľom práce bolo klasifikovať, ktorí zákazníci s vyššou pravdepodobnosťou zrušia svoje služby, a identifikovať kľúčové faktory, ktoré tento odchod ovplyvňujú. Pri tejto práci sme postupovali metodológiou CRISP-DM, ktorá je veľmi populárna pri objavovaní znalostí v databázach. Pri práci sme postupovali pochopením dát a ich predspracovaním na modelovanie. Vybrali sme si modely na ktorých sme klasifikovali odchodovosť zákazníkov, a to konkrétne CatBoost, Náhodné lesy, Rozhodovací strom, Logistická regresia a XGBoost. Skúšali sme rôzne metódy vyberania atribútov na modelovanie a rovnako sme použili aj vylepšenia modelov, konkrétne nadvzorkovania a ENN. Po aplikovaní vylepšení, modely nedosahovali najvyššie výsledky, ale odrážali skutočnosť a poukázali, že je náročné odhadnúť správanie každého zákazníka. Z týchto modelov najlepšiu úspešnosť preukazoval model Logistickej regresie, kde to bolo 80,7% a presnosť 68%. Po použití nadvzorkovania sa úspešnosť a návratnosť znížili pri každom modely. Najväčšiu úspešnosť mal CatBoost 75,4% a najlepšiu návratnosť mala Logistická regresia s hodnotou 86%.  Následne sme si porovnali jednotlivé AUC hodnoty kde najlepšie obstali modely CatBoost a Logistická regresia s hodnotou 85%. Medzi najvýznamnejšie atribúty ovplyvňujúce odchod zákazníkov patrili dĺžka zmluvy, spôsob platby a využívanie internetových služieb. Výsledky práce môžu pomôcť telekomunikačným spoločnostiam lepšie riadiť vzťahy so zákazníkmi vďaka využitiu analytických a klasifikačných nástrojov.
### Použité modely

 -  Logistická regresia
    
-   Rozhodovací strom
    
-   Náhodné lesy 
    
-   CatBoost
    
-   XGBoost
    

Na vyrovnanie dátovej nerovnováhy boli použité:

-   Nadzvorkovanie (Random Oversampling)
    
-   ENN (Edited Nearest Neighbours)

### Obsah repozitára

 - bp_data.ipynb -> zdrojový kód v jazyku python s pochopením dát, prípravou dát a modelovaním
 - WA_Fn-UseC_-Telco-Customer-Churn.csv -> dataset
 - README.md
 - catboost_info -> vypis modelu
### Požiadavky
Dáta boli spracované v prostredí Visual Studio Code. Notebook je uložený vo formáte `.ipynb`. Je možné ho otvoriť vo Visual Studio Code ale s rozšírením Python a jupyter notebook, alebo priamo cez Jupyter notebook.
Potrebné knižnice a verzie:
 - catboost 1.2.8
 -  imbalanced_learn 0.13.0
 -  matplotlib 3.10.3
 -  numpy 2.2.6
 - pandas 2.2.3
 -  scikit_learn 1.6.1
 -  scipy 1.15.3
 -  seaborn 0.13.2
 -  xgboost 1.7.6
 -  Python 3.13.2
 ### Inštalácia knižníc
 Projekt bol vytvorený v Python 3.13.2. 
 Všetky potrebné knižnice si viete nainštalovať týmto príkazom:

    pip install catboost==1.2.8 imbalanced_learn==0.13.0 matplotlib==3.10.3 numpy==2.2.6 pandas==2.2.3 scikit_learn==1.6.1 scipy==1.15.3 seaborn==0.13.2 xgboost==1.7.6
    
#### František Vaľko
