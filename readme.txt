Official Web Link https://www.elastic.co/guide/en/logstash/7.3/configuration.html
Dataset Link  - https://www.kaggle.com/

If you want to index file logstash to mongodb that also you can do that
 
 output {
    mongodb {
        hosts => "localhost:9200"
        index => "african"
        document_type => "african_crises"
    }
    stdout {}
}

stdout we are using to see the output in terminal. While we are indexing the file into elasticsearch or
mongodb or any database.


for running the logstash

bin/logstash -f /Users/Atique/Desktop/Projects/myblog/Youtube/youtube_logstash/logstash-elasticsearch.conf

If you are windows or mac user you can do  
sincedb_path => "NUL"
If you are ubuntu or windows user you can do 
sincedb_path => "/dev/null"
