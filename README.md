# grinnode-progress
 


## Progress Report
 

| Date  | Name | Worked Hours | Work Done | Work Not Done | Problems | Received |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ----------- | 
| 12.11.2020 | stakervali | 2 | I checked example log file and make a quick filtering for target lines. I cloned frontend and backend source code. I will work on python parser for regex and develop a log file generator for testing parser. I also cloned and skim through frontend code | Parser and mobile friendly frontend | I could not start up backend application due to database connection problems. I will leave it as it is now, parser will be tested on synthetic data | Yes |
| 14.11.2020 | stakervali| 5 | I have coded a scraper which extracts collected reorg lines from grinnode.live server. This logs will be used in data generator. I researched on regular expressions and started coding of parser. I will tokenize different parts of the line for date, blockhash etc and extract data| tokenization of reorg line is not finished | ----| Yes |
| 16.11.2020 | stakervali| 5 | I finished line parser which uses regular expressions to extract proper segments of line. I tested parser in scrapped log files and inspected results. It worked without any errors. | I will work on parser for running on different files in the folder structure and write results to database. Also I need to code a sample data generator for testing.  | ----| Yes |
| 18.11.2020 | stakervali  | 3 | I developed table script  for reorg_lines in database and code for inserting parsed line information to database. I researched python libraries for writing script such as parsing command line options and traversing folder structure. Also worked on carrying periodic tasks with python threading | I will work on converting parser to system script and sample data generator | ---- |  Yes | 
| 20.11.2020 | stakervali  | 5| I created a sample data generator script which creates file with desired reorg line ratio in a defined timespan in real time. | I will convert parser into a system script and test it in real-time  | ---- | Yes |
| 24.11.2020 | stakervali  | 4| I have worked on creating a manager which generates files for different nodes using threading.   | I will continue work on converting parser into a system script and testing it in real-time  | ---- | No |
| 25.11.2020 | stakervali  | 5| I have finished sample data manager. It creates a thread for each node and use that thread for creating a log file for a given number of lines and lines per file. | I will work on running parser in directory tree and process each log file.   | ---- | No |
| 26.11.2020 | stakervali | 5 |I created a sample directory with 5 nodes creating log and tested parser. I fixed a bug on parser caused by miliseconds on date strings with regex. I have modified data generator and parser to work on .gz archive files. Also worked on parsing algorithm to avoid possible duplicates on archive and plain files | Finalize and test parser on production | --- | No |
| 27.11.2020| stakervali | 6 | I developed parser to work with infinite loop and parse only modified files. I have tested with sample file generator. | Convert parser to a command-line utility (read database credentials from environment, get parsing options from user ) and test in production| --- | No|
| 30.11.2020| stakervali | 5 | I converted parser and data generator to commandline scripts. | I will convert frontend to mobile friendly material design using vuetify | data generator creates wrong number of reorg lines due to archive and remove file process. | No|
| 1.12.2020| stakervali | 4 | I have forked codebase for grinnode.live frontend. I have import vuetify framework and started from converting header | I will continue on converting header than individual pages to vuetify | ---- | No|
| 3.12.2020| stakervali | 5 | I have studied through vuetify documentation, converted navbar with navigation drawer.| I will continue working on linking vue views with navigation buttons.  | ---- | No|
