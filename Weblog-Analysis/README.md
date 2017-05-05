access-analysis_2017-05-01_2017_05_02.txt is the result of processing apache weblogs 
provided by WebOps. We requested 48 hours of logs from 2017-05-01 - 2017-05-02. The logs
were concatenated and the following command was run to aggregate and sort by number of occurances.

awk {'print $8'} access_2017-05-01_2017_05_02 | sort | uniq -c | sort -rn > output.txt