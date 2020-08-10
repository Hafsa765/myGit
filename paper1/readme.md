# LogChunks: A Data Set for Build Log Analysis

## Authors

Carolin Brandt, Annibale Panichella, Andy Zaidman, Moritz Beller

>Venue:  Mon 29 Jun 2020 11:48 - 12:00 at MSR:Zoom - Quality "_Chair(s): Raula Gaikovina Kula_"

[Paper Link](https://2020.msrconf.org/details/msr-2020-Data-showcase/2/LogChunks-A-Data-Set-for-Build-Log-Analysis "Click to view paper")

[Pdf Link](https://pure.tudelft.nl/portal/files/71450840/paper.pdf)


## **Bold Text**

## _Italic Text_

**_Both Together_**

+ Carolin Brandt
+ Annibale Panichells
+ Andy Zaidman
+ Moritz Beller

1. Carolin Brandt
2. Annibale Panichells
3. Andy Zaidman
4. Moritz Beller

|Col 1| Col 2|
|-----|-----|
|1| Value 1|
|2| Value 2|
|3| Value 3|
|4| Value 4|

In software engineering continuous integration (CI) has become a very common practice. CI buils are used to report resultss of various  substeps within build and it's used in many software processes to detect bugs early, devoleper productivity's improvance and communcication.
Size of build log can be excess of 50 Mb of ASCII text and it can be verbose to make them indequate for direct human consumption.  For suppporting developers and reasearchers in infdormation build logs 
we should retrieve chunks of logs that describe information which is targeted. There are many mrthods for retrieving of chunks like BELLER ET ALanalyze logs from tarvis by using rule-based system of  expression and those expressions are developed through exemplary build log's vision. An other way of chunking is VASSALLO ET AL which build repair hints to wrote a custom parser to gather information. These approaches consists some strengths as well as weeekneses likeregular expressions are exact but tedious 
to maintin, or  custom parser are powerful though fragile in lighting changes in structure of log.
LOG CHUNK ia actually collection of 797 labeled Travis CI build logs from 80 highly popular GitHub repositories in 29 programming languages with manually labeled chunk describing why the build failed. 

                                                            Methods for gathering logs and mannual labeling processing:
1:= LOG COLLECTION: Log creation contain Repository samplin, build sampling and log sampling.
     =>Repository sampling:- For log chunks GH Torent were queried from three most popular repositories to cover broad range of development lnguages from each of 30 propular languages from which repository 
languages are like Microsoft/TypeScrip, git/git.
   =>Build Sampling:- To sample builds for logchunksten most recent builds of status were kept. 1000  builds per repostory were checked to ensure predictable termination of log collection.
   =>Log Sampling:- Three repositories collected build logs and discarded logs were inspected. 

2:= Manual Labeling:- After collection firstb aunthor dwescribed why the build failed by manual labeling and assigned keywords and structural categories to each log chunk. 
   => Chunk That Describes Why The Build Failed:- The authoirb preserved whitespaces and special characters to detect the targeted substring and copied out first occurence about the failure of build for 
each repository. 

   => Search Keyboard: To extract the search word ten lines above and below and chunk were considered and labeler's task was to find description failure by noting down three strings they would search for  ("grep"). There were no limitatiuon made on strings.

   => Structural Category:- For labeling the structural categories chunk and sorrounding were presented from a repository to labeler for all logs.
  3:= Validation:> Collected data points were validated in an iterative fashion.

                                                                                                RELATED DATASET AND HOW LOGCHUNKS ARE DIFFER FROM THEM:

 Travis Torrent:- It collects wide range about Travis CI build log's data about data and combines data which is accessible by GitHub APIs and GHTorrent. TravisTorrent obtaned by developer parser 
which only supports Java Marvin or Junit logs whereas LogChunk provides why build failed from manually labeled an two-fold-cross-validated data for all possible build failing errors.
  
LogHub:- It is collection of broad range of system log data set. It is basis that compare different approaches into structured data for further analysis. Logchunks is situated in different area which tend 
to be semi-structured.

      CURRENT LIMITATION AND FUTURE IMPROVEMENTS
      OF LOGCHUNKS

   Chunks As One Consecutive Substring:- Multiple substring of log text were proposed to extend LogChunks and chunk contain only one continuous substring of log text. Reason of build failure could be described at multiple location witjhin log text.

   Include More Repositories And Logs:- Extension of more repositories and logs will strengthen logchunks as the go to benchmark.
    Classification Of Build Failure Cause:- The data set contain no further classification such as due to test, compilation or linter errors.
    Other Information Chunks:- LogChunks can be extended with labels contained in build log like build infrastructure and more.
    Validation Of Search Keywords:- Keywords logchunks provides are baased on experience of authors gained from analyzing around 800 build logs.

LOGCHUNKS adavances the research field of build log analysis by introducing a benchmark to examine research contribution and opening various research possibilities that previously required tedious manual
classification.