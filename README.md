# ipl_da_using_sql

# Indian Premier League Cricket Data  Analysis Project using Python and SQL

<p align="center">

## Instructions <br> 
>
<ol>
    <li> Code File name to execute : ipl_cricket_data_analysis.ipynb </li>
    <li> Data is stored in Data folder and Contains database.sqllite in database format. More info about it in Software Intallation Steps.pdf Document</li>
    <li> In order to run the code, please follow below instructions </li>
      <ul>
        <li> Please refer to Software Installation Steps.pdf for instructions on installing software required to run this program</li>
        <li> Step5: Install Git </li>
        <li> Step6: Download the contents from git repo https://github.com/Adikharche19/uberrides_analysis and store it in local folder</li>
        <li> Step7: open terminal/command prompt, naviate to folder location where content was downloaded and type jupyter notebook </li>
        <li> Step8: jupyter notebook will be launched in browser. Select the ipl_cricket_data_analysis.ipynb from folder and open the file </li>
        <li> Step9: Start executing the file by clicking on run button on each cell or go in Kernel option and click on Restart and Run all </li>
        <li> Step10: View the output cell by cell to understand the data flow and insights </li>
      </ul>
</ol>


## Business Problem: <br> 
>
<ul>
    <li> Indian Premier League (Cricket) Data Needs to be analyzed to understand patterns and positioning of matches, utilization of venues etc  </li>    
<ul>

## Dataset:  <br> 
>
> Data is downloaded from below website:  <br> 
> https://www.kaggle.com/code/harsha547/overall-metrics-in-indian-premier-league/input <br> 


## Dataset Metadata/Meaning of each column in data: <br> 
>
<ol>
  <li> <strong> Input Data is in database format with size of 12.82 MB
  </li>
  <li> <strong>Number of years:</strong> 9
  </li>
    <li> <strong>year Name:</strong> 2008, 2009, 2010, 2011, 2012, 2013, 2014, 2015, 2016
  </li>
    <li> <strong>File Data separator:</strong> Data is stored as tables in input file.
  </li>
  <li> <strong>Column Descriptions:</strong> These files are separated by Month and each has the following Columns:
    <ul>
		|	Table Name	|	Number of Rows	|	Number of Columns	|	Table Description	|
		|	:---:	|	:---:	|	:---:	|	:---:	|
		|	Ball_by_Ball	|	136590	|	10	|	Ball by Ball Details	|
		|	Batsman_Scored	|	133097	|	5	|	Runs Scored by Batsman	|
		|	Batting_Style	|	2	|	2	|	Batting Style	|
		|	Bowling_Style	|	14	|	2	|	Bowling Style (Spin, Pace etc)	|
		|	City	|	29	|	3	|	City where Match was conducted	|
		|	Country	|	12	|	2	|	Country where Match was conducted	|
		|	Extra_Runs	|	7469	|	6	|	Extra Runs Conceded	|
		|	Extra_Type	|	5	|	2	|	Type of Exta Run (Wide, No ball etc)	|
		|	Match	|	577	|	13	|	Match Details (Match Id, Match Facts)	|
		|	Out_Type	|	9	|	2	|	Out type of how batchman got out	|
		|	Outcome	|	3	|	2	|	Outcome of the Match	|
		|	Player	|	469	|	6	|	Player Details	|
		|	Player_Match	|	12694	|	4	|	Player of the Match (award)	|
		|	Rolee	|	4	|	2	|	Rolee	|
		|	Season	|	9	|	5	|	Season year	|
		|	Team	|	13	|	2	|	Team name and details	|
		|	Toss_Decision	|	2	|	2	|	Toss Decision (Win, lose)	|
		|	Umpire	|	52	|	3	|	Umpire Details	|
		|	Venue	|	35	|	3	|	Venue Details	|
		|	Wicket_Taken	|	6727	|	7	|	Wickets details	|
		|	Win_By	|	4	|	2	|	Win by (team won by runs or wickets)	|

    </ul>
  </li>
</ol>
        
## Coding Tools:
>
<ol>
  <li><strong>Version Control </strong> - Using Github
  </li>
  <li><strong>Coding Interface </strong> - Jupyter Notebook.
  </li>
  <li><strong> Python Libraries used </strong>- 
    <ul>
      <li><strong>For Data Preparation and Transformation</strong> - Pandas, Numpy, Calendar, sqlite3</li>
      <li><strong>For Data Visualization</strong> - Matplotlib, Seaborn, Plotly</li>
    </ul>
  </li>
