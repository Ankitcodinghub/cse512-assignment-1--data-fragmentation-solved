# cse512-assignment-1--data-fragmentation-solved
**TO GET THIS SOLUTION VISIT:** [CSE512 Assignment 1- Data Fragmentation Solved](https://www.ankitcodinghub.com/product/cse512-assignment-1-data-fragmentation-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;77454&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE512 Assignment 1- Data Fragmentation Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
The required task is to simulate data partitioning approaches on-top of an open source relational database management system (i.e., PostgreSQL) and build a simplified query processor that access data from the generated partitions. Each student must generate a set of Python functions that load the input data into a relational table, partition the table using different horizontal fragmentation approaches, insert new tuples into the right fragment, and perform query on various fragments.

<strong>Input Data:</strong> The input data is a Movie Rating data set collected from the MovieLens web site (http://movielens.org). The raw data is available in the file ratings.dat.

The rating.dat file contains 10 million ratings and 100,000 tag applications applied to 10,000 movies by 72,000 users. Each line of this file represents one rating of one movie by one user, and has the following format:

<h2>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; UserID::MovieID::Rating::Timestamp</h2>
Ratings are made on a 5-star scale, with half-star increments. Timestamps represent seconds since midnight Coordinated Universal Time (UTC) of January 1, 1970. A sample of the file contents is given below:

1::122::5::838985046

1::185::5::838983525

1::231::5::838983392

<strong>Required Task:</strong>&nbsp; Below are the steps you need to follow to fulfill this assignment requirements:

<ol>
<li>Install PostgreSQL.</li>
<li>Install Python3.x if it is not installed.</li>
<li>Install module psycopg2 for python3.x</li>
<li>Download rating.dat file from the MovieLens website: http://files.grouplens.org/datasets/movielens/ml10m.zip</li>
</ol>
You can use partial data for testing.

<ol start="5">
<li>Implement a Python function loadRatings() that takes a file system path that contains the rating file as input. loadRatings() then load all ratings into a table (saved in PostgreSQL) named ratings that has the following schema</li>
</ol>
<h2>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; userid(int) – movieid(int) – rating(float)</h2>
For your testing, we provide test_data.txt which provides a small fraction of rating.dat file. Be noted that we will use a larger dataset during evaluation. Also note that we don’t load timestamps of ratings.

<ol start="6">
<li>Implement a Python function <em>rangePartition()</em> that takes as input: (1) the Ratings table stored in PostgreSQL and (2) an integer value N; that represents the number of partitions. Then, <em>rangePartition()</em> generates N horizontal fragments of the ratings table and store them in PostgreSQL. The algorithm should partition the ratings table based on N uniform ranges of the rating attribute.</li>
<li>Implement a Python function <em>roundRobinPartition()</em> that takes as input: (1) the ratings table stored in PostgreSQL and (2) an integer value N; that represents the number of partitions. The function then generates N horizontal fragments of the ratings table and stores them in PostgreSQL. The algorithm should partition the ratings table using the round robin partitioning approach (explained in class).</li>
<li>Implement a Python function <em>roundRobinInsert()</em> that takes as input: (1) ratings table stored in PostgreSQL, (2) userid, (3) itemid, (4) rating. Then, <em>roundRobinInsert()</em> inserts a new tuple to the ratings table and the right fragment based on the round robin approach.</li>
<li>Implement a Python function <em>rangeInsert()</em> that takes as input: (1) ratings table stored in PostgreSQL (2) userid, (3) itemid, (4) rating. Then, <em>rangeInsert()</em> inserts a new tuple to the ratings table and the correct fragment (of the partitioned ratings table) based upon the rating value.</li>
<li>Implement a Python function rangeQuery() that takes as input: (1) <em>RatingMinValue </em>(2) <em>RatingMaxValue </em>(3) <em>openconnection (4) outputPath</em>. Please note that the <em>rangeQuery </em>would not use ratings table but it would use the range and round robin partitions of the ratings table. Then,<em> rangeQuery</em>() returns all tuples for which the <em>rating </em>value is larger than or equal to <em>RatingMinValue </em>and less than or equal to <em>RatingMaxValue</em>. The returned tuples should be stored in outputPath. Each line represents a tuple that has the following format such that <em>PartitionName </em>represents the full name of the partition i.e. <em>RangeRatingsPart1 </em>or <em>RoundRobinRatingsPart4 </em> in which this tuple resides. <strong><em>PartitionName</em>, <em>UserID</em>, <em>MovieID</em>, <em>Rating </em></strong>Example:</li>
</ol>
<strong><em>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; range_ratings_part0,1,377,0.5&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; round_robin_ratings_part1,1,377,0.5 </em></strong>

Note: Please use ‘,’ (COMMA, no space character) as delimiter between <em>PartitionName</em>, <em>UserID</em>, <em>MovieID </em>and <em>Rating</em>.

<ol start="10">
<li>Implement a Python function <em>pointQuery </em>that takes as input: (1) <em>RatingValue</em>. (2) <em>openconnection (3) outputPath</em>. Please note that the <em>pointQuery </em>would not use ratings table but it would use the range and round robin partitions of the ratings table. Then, <em>pointQuery</em>() returns all tuples for which the <em>rating </em>value is equal to <em>RatingValue</em>. The returned tuples should be stored in outputPath. Each line represents a tuple that has the following format such that <em>PartitionName </em>represents the full name of the partition i.e. <em>RangeRatingsPart1 </em>or <em>RoundRobinRatingsPart4 </em>etc. in which this tuple resides.</li>
</ol>
<strong><em>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; PartitionName</em></strong><strong>, <em>UserID</em>, <em>MovieID</em>, <em>Rating </em></strong>

Example

<strong><em>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;range_ratings_part3,23,459,3.5&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; round_robin_ratings_part4,31,221,0 </em></strong>

Note: Please use ‘,’ (COMMA, no space character) as delimiter between <em>PartitionName</em>, <em>UserID</em>, <em>MovieID </em>and <em>Rating</em>.

&nbsp;

<strong>Partitioning Questions: </strong>

The number of partitions here refer to the number of tables to be created. For rating values in [0, 0.5, 1, 1.5,

2, 2.5, 3, 3.5, 4, 4.5, 5]

Case N = 1, One table containing all the values.

Case N = 2, Two tables

Partition 0 has values [0,2.5]

Partition 1 has values (2.5,5]

Case N = 3, Three tables

Partition 0 has values [0, 1.67]

Partition 1 has values (1.67, 3.34]

Partition 2 has values (3.34, 5]

Uniform ranges means a region is divided uniformly, I hope the example gives a clear picture.

<strong>Assignment Tips!</strong>

<ul>
<li>Partition numbers start from 0, if there are 3 partitions then <em>range_ratings_part0</em>, <em>range_ratings_part1</em>, <em>range_ratings_part2</em> are partition table names for range partitions and <em>round_robin_ratings_part0</em>, <em>round_robin_ratings_part1</em>, <em>round_robin_ratings_part2</em> are partition table names for round robin partitions.</li>
<li>Do not change partition table names prefix given in tester1.py</li>
<li>Do not hard code input filename.</li>
<li>Please use the same database name, table name, user name and password as provided in the assignment to keep it consistent.</li>
<li>Do not import anything from testHelper1.py and tester1 files. These files are provided only for your testing purpose. If you import anything from these files, your submission will raise error in our test environment which will result in 0 point.</li>
<li>Please make sure to run the provided tester and make sure there is no indentation error in your submission. In case of <strong>any compilation error, 0 marks will be given.</strong></li>
<li>For any case of doubt in the assignment, PLEASE USE Discussion Boards, Individual mails would not be entertained.</li>
<li>The output file should have the exactly same format with the sample. The grading is based on string comparison. One <strong>mismatch </strong>will cause 1 point loss, two mismatch will cause 2 points loss, etc.</li>
<li>Pay attention to the <strong>outputPath</strong>. If you output the result to a different path, the grading script will not be able to locate your file. You will get 0 point.</li>
<li>Do not use global variables in your implementation. Global variable is allowed only for storing two prefixes: RANGE_TABLE_PREFIX and RROBIN_TABLE_PREFIX provided in tester1.py file. You</li>
</ul>
can declare these two global variables in Interface1.py file also. No other global variable is allowed. Metadata table in the database is allowed.

<ul>
<li>You are not allowed to modify the data file on disk.</li>
<li>Two insert functions can be called many times at any time. They are designed for maintaining the tables in the database when insertions happen.</li>
<li>Test cases provided in tester1.py file are for your testing only. We will use more test cases during evaluation. So, think about critical test cases during your implementation.</li>
<li>Use Python 3.x version.</li>
</ul>
