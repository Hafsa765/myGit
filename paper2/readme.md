# A Manually Curated Method Level Dataset for Test-to-Code Traceability

### Authors 

András Kicsi, László Vidács, Tibor Gyimothy
>Venue: Mon 29 Jun 2020 10:52 - 11:00 at MSR:Zoom2 - Refactoring & Testing **Chair(s): Mauricio Aniche**

[Paper Link](https://2020.msrconf.org/details/msr-2020-Data-showcase/5/TestRoutes-A-Manually-Curated-Method-Level-Dataset-for-Test-to-Code-Traceability "Click to view paper")

**Bold Text**

_Italic Text_

**_Both Together_**

* András Kicsi
* László Vidács
* Tibor Gyimothy

1. András Kicsi
3. László Vidács
3. Tibor Gyimothy

|Col 1|Col 2|
|-----|-----|
|1| Value 1| 
|2| Value 2|
|3| Value 3|
|4| Value 4|

Software testing is one main aspect of software activities wbhich is used to uncover faults that lie within software. A term in ssoftware testing which is considered good practice throughout world is called ecxtensive testing. In software enginnering there's a tem known as traceability wwhich is used for ability of tracing work, having large number of tests, and that problem of tracing test unit under test is called test-to-code trceability. For uncovering tracability link auntomatic extraction methods are necessary.  main advantages of proper traceability information lie in method level identification, which could ease the development and open new doors for bug localization. There is another term TestRoute dataset which includess  220 test cases of trancability links involving more than 2000 manually discovered methods. TestRoute allludes many different methods like Joda-Time’s org.joda.time.TestDateTime_Basics.testIsAfterNow() test that asserts that the org.joda.time.base.AbstractInstant.isAfter Now() method runs properly were displayed. The method includes bollean value e signifying whether the instance it belongs to resembles a date and time in milliseconds after our current date and time. Dataset contain information in java programming language on four open sourc software. Gson supports the serialization and deserialization of Java objects. JFreeChart is the largest of the systems but Joda-Time has the most tests, more than a third of its total methods are tests. Dataset contain four methods of testing process. The test cases are the methods aiming to assess a specific part of the software. Focal methods are use to case  aims to test. Contextual calls and calls made by focal method are mandatory. Helper methods are usedv for setup or modularity purposes. Tests and helper methods are easier to distinguish as helpers usually do not make assertions.

 Dataset contain two types of files 1)Route files   2)Data files. Route files are those files in which traceability links can be found. The first column marks the test case, the second column contains a connected method while the third column describes the nature of the connection, this is either focal, contextual or helper. While, data files are those which contain more information on referenced  methods. In data files first column is the unique identifier of the method while the following columns contain the header, qualified name, starting and ending position of each method in this order.
 
Positions describe the line numbers of the methods in their files. Dataset contains information on four systems, which are   1) Test Method   2) Focal Method   3) Context Method   4)Test Helpers.
The majority of the graph forms a loosely-connected subgraph with only a few isolated test cases. Test friven development and improvement of software system is facilitate by knowledge of real traceability.
It can enable seamless integration between continuous code changes and unit tests, and serve as an important source of system documentation. The dataset is mainly intended for test-to-code traceability research evaluation purposes. It provides more detailed data than the currently available alternatives and can also be used in methodlevel evaluations. Dataset is also suitable for class-level assessment. While the test cases of Commons Lang and Gson represent random tests from the systems, the test cases of Joda-Time and JFreeChart contain random tests that are not covered by naming conventions.
Software testing is one main aspect of software activities wbhich is used to uncover faults that lie within software. A term in ssoftware testing which is considered good practice throughout world is called ecxtensive testing. In software enginnering there's a tem known as traceability wwhich is used for ability of tracing work, having large number of tests, and that problem of tracing test unit under test is called test-to-code trceability. For uncovering tracability link auntomatic extraction methods are necessary.  

Main advantages of proper traceability information lie in method level
 identification, which could ease the development and open new doors for bug localization. There is another term TestRoute dataset which includess  220 test cases of trancability links involving more than 2000 
manually discovered methods. TestRoute allludes many different methods like Joda-Time’s org.joda.time.TestDateTime_Basics.testIsAfterNow() test that asserts that the org.joda.time.base.AbstractInstant.isAfter
Now() method runs properly were displayed. The method includes bollean value e signifying whether the instance it belongs to resembles a date and time in milliseconds after our current date and time. Dataset contain information in java programming language on four open sourc software. Gson supports the serialization and deserialization of Java objects. JFreeChart is the largest of the systems but Joda-Time has 
the most tests, more than a third of its total methods are tests. Dataset contain four methods of testing process. The test cases are the methods aiming to assess a specific part of the software.

Focal methods are use to case  aims to test. Contextual calls and calls made by focal method are mandatory. Helper methods are usedv for setup or modularity purposes. Tests and helper methods are easier to distinguish as helpers usually do not make assertions. Dataset contain two types of files 1)Route files   2)Data files. Route files are those files in which traceability links can be found. The first column marks the test case, the second column contains a connected method while the third column describes the nature of the connection, this is either focal, contextual or helper. While, data files are those which contain more 
 information on referenced  methods. In data files first column is the unique identifier of the method while the following columns contain the header, qualified name, starting and ending position of each method in this order. Positions describe the line numbers of the methods in their files. 
 
 Dataset contains information on four systems, which are  1) Test Method   2) Focal Method   3) Context Method   4)Test Helpers.
The majority of the graph forms a loosely-connected subgraph with only a few isolated test cases. Test friven development and improvement of software system is facilitate by knowledge of real traceability. It can enable seamless integration between continuous code changes and unit tests, and serve as an important source of system documentation. The dataset is mainly intended for test-to-code traceability research evaluation purposes. It provides more detailed data than the currently available alternatives and can also be used in methodlevel evaluations. Dataset is also suitable for class-level assessment. While the test cases of Commons Lang and Gson represent random tests from the systems, the test cases of Joda-Time and JFreeChart contain random tests that are not covered by naming conventions.
Test-to-code traceability provides the target of test cases in the production code. State-of-the-art algorithms are typically evaluatedusing a relatively small number of manually collected links. In addition, only very few of these links are available, which hampersthe comparative evaluation of novel methods.  A manually curated dataset, which contains traceabilitylinks for 220 test cases at method level granularity from4 open-source Java programs were described here. The dataset includes not only the traceability links but also highlights the context of the test and production methods. The whole dataset consists of more than  2000 categorizations of methods that were manually examined. test-to-code traceability links together with their closely related neighborhood. The evaluation of the proposed approaches in test-to-code link recovery is usually accomplished using manually collected links.

Media

http://www.inf.u-szeged.hu/~lac/papers/MSR2020/MSR_2020_Data_Showcase_paper_11.pdf