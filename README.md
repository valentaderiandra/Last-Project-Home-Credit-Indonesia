# Last Project Home Credit Indonesia


[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)

[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)

[![Ask Me Anything !](https://img.shields.io/badge/Ask%20me-anything-1abc9c.svg)](https://GitHub.com/Naereen/ama)

# Logistic Regression variable Target
by Valent Aderiandra

# Use Case
* **Use Case Summary**


* **Objective Statement** :
    
    * Get business insight about  How Clients distribution group by gender?
    * Get business insight about  the average, maximum and minimum amount issued by the clients?
    * Get business insight about  Target distribution?
    * Get business insight about  Contract Type and Target?
    * Get business insight about  Income Type and Target?
    * Get business insight about  Impact Education Type and Target?
    * Build models Logistic Regresion Model 
    
    
* **Challanges** :
    * Large size of data, can not maintain by excel spreadsheet

* **Methodology / Analytic Technique** :
    * Descriptive analysis
        * Describe the information such as, min/max value of each column, average, and the total count of data contained in grand_total column.
    * Logitstic Regresion


* **Expected Outcome**:

    * Know how Clients distribution group by gender?
    * Know how about the average, maximum and minimum amount issued by the clients?
    * Know how Target distribution?
    * Know Impact Contract Type and Target?
    * Know Impact Income Type and Target?
    * Know Impact Education Type and Target?
    * Know how to build model logistic regression model?

# Business Understanding
* Data loan is static data for all applications. One row represents one loan in our data sample.
- This case has some business question using the data:
    * How Clients distribution group by gender?
    * How about the average, maximum and minimum amount issued by the clients?
    * How Target distribution?
    * Impact Contract Type and Target?
    * Impact Income Type and Target?
    * Impact Education Type and Target?
    * How to build model logistic regression model?

* **Use Case Summary**


* **Objective Statement** :

    * Get business insight about  How Clients distribution group by gender?
    * Get business insight about  the average, maximum and minimum amount issued by the clients?
    * Get business insight about  Target distribution?
    * Get business insight about  Contract Type and Target?
    * Get business insight about  Income Type and Target?
    * Get business insight about  Impact Education Type and Target?
    * Build models Logistic Regresion Model 
    
    
* **Challanges** :
    * Large size of data, can not maintain by excel spreadsheet

* **Methodology / Analytic Technique** :
    * Descriptive analysis
        * Describe the information such as, min/max value of each column, average, and the total count of data contained in grand_total column.
    * Logitstic Regresion


* **Expected Outcome**:
    * Know how Clients distribution group by gender?
    * Know how about the average, maximum and minimum amount issued by the clients?
    * Know how Target distribution?
    * Know Impact Contract Type and Target?
    * Know Impact Income Type and Target?
    * Know Impact Education Type and Target?
    * Know how to build model logistic regression model?


# Business Understanding
* Data loan is static data for all applications. One row represents one loan in our data sample.
- This case has some business question using the data:
    * How Clients distribution group by gender?
    * How about the average, maximum and minimum amount issued by the clients?
    * How Target distribution?
    * Impact Contract Type and Target?
    * Impact Income Type and Target?
    * Impact Education Type and Target?
    * How to build model logistic regression model?


# Data Understanding

* **Source Data**:
    * The dataset used is data from Home Credit Indonesia by Rakamin Academy
    * The raw data contains 307511 rows and 122 columns.

* **Data Dictionary** :
    * SK_ID_CURR	ID of loan in our sample
    * TARGET	Target variable (1 - client with payment difficulties: he/she had late payment more than X days on at least one of the first Y installments of the loan in our sample, 0 - all other cases)
    * CNT_CHILDREN	Number of children the client has
    * AMT_INCOME_TOTAL	Income of the client
    * AMT_CREDIT	Credit amount of the loan
    * FLAG_MOBIL	Did client provide mobile phone (1=YES, 0=NO)
    * FLAG_EMP_PHONE	Did client provide work phone (1=YES, 0=NO)
    * FLAG_WORK_PHONE	Did client provide home phone (1=YES, 0=NO)
    * FLAG_CONT_MOBILE	Was mobile phone reachable (1=YES, 0=NO)
    * FLAG_PHONE	Did client provide home phone (1=YES, 0=NO)
    * FLAG_EMAIL	Did client provide email (1=YES, 0=NO)
    
# Data Preparation

* **Code use** :
    * Python 3.9.12
* **Package** : 
    * Pandas, Numpy, Matplotlib, Seaborn, Scipy, Sklearn, and Warning 
    
# Data Cleansing

the data is clean **because there are no missing values and the data types are appropriate** so **no need for data cleansing**

# Exploratory Data Analysis

In statistics, exploratory data analysis is the approach of analyzing a data set to summarize its main characteristics, often using statistical charts and other data visualization methods

* **Describe Data**

![Describe](https://user-images.githubusercontent.com/97577380/205304960-ad562c2a-65b1-49a6-a47c-949ab3726969.png)

Dari analisis deskriptif diatas,Jumlah baris data yang dimiliki sebanyak **8602** baris dan *dapat diasumsikan bahwa 75% customer kita tidak memiliki gagal bayar*.Dari data yang kita miliki,jumlah anak terbanyak sejumlah **5 anak**.Rata-rata pendapatan client kita sejumlah **222872.41** dengan pendapatan terbesar sejumlah **4500000** dan terkecil sejumlah **33750**.Rata-rata jumlah kredit yang dipinjam nasabah berjumlah **699998.70** dengan nilai terbesar dipinjam **4050000.00** dan terkecil sejumlah **45000**.Client dengan gaji dibawah 270000,diasumsikan meminjam tertinggi sejumlah 958144.50.

* **Clients distribution group by gender**

![Clients distribution group by gender](https://user-images.githubusercontent.com/97577380/205304932-3158daaf-68cb-4d58-a714-c2b4b7e12336.png)

Perbandingan jumlah clients dengan gender wanita dengan laki-laki hampir sama,sebanyak 50,93 % clisent kita berjenis kelamin laki-laki dan sebanyak 49.07% client kita berjenis kelamin wanita*

* **Target Distribution**

![Target Distribution](https://user-images.githubusercontent.com/97577380/205304971-4cdb792a-7a71-4107-a094-550032599cb2.png)

Berdasarkan grafik diatas,dapat diasumsikan bahwa 6,11 % clients kita memiliki payment difficulties

* **Contract Type and Target**

![Contract Type and Target](https://user-images.githubusercontent.com/97577380/205304943-3f813b00-2637-489f-89b3-749e753dbe94.png)

Berdasarkan grafik diatas,dapat diasumsikan jenis contract yang paling diminati oleh client yaitu Cash loans.Jenis kontrak Revolving Loans yang memiliki peluang gagal bayar yang rendah 

* **Target vs Income Type**

![Target vs Income Type](https://user-images.githubusercontent.com/97577380/205304974-1feba30c-5f83-48db-bfa7-26ed4a9c7433.png)

Berdasarkan grafik diatas,dapat diasumsikan bahwa customer kita kebanyakan mendapatkan income dari bekerja (working) 

* **Education VS Target**

![Education VS Target](https://user-images.githubusercontent.com/97577380/205304963-e38626c3-7ddb-4a5e-929c-f2f8c1a7fbee.png)

Dari grafik diatas,dapat disimpulkan bahwa clients dengan kasus payment difficulties terbanyak ada di education Secondary / secondary special,setelah itu di urutan kedua adalah Higher education.Namun,hal ini dipengaruhi dengan jumlah clients terbesar ada di level educaiton Secondary / secondary special dan Higher education.Pada level Secondary / secondary special perbandingan antara clients dengan payment difficulties dan clientst non payment difficulties kurang lebih 1:10

* **Correlation **

![Corelation](https://user-images.githubusercontent.com/97577380/205304954-94f9acc2-dd2e-4d99-bb0c-0a42fb4c64f0.png)
