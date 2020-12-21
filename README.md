# grinnode-progress
 


## Progress Report
 

| Date  | Name | Worked Hours | Work Done | Work Not Done | Problems | Received |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ----------- | 
| 12.11.2020 | stakervali | 2 | I checked example log file and make a quick filtering for target lines. I cloned frontend and backend source code. I will work on python parser for regex and develop a log file generator for testing parser. I also cloned and skim through frontend code | Parser and mobile friendly frontend | I could not start up backend application due to database connection problems. I will leave it as it is now, parser will be tested on synthetic data | Yes |
| 14.11.2020 | stakervali| 5 | I have coded a scraper which extracts collected reorg lines from grinnode.live server. This logs will be used in data generator. I researched on regular expressions and started coding of parser. I will tokenize different parts of the line for date, blockhash etc and extract data| tokenization of reorg line is not finished | ----| Yes |
| 16.11.2020 | stakervali| 5 | I finished line parser which uses regular expressions to extract proper segments of line. I tested parser in scrapped log files and inspected results. It worked without any errors. | I will work on parser for running on different files in the folder structure and write results to database. Also I need to code a sample data generator for testing.  | ----| Yes |
| 18.11.2020 | stakervali  | 3 | I developed table script  for reorg_lines in database and code for inserting parsed line information to database. I researched python libraries for writing script such as parsing command line options and traversing folder structure. Also worked on carrying periodic tasks with python threading | I will work on converting parser to system script and sample data generator | ---- |  Yes | 
| 20.11.2020 | stakervali  | 5| I created a sample data generator script which creates file with desired reorg line ratio in a defined timespan in real time. | I will convert parser into a system script and test it in real-time  | ---- | Yes |
| 24.11.2020 | stakervali  | 4| I have worked on creating a manager which generates files for different nodes using threading.   | I will continue work on converting parser into a system script and testing it in real-time  | ---- | Yes |
| 25.11.2020 | stakervali  | 5| I have finished sample data manager. It creates a thread for each node and use that thread for creating a log file for a given number of lines and lines per file. | I will work on running parser in directory tree and process each log file.   | ---- | Yes |
| 26.11.2020 | stakervali | 5 |I created a sample directory with 5 nodes creating log and tested parser. I fixed a bug on parser caused by miliseconds on date strings with regex. I have modified data generator and parser to work on .gz archive files. Also worked on parsing algorithm to avoid possible duplicates on archive and plain files | Finalize and test parser on production | --- | Yes |
| 27.11.2020| stakervali | 6 | I developed parser to work with infinite loop and parse only modified files. I have tested with sample file generator. | Convert parser to a command-line utility (read database credentials from environment, get parsing options from user ) and test in production| --- | Yes|
| 30.11.2020| stakervali | 5 | I converted parser and data generator to commandline scripts. | I will convert frontend to mobile friendly material design using vuetify | data generator creates wrong number of reorg lines due to archive and remove file process. | Yes|
| 1.12.2020| stakervali | 4 | I have forked codebase for grinnode.live frontend. I have import vuetify framework and started from converting header | I will continue on converting header than individual pages to vuetify | ---- | Yes |
| 3.12.2020| stakervali | 5 | I have studied through vuetify documentation, converted navbar with navigation drawer.| I will continue working on linking vue views with navigation buttons.  | ---- | Yes |
| 6.12.2020| stakervali | 6| I have converted tutorial pages, Faq pages, contacts, privacy policy and terms of use pages. I worked on typography and design of the pages to make it more readable. I have used collapsable list items for table of contents links | I will convert remaining pages to material design with vuetify and implement countdowns for time and block counts to hardfork-5 | --- | Yes| 
| 7.12.2020| stakervali | 5| I have converted stat and challenge pages. In order to create stat and challenge tables, I had to fetch data in the component otherwise, it did not refreshed at first load | I will implement countdown and some fixing like theme color and scroll links. | Fetching data in component break maybe problematic , I will consult WarmBeer. |Yes|
|8.12.2020| stakervali | 4| I have implemented countdown for remaining block and time to hardfork 5.0. I have fixed theme color | I will make a pull request after merging/replacing code with master branch and  a last overall check | I got cors error while getting remaining block count from api | Yes |
|9.12.2020| stakervali | 3| I have converted globalhealth-check view. I have used a calendar component for scheduled downtimes. Fixed some bugs, converted links, choose theme colours from colormind.io. I have made a pull request | Adding grinaddress checker | ----| Yes|
|10.12.2020| stakervali | 3| I have fixed api status bug, made an anchor for hardfork countdown and fixed other stuff  | Adding grinaddress checker and coingecko api check  | ----|Yes|
|12.12.2020| stakervali| 3| I have worked on accessing coingecko api for health status. I acquired anomaly data and price from exchange via python script. I added price and change data to status bar in frontend. I examined based on davidtavarez's grinaddresschecker repo code to implement in frontend. Could not validate my wallet on his site for testing | I will test and deploy reorg parser to production and add health status from coingecko and grin address checker. |CoinGecko api presents anomaly and trust score per each exchange, some gives green, some gives yellow. Need to decide how to process this data in order to obtain health status. I could not have progress on address checker, need to learn more about owner and foreign api | Yes| 
|19.12.2020| stakervali| 4| I have added random grin art shown in contact page fix a bug on grinnode live page and make updates to news. I explained reorg parser towarmbeer  | I will work on grin health check api  | --- | No| 
|21.12.2020| stakervali |4 | I have examined github repos of  j01tz  and  bladedoyle for nicehash api usage with respect to grin health check. I have created script for accessing parameters such as average_price and speed | I will continue implementing algorithm based on rules gin j01tz grin-health repo. |---- |No |


