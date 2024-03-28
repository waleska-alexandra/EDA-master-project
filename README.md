
# Basic Exploratory Data Analysis - Master Degree Project

It was a statistics project for my master's degree in finance. The dataset contains information about an NGO, whose objective is to help people with limited resources to access medical examinations, and thus be able to cope with the diseases they may suffer from. 
In total there were 838 observations, covering the months of July, August and September 2023. The data only includes people whose application was approved, but does not include those who were rejected.
The variables are: 
- Mes: Refers to the month.
- Tipo: Refers to the nationality of persons
- Cedula: This is like a DNI
- Solicitante: Refers to the person making the request
- Porcentaje: Refers to the approved percentage
- M_Factura: This is the amount of the invoice
- M_Aportado: This is the approved amount
- Embarazadas: if the woman is pregnant
- M_USD: This is the approved amount in USD$
- Veces atendido: The number of times the patient was seen
- Sexo: Genre
- Hogar: Number of people living in the household
- C_Laboral: Applicant's employment status
- Motivo: reason for the request 
- Causa: cause of application (disease)
- Exámen 1 al 7: what was the test that was done 

Obviously, not all variables are relevant to the final objective of the model. However, since it is an EDA, everything concerning the variables presented to us must be analyzed.


We will need some libraries such as:
empiricaldist,
janitor,
matplotlib.pyplot,
numpy,
pandas,
scipy.stats,
seaborn,
sklearn.metrics,
statsmodels.api.

## Steps

1. Our first step is to check whether or not there are any null values in our data

![image](https://github.com/waleska-alexandra/EDA-master-project/assets/76563412/29bd48b6-e5e9-493c-a390-c5815fbc3de9)


 Variables Exámen 2 to 7 have NAN.

 2. EDA

#### Qualitatives
We check the date
![image](https://github.com/waleska-alexandra/EDA-master-project/assets/76563412/82f25f65-13fc-4473-bd21-b6538f9e3401)


We check the sex variable
![image](https://github.com/waleska-alexandra/EDA-master-project/assets/76563412/d6e545f2-c394-47e3-a5da-a8a6ccd1560c)


We check the variable Embarazada for Woman
![image](https://github.com/waleska-alexandra/EDA-master-project/assets/76563412/414af25d-7fa2-4d64-af07-9615d59e4665)


We check Motivos variable
![image](https://github.com/waleska-alexandra/EDA-master-project/assets/76563412/69325f5f-a416-4c33-8a22-7b04e2c955ae)

We check C_Laboral

![image](https://github.com/waleska-alexandra/EDA-master-project/assets/76563412/cccff42a-dc33-4e68-b3c8-4fac9cdf3cdb)

#### Quantitatives

We make a histogram for the age variable
![image](https://github.com/waleska-alexandra/EDA-master-project/assets/76563412/6c9ad78a-a7f1-469a-b897-2dcafda3ecd2)


We make a boxplot for the M_Factura variable
![image](https://github.com/waleska-alexandra/EDA-master-project/assets/76563412/0fb3ffec-c7f4-45e1-b73f-8d5b04431d6b)
Yes, we can see outliers.

The same thing with M_Aportado
![image](https://github.com/waleska-alexandra/EDA-master-project/assets/76563412/89bd282d-5a0b-4995-accf-77326e21465d)



 3. Tendency Central Measures

Mean, min, IQR and Max
![image](https://github.com/waleska-alexandra/EDA-master-project/assets/76563412/b3c718a8-2149-49b5-93c2-3ee20914b4c3)



 4. Bivariante Analysis
![image](https://github.com/waleska-alexandra/EDA-master-project/assets/76563412/370028d7-0827-404b-9fef-205372dcb46a)


Finally, we ran five multiple linear regression models in which we sought to predict the amount contributed according to certain characteristics. There were 5 models because we selected one for the 20,40,60,80,100 percentile. In this way, we were able to segment the sample and avoid the enormous variability in the amounts. 
That part of the project is in SPSS and Eviews.
The conclusion was that there were variables that the association was NOT taking into account when determining the amount, and they were doing so subjectively. However, there are ranges of people for whom the best possible amount can be predicted. 

![Waleska_Rangel](https://github.com/waleska-alexandra/EDA-master-project/assets/76563412/b1638972-916b-4ac5-9789-42611d8b6c08)
