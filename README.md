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
|19.12.2020| stakervali| 4| I have added random grin art shown in contact page fix a bug on grinnode live page and make updates to news. I explained reorg parser towarmbeer  | I will work on grin health check api  | --- | Yes | 
|21.12.2020| stakervali |4 | I have examined github repos of  j01tz  and  bladedoyle for nicehash api usage with respect to grin health check. I have created script for accessing parameters such as average_price and speed | I will continue implementing algorithm based on rules gin j01tz grin-health repo. |---- | Yes |
|1.01.2021| stakervali |9 | I have created bug-challenge page. I have converted topbar from tab view to normal view. I converted challenges to submenu as decided | I will continue implementing algorithm based on rules gin j01tz grin-health repo. | Challenges item in topbar is not highlighted when navigated. Also I have not be able to convert challenges to submenu in sidebar navigation drawer despite trying. The icon placement was problematic.    | Yes |
|14.01.2021| stakervali | 2 | I have added a new FAQ item, added new art from grinsun to contact page and recalibrated countdown timer to remaining block count| I will update the news section and implement other changes requested by @MCM-Mike | ---- | Yes |
|15.01.2021| stakervali | 3 | I have found out that countdown timer shows different values depending on client timerzone. I have changed code so that in every 30 seconds, countdown is readjusted to remaining block count. I have updated news section. Added blockheight to stats page and removed API V1 links from tutorials section| I will work on implementing algorithm based on rules in j01tz grin-health repo. | ---- | Yes |
|22.01.2021| stakervali | 4 | I have developed nicehash score calculation by querying coingecko, grinmint and nicehash apis. calculation algorithm is based on @joltz repo. I tested script and validated that results are same with https://joltz.keybase.pub/api/grin | I will implement script for reorg score calculation | ---- | Yes |
|23.01.2021 | stakervali | 4 | I have fixed a bug in reorg_parser. I have implemented reorg_score calculation based on @joltz repo | I will store results of nicehash and reorg score  into database with a new table| ---| Yes |
|24.01.2021 | stakervali | 4 | I have created sql script for health_score table in db. I have developed health_check script as command line utilty. I have updated readme.md with health_check section. | Deployment of scripts to production. Addition of Geomap for grinnodes in frontend | ---- | Yes |
|31.01.2021 | stakervali | 1 | I have added health, nicehash and reorg score ro statistics page. I fetch joltz API but got CORS error due to missing 'access-control-allow-origin' header. | I will  fetch nicehash and grinming api from client for nicehash calculation. | I could not fetch joltz's API as planned | Yes |
|1.01.2021| stakervali | 2| I have implemented nicehash calculation logic in vue-frontend. | Nicehash api calls must be done from backend. I will test it after python script's deployment. | Nicehash api does not add Cross Origin and returns 403 response. I have tried crossorigin.me to proxy api call and it failed with 403 response too. | Yes|
|12.02.2021| stakervali| 3| I have examined summary logs and extract depth count and deepest branch values for calculation of reorg score. I did some explatory data analysis | I will work on grinnode-backend for parser integration | ---| Yes|
|14.02.2021| stakervali| 6| I have worked on accessing Wallet API to check donation wallet of grinnode.live. Based on bladedoyle's help we checked wallet via curl command. | I will work on adding wallet health-check feature on backend. |--- | Yes|
|16.02.2021| stakervali| 3| I have cloned backend api code on my local computer and setup. Mainly I tried to overcome an authorization problem in sql connection. I have managed to run application | I will get familiar on code and integrate health score query to API | --- | Yes |
|17.02.2021| stakervali| 5 | I have studied existing code and application logic. I have added healthscore as a route and add sql query to api_controller and cache sections. I have setup health_check and parser setup script to feed database and query database on backend api controller and ran succesfully. I have fixed some bugs on health_checker script. | I will look into  healthscore last updatetime issue. I will deploy backend to a remote server for testing and adding donation-wallet health check.| Backend api reports healthscore check time shifted-incorrectly. python script saves time to database in utc timezone.Backend converts it to wrong timezone  | Yes |
|23.02.2021| stakervali| 5 | I have converted logging dates for reorg parser and health checker to utc timestamps (integer) in database. I have converted python scripts and queries in backend accordingly. I have setup a test server and deployed both python scripts and backend. |  I will work on donation wallet check in backend | --- | Yes |
|24.02.2021| stakervali| 6 | Test server crashed due to cpu spike, I have fixed it wrapping main script function with a daemon thread. I have added pid logging for following/killing script process. I have implementd donation-wallet-health check in backend api and deployed to test server. |  I will work on presentation of health check in frontend and continue testing the script. | --- | Yes |
|26.02.2021| stakervali| 6| I have removed verbose print statement and implement logging in parser, sample-generator and health-checker scripts. I have added max_depth option to sample generator for better testing. I have switch back to normal threads from daemon and fixed time issue by removing file-time argument. I have searched for a charting library with small size and decided to use flot library. I have start working on frontend for consuming and presentation of health-score endpoint | I will continue working on frontend and testing | --- | Yes | 
|1.03.2021| stakervali| 8| I have worked on integration of health-score to frontend. I converted date to more human readable format. Added health check to vue-$dao which  queries test-server like other api endpoints. I have discarded flot because of jquery dependence. I have integrated chartist.js, I have added option to interactively plot reorg, nicehash and overall health scores. | I will work on testing frontend. I will work on tor address check to faq page, existing links are not working. | --- | Yes |
|2.03.2021| stakervali| 5 | I have added custom wallet check as an endpoint to API and deployed to test-server. I have added an input form in the frontend stat page for checking validity of wallet via this endpoint. I have done some research for world map visualization of grinnode count per country. I have found that d3.js is simplest approach. I have checked script logs in the test-server.| I will complete world map visualization of nodes and clean up code for deployment. | ---- | Yes |
|5.03.2021|stakervali|9 | I have added world map visualization of nodes to frontend. I have first tried to use d3.js library, then switched to d3plus.js which is a higher level. I have created an endpoint in the backend for converting ips to country locations. I have added a library to backend for conversion of ip to loc. I have created a utility method for converting 2-letter iso codes to 3-letter in frontend. | I will clean up code and commit to github repo. | I have some questions about sql query of recent ips. I have consulted to WarmBeer | Yes |  
|10.03.2021| stakervali| 2 |I have added an endpoint for ip locations via querying grin node API based on our discussions with @Warm Beer| I will clean up code and commit to github repo|----| No | 
|14.03.2021| stakervali| 8 | I have removed chartist library due to deprecated dependency issues and used d3plus chart library (which I used for ip geomap) I worked customization of bar chart for displaying score. I have added a description text for score section. I have made a small change in API to reduce overall health score into 0-5 range. I have added a radio group for switching score charts. Chart works with hardcoded sample data  | I will finalize charting section | There is a bug when I try to refresh chart with fetched data from backend API that needs to be fixed | No|
|15.03.2021| stakervali| 5 | I have setup nginx with backend and frontend in the server. In tor address check wasnot working when user add .onion to end, I have fixed that. I reorg parser script failed 5 days ago because of failed database connection (after working 14 days). I have made changes to remedy it. CPU spikes every 30 minutes due to mysql process.   | I will continue on testing... |  tor address check stucks if one checks one address after another, I will fix it | No |
|16.03.2021| stakervali| 6| I have fixed tor address check. When ordinary urls entered, wallet check stucked, fixed. Adjusted frontend due to changes in API for health score endpoint. Fixed some alignment issues, edited chart ppadding for better view in mobile. Edited health text description. I tested cpu usage without scripts running and also tested with current master branch in order to find out if the additions I made in backend caused it. It seems the present codebase also creates spikes due to low spec of test server. I fixed a bug in reorg_parser causing wrong log_date storage. | I will comment and clean code to get ready for deployment. I will finish the adjustments/additions MCMMike asked | --- | No | 
|18.03.2021| stakervali|5| I have switched geolite2 package. Cleaned and commited backend code to world_map branch on github repo. I have switched codebase to test-server| I will finish deployment related work and write an article about new features | --- | No|
|19.03.2021| stakervali|3  | I have made modifications with new installed ip location package. I have caught a problem with wallet address check. Added license requirement to world map, fixed alignment issues in tutorial section, added new api points to faq page | I will continue working on deployment| --- | No | 