</ol>


## Overall Tasks Performed for IPL cricket Data Analysis:
>
<ol>
  <li><strong>Step 1 : Collecting Data</strong>
    <ul>
      <li>Get Data and Metadata from Kaggle for IPL Cricket seasons</li> <br>
    </ul>
  </li>
  <li><strong>Step 2 : Loading Data</strong>
    <ul>
      <li>Load the data from sqlite database into notebok environment for futher transformation.</li> <br>
    </ul>
  </li>
  <li><strong>Step 3 : Cleanse Data</strong>
    <ul>
      <li>Clean the data by identifying and removing duplicates using gruop by queries</li> <br>
    </ul>
  </li>
  <li><strong>Step 4 : Transform Data</strong>
    <ul>
      <li>Add more dervied columns to the data which will be used for grouping and visualization later</li> <br>
    </ul>
  </li>
  <li><strong>Step 5 : Data Grouping and Visualization</strong>
    <ul>
      <li>Group the data by same condition with which visualization needs to be created.</li> <br>
      <li>Visualizations are mentioned in below section.</li>
    </ul>
  </li>
</ol>


## IPL Cricket data Insights Calculated for:
>
<ol>
  <li><strong>Insight 1 : Total number of IPL Matches by Season</strong>
    <ul>
      <li>Determine Number of Matches in each season </li>
      <li>Determine the nature of the trend</li><br>
    </ul>
  </li>
  <li><strong>Insight 2 : Total number of IPL Matches by Venue</strong>
    <ul>
      <li>Determine the Venue with Most and Least matches.</li>
      <li>Determine the nature of the trend</li> <br>
    </ul>
  </li>
  <li><strong>Insight 3 : Total number of IPL Matches Played by a Team</strong>
    <ul>
      <li>Determine teams which play the most matches/ consistet team throughout the seasons </li>
      <li>Determine the team consistency throughout seasons </li> <br>
    </ul>
  </li>
  <li><strong>Insight 4 : Analyze Percentage Factor of Winning a Match If you win the Toss</strong>
    <ul>
      <li>Determine Percentage Factor of Winning a Match If you win the Toss </li>
      <li>Determine the toss contribution in winning </li> <br>
    </ul>
  </li>
  <li><strong>Insight 5 : HeatMap of Number of Matches Played in each City</strong>
    <ul>
      <li>Determine Most and least Busiest Venue to host the matches </li>
      <li>Determine the nature of the trend</li> <br>
    </ul>
  </li>
  <li><strong>Insight 6 : HeatMap of Number of Sixes Hit by a team in each Over</strong>
    <ul>
      <li>Determine overs where most of sixes are hit by each team</li>
      <li>Determine the nature of the trend</li> <br>
    </ul>
  </li>
</ol>



## Results:
> 
<p><strong>Finding 1:</strong></p>
<ol>
    <ul>
      <li>Number of Matches went up from 2009 till 2013 and it went down  </li>
      <li>Reason - eason - Number of teams going up and down impact the number of matches played</li>     
    </ul>         
</ol>

<p><strong>Finding 2:</strong></p>
<ol>
    <ul>
      <li>Chinnaswammy Stadium is most favorite to play more number of matches followed by Eden Garden </li>      
    </ul>              
</ol>


<p><strong>Finding 3:</strong></p>
<ol>
    <ul>
      <li>Mumbai Indians and Royal Challengers are teams which have played most season and most matches  </li>
      <li>Some teams were added only for some seasons and were dropped hence their number of matches are lower</li>  
	</ul>  
</ol>


<p><strong>Finding 4:</strong></p>
<ol>
    <ul>
      <li>Green park, Holkar and OUTsurance Oval are the Venues were team winning the toss has always won the match  </li>      
	</ul>  
</ol>

<p><strong>Finding 5:</strong></p>
<ol>
    <ul>
      <li>2009 season was help outside of India and Durban was more common venue  </li>      
	</ul>  
</ol>

<p><strong>Finding 6:</strong></p>
<ol>
    <ul>
      <li>19th and 20th over is either low or high as teams are trying to score big and may lose wicket  </li>      
	</ul>  
</ol>
