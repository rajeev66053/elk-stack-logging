# elk-stack-logging-example
How to perform centralize logging in microservice architecture using ELK Stack

###### Download ELK Binary Distrubution

###### 1.Download Elastic Search [Download]( https://www.elastic.co/downloads/elasticsearch)
###### 2.Downl;oad Logstash [Download](https://www.elastic.co/downloads/logstash/)
###### 3.Download Kibana [Download](https://www.elastic.co/downloads/kibana/)

###### Configure Kibana

###### Open config/kibana.yml in an editor. D:\kibana-7.16.2-windows-x86_64\config\kibana.yml
###### Uncomment elasticsearch.hosts to point at your Elasticsearch instance.

###### Run elasticsearch.bat file from D:\elasticsearch-7.16.2\bin
###### elasticsearch.bat

###### Run kibana.bat file from D:\kibana-7.16.2-windows-x86_64\bin
###### kibana.bat

###### Have to create a logstash.conf file. Link your log file in logstash.conf, Then paste the conf file in logstash bin folder D:\logstash-7.16.2\bin

###### Now run the cmd from D:\logstash-7.16.2\bin path
###### logstash -f logstash.conf 

###### Then the log will be display in logstash console.


###### Go to url to see logstash file name
###### http://localhost:9200/_cat/indices
###### http://localhost:9200/logstash-2021.12.30-000001/_search

###### Run elastic search in 
###### http://localhost:9200/

###### Run kibana in port 5601
###### http://localhost:5601/