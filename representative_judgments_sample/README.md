# Representative sample of Indian Court Judgments 
A representative sample of Indian court judgment was created by taking most cited IndianKanoon judgments controlling for court and case type.

Taking most cited judgments from a given court would result in bias in certain types of cases (E.g. criminal cases). Hence it is needed to control for types cases to consider the variety of judgements. So we created following 8 types of cases (tax, criminal ,civil, Motor Vehicles, Land & Property, Industrial & Labour, Constitution, Financial) which are most frequently present. Classification of each judgement into one these 8 types is complex task. We have used naive approach to use act names for assigning a judgment to a case type. E.g. if judgment mentions "tax act" then most probably it belongs to "tax" category. Following are the key act names were used in the Indian Kanoon search queries.  
<!-- This is commented out. 
<center>

| Case Type |  Key Act keywords|
|:--------------:|--------------------------------|
| Tax  |  tax act , excise act, customs act, goods and services act etc. |
| Criminal |  IPC, penal code, criminal procedure etc. |
| Civil |  civil procedure, family courts, marriage act, wakf act etc. |
| Motor Vehicles | motor vehicles act, mv act, imv act etc. |
| Land \& Propery |  land acqusition act, succession act, rent control act etc. |
| Industrial \& Labour |  companies act, industrial disputes act, compensation act etc.|
| Constitution |  constitution |
| Financial | negotiable instruments act, sarfaesi act, foreign exchange regulation act etc.|

  </center> -->

| Domain              | IndianKanoon Query                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| tax                 | tax act ORR excise act ORR customs act ORR abkari act ORR it act ORR income-tax act ORR ke act ORR kvat act ORR tariff act ORR goods and services tax                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| criminal            | IPC ORR penal code ORR criminal procedure ORR dowry ORR narcotics ORR narcotic ORR domestic violence ORR ndps act ORR arms act ORR dp act ORR immoral traffic                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| civil               | civil procedure ORR family courts ORR marriage act ORR wakf act ORR hindu adoption and maintenance act ORR hindu minority and guardianship act                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Motor Vehicles      | motor vehicles act ORR mv act ORR motor vehicle act ORR imv act ORR national highways act ORR motor vehicles taxation act                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| Land & Property     | land acquisition act ORR la act ORR succession act ORR rent control ORR transfer of property act ORR land revenue act ORR land reforms act ORR land reforms (amendment) act ORR rent act ORR eviction of unauthorised occupants ORR ptcl act ORR tenancy and agricultural lands act ORR tp act ORR prohibition of transfer of certain lands ORR land revenue code ORR drc act ORR hindu succession (amendment) act ORR town planning act ORR country planning act ORR mhada act ORR land conservancy act ORR klr act ORR public premises act ORR tenancy act ORR easements act ORR registration act ORR stamp act ORR real estate (regulation and development) act ORR foreign exchange management act ORR right to fair compensation and transparency in land acquisition                                                     |
| Industrial & Labour | industrial disputes act ORR companies act ORR compensation act ORR wages act ORR mines and minerals development and regulation (mmdr) act ORR payment of gratuity act ORR id act ORR pulp act ORR labour practices act ORR industrial dispute act ORR mines and minerals (development and regulation) act ORR industrial areas development act ORR meps act ORR mmrd act ORR information technology act ORR provident funds and miscellaneous provisions act ORR area development act ORR factories act ORR wc act ORR commercial courts act ORR mines and minerals regulation of development act ORR industrial relations act ORR trade unions act ORR maharashtra employees of private schools (condition of service) ORR industrial townships act ORR state insurance act                                                  |
| Constitution        | Constitution                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Financial           | negotiable instruments act ORR ni act ORR sarfaesi act ORR securitisation and reconstruction of financial assets and enforcement of security interest act ORR finance act ORR foreign exchange regulation act ORR bankers book evidence act ORR state bank of india act ORR employees state insurance act ORR conservation of foreign exchange and prevention of smuggling activities act ORR prevention of money laundering act ORR benami transactions ORR securitization and reconstruction of financial assets and enforcement of security interest act ORR banking regulation act ORR recovery of debts due to banks and financial institutions act ORR state financial corporation act ORR interest act ORR chartered accountants act ORR state financial corporations act ORR securities and exchange board of india act |


For each of the court and the case type combination mentioned above, an Indiankanoon query was created with with key words and court filters. Top most cited results from each query was taken. All such results were combined to produce final result. Duplicate judgments obtained in the results were dropped. 
The final distribution of case type and court for duration 1950 to 2017 is as below.

