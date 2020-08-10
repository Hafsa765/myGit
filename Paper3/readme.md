#  A Large Collection of Java Test Classes for Test Code Analysis and Processing 

Federico Corò, Roberto Verdecchia, Emilio Cruciani, Breno Miranda, Antoni 

a Bertolino

>Venue: Mon 29 Jun 2020 10:45 - 10:52 at MSR:Zoom2- Refactoring & Testing  **Chair(s): Mauricio Aniche** 

([Paper link](https://2020.msrconf.org/details/msr-2020-Data-showcase/1/JTeC-A-Large-Collection-of-Java-Test-Classes-for-Test-Code-Analysis-and-Processing "Click to view paper")

**Bold Text**_**

_Italic Text_ 


**_Both Together**_

* Federico Corò
* Roberto Verdecchia 
* Emilio Cruciani
* Antonia Bertolino

1. Federico Corò
2. Roberto Verdecchia 
3. Emilio Cruciani
4. Antonia Bertolino

|Col 1| Col 2|
|-----|-----|
|1| Value 1|
|2| Value 2|
|3| Value 3|
|4| Value 4|

Test automation is used to reduce the high costs of software testing and improve product quality. Test code expose different charaacteristics than production code. Hence difference testing is mandatory. It is done to analyze
the quality of test code, propose matrics to access test code quality and try to identify useful patterns for good test code. It demands availability of large dataset of test code, which doesn't yet exist such a collection for ready
usage. Therefore mostly database of open sorce project , for example from github to collect a proper amout of test code are needed. In this context we make available community for test classes dataset that we collected. 
The dataset called JTeC (Java Test Classes) prorepositories vides 2.5M+ classes on which community works on test code analysis and processing can reuse without spending more efforts. For minimizing possi ble threats to
validity associated with use of synthetic tests, we downloaded 500k real test cases from multiplr github projects. The methodology togathers and evaluates results contain six steps:
1: GITHUB  REPOSITORY FILTERING                  2:JAVA REPOSITORY IDENTIFICATION                                 3:TEST CLASSES IDENTIFICATION
4:REPOSITORY SELECTION                                    5:LOCAL STORAGE OF TEST CLASSES                                  6:PRELIMINARY QUALITY FILTERING.

1: GITHUB REPOSITORY FILTERING: It consists of indexing the public github repositries and is carrried out in order to execute efficiently the subsequent phases of our processes. first name of public 
repositories and username of their creaters were retrieved.  Once the list of repository names mapped to username of their creators are obtaned now one can launch second query to the github API in order to 
retrieve the PLs associated with each repository.

2: JAVA REPOSITORY IDENTIFICATION: We parse .csv file to isolate repositories developed exclusively in java by inspecting language tag of indexed repositories and combine their name with username of their
creators to identify the unique URL of repositories.

3:TEST CASE IDENTIFICATION: After isolating the repositories developed in java now we  can identify the test classes of repositories to store them locally. This was done by selecting the source code files of 
selected repositories selecting the source code files of selected repositories whose name ends with "Test.java" and "Tests.java". This step entails the recursive retrieval of files listing of repositories by executing the query via GITHUB API. 
The list of files per repository is parsed in order to identify files matching our specofied naming convention. 
4: REPOSITORY SELECTION: Among the frocks of each original repository the one which contain highest number of test cases were selected. The fork containing the highest numbers of test cases as this option maximizes the efficiency and effectiveness of process were included exclusively.

5:LOCAL STORAGE OF TEST CLASSES: Source code of identified test classes were needed to store. The file system of hierarchy of is preserved while storing test source code.

6:PRELIMINARY QUALTY FILTERING: This is carried out by excluding potential "toy" test suites and entails identifying test suites comprising less than 5 test cases , and subsequently removing such instances from the dataset.

Dataset can be expanded inseveral directions as first step we intend to argument the collection by including test code written in other programming language. Another improvement to compute and provide test related measurements with test classes like code coverage info. 
