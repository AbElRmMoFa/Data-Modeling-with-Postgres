<h1>Data Modeling with Postgres</h1>
<p>build a database for Sparkify  startup</p>
<p>We, as a team, have been hired by Sparkify, a startup music streaming app, to analyze the data they've been collecting on songs and user activity. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.</p>

<p>Our role is to create a Postgres database with tables designed to optimize queries on song play analysis. We will create a database schema and ETL pipeline for this analysis.</p>

<h2>Schema for Song Play Analysis</h2>
<p>Using the song and log datasets, we will create a star schema optimized for queries on song play analysis. This includes the following tables.</p>

<h3>Fact Table</h3>
<p>songplays - records in log data associated with song plays i.e. records with page NextSong</p>
<ul>
    <li>songplay_id</li>
    <li>start_time</li>
    <li>user_id</li>
    <li>level</li>
    <li>song_id</li>
    <li>artist_id</li>
    <li>session_id</li>
    <li>location</li>
    <li>user_agent</li>
</ul>

<h3>Dimension Tables</h3>
<ul>
    <li>users - users in the app</li>
    <ul>
        <li>user_id</li>
        <li>first_name</li>
        <li>last_name</li>
        <li>gender</li>
        <li>level</li>
    </ul>
    <li>songs - songs in music database</li>
    <ul>
        <li>song_id</li>
        <li>title</li>
        <li>artist_id</li>
        <li>year</li>
        <li>duration</li>
    </ul>
    <li>artists - artists in music database</li>
    <ul>
        <li>artist_id</li>
        <li>name</li>
        <li>location</li>
        <li>latitude</li>
        <li>longitude</li>
    </ul>
    <li>time - timestamps of records in songplays broken down into specific units</li>
    <ul>
        <li>start_time</li>
        <li>hour</li>
        <li>day</li>
        <li>week</li>
        <li>month</li>
        <li>year</li>
        <li>weekday</li>
    </ul>
</ul>
<h2>Techniques and Technologies </h2>
<ul>
  <li><strong>Data Modeling:</strong> A star schema is used for optimizing queries on song play analysis.</li>
  <li><strong>PostgreSQL:</strong> A relational database management system is used to store the data.</li>
  <li><strong>Python:</strong> The ETL pipeline and database creation scripts are written in Python.</li>
  <li><strong>ETL (Extract, Transform, Load):</strong> The ETL process is used to extract the data from the JSON files, transform it into a format that fits the database schema, and load it into the PostgreSQL database.</li>
  <li><strong>Pandas:</strong> A Python library is used to manipulate and clean data before inserting it into the database.</li>
  <li><strong>Jupyter Notebook:</strong> A web-based interactive computing environment is used to develop and test the code in an iterative manner.</li>
  <li><strong>Git:</strong> A version control system is used to manage and track changes to the codebase.</li>
</ul>