| **Court\_Name**               | **Civil** | **Constitution** | **Criminal** | **Financial** | **Industrial&Labour** | **Land&Property** | **Motorvehicles** | **Tax** | **total** |
| ----------------------------------------- | --------- | ---------------- | ------------ | ------------- | --------------------- | ----------------- | ----------------- | ------- | --------- |
| **Supreme Court of India**                | 200       | 200              | 200          | 200           | 200                   | 200               | 200               | 200     | 1600      |
| **Delhi High Court**                      | 100       | 100              | 100          | 100           | 100                   | 100               | 100               | 100     | 800       |
| **Bombay High Court**                     | 100       | 100              | 100          | 87            | 100                   | 53                | 100               | 100     | 740       |
| **Madras High Court**                     | 100       | 100              | 100          | 35            | 100                   | 100               | 100               | 100     | 735       |
| **Karnataka High Court**                  | 100       | 100              | 100          | 53            | 100                   | 80                | 100               | 99      | 732       |
| **Patna High Court**                      | 100       | 100              | 0            | 116           | 100                   | 111               | 100               | 100     | 727       |
| **Rajasthan High Court**                  | 100       | 100              | 100          | 112           | 58                    | 76                | 71                | 100     | 717       |
| **Madhya Pradesh High Court**             | 96        | 100              | 100          | 77            | 88                    | 91                | 55                | 100     | 707       |
| **Calcutta High Court**                   | 70        | 100              | 79           | 72            | 17                    | 164               | 100               | 100     | 702       |
| **Kerala High Court**                     | 0         | 100              | 100          | 94            | 100                   | 100               | 100               | 100     | 694       |
| **Punjab-Haryana High Court**             | 100       | 100              | 100          | 77            | 53                    | 76                | 83                | 100     | 689       |
| **Gujarat High Court**                    | 79        | 100              | 100          | 98            | 14                    | 86                | 100               | 100     | 677       |
| **Delhi District Court**                  | 100       | 100              | 91           | 98            | 63                    | 100               | 100               | 0       | 652       |
| **Allahabad High Court**                  | 100       | 100              | 100          | 40            | 22                    | 74                | 100               | 100     | 636       |
| **Andhra High Court**                     | 100       | 100              | 100          | 75            | 18                    | 38                | 100               | 86      | 617       |
| **Orissa High Court**                     | 0         | 0                | 0            | 77            | 0                     | 89                | 0                 | 0       | 166       |
| **Income Tax Appellate Tribunal**         | 0         | 0                | 0            | 0             | 0                     | 0                 | 0                 | 80      | 80        |
| **Himachal Pradesh High Court**           | 0         | 0                | 0            | 18            | 0                     | 44                | 0                 | 0       | 62        |
| **Gauhati High Court**                    | 0         | 0                | 0            | 39            | 0                     | 16                | 0                 | 0       | 55        |
| **Bangalore District Court**              | 0         | 0                | 9            | 2             | 37                    | 0                 | 0                 | 0       | 48        |
| **Jharkhand High Court**                  | 0         | 0                | 0            | 24            | 0                     | 18                | 0                 | 0       | 42        |
| **Chattisgarh High Court**                | 0         | 0                | 0            | 16            | 0                     | 16                | 0                 | 0       | 32        |
| **Jammu & Kashmir High Court**            | 0         | 0                | 0            | 15            | 0                     | 16                | 0                 | 0       | 31        |
| **Uttarakhand High Court**                | 0         | 0                | 0            | 7             | 0                     | 13                | 0                 | 0       | 20        |
| **Customs, Excise and Gold Tribunal**     | 0         | 0                | 0            | 0             | 0                     | 0                 | 0                 | 19      | 19        |
| **Sikkim High Court**                     | 0         | 0                | 0            | 9             | 0                     | 6                 | 0                 | 0       | 15        |
| **High Court of Meghalaya**               | 0         | 0                | 0            | 5             | 0                     | 7                 | 0                 | 0       | 12        |
| **Tripura High Court**                    | 0         | 0                | 0            | 0             | 0                     | 2                 | 0                 | 0       | 2         |
| **Custom, Excise & Service Tax Tribunal** | 0         | 0                | 0            | 0             | 0                     | 0                 | 0                 | 1       | 1         |


The data during 1950 to 2017 can be found [here](https://storage.googleapis.com/indianlegalbert/OPEN_SOURCED_FILES/Representative_Judgements_Sample/representative_judgement_sample.csv).