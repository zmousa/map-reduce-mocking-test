MapReduce Test using Mocking
============================
There are multiple libraries that helps developers unit test Apache Hadoop map reduce jobs, in this project we applied:
    * MRUnit: this library had been retired (from apache), since it's functionalties included in the normal mocking libraries.
    * Mockito: used even in normal unit testing, and capable for mocking the hadoop context.

Project Source
--------------
Contains:
    * `WordCountMapper.java`: simple hadoop map
    * `WordCountReducer.java`: simple hadoop reduce
    * `WordCountMapperTest.java`: Mockito test for map
    * `WordCountReducerTest.java`: Mockito test for reduce
    * `WordCountMRUnitTest.java`: MRUnit test for the job
    
Notice
------
The hadoop library in this project is too old because of the MRUnit compatibility.

References
----------
    * [MR Test with Mockito blog](https://caffebig.wordpress.com/2012/10/16/unit-testing-hadoop-map-reduce-jobs/)
    * [MRUnit tutorial](https://cwiki.apache.org/confluence/display/MRUNIT/MRUnit+Tutorial)

Run Tests
---------
mvn test