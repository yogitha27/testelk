# testelk
#for installing elastic search commands
wget -qO - https://artifacts.elastic.co/GPG-KEY-elasticsearch 
 sudo apt-key add
 sudo apt-get install apt-transport -https 
echo "deb https://artifacts.elastic.co/packages/7.x/apt stable main"
sudo apt-get update && sudo apt-get install elasticsearch
sudo service elasticsearch start
#for installing kibana
sudo apt-get install kibana
sudo service kibana start
#for installing logstash
sudo apt-get install logstash
sudo /etc/logstash/conf.d/apache.conf
#for installing kafaka
sudo apt-get install zookeeperd
wget http://apache.mivzakim.net/kafka/2.2.0/kafka_2.12-2.2.0.tgz
tar -xvzf kafka_2.12-2.2.0.tgz
sudo cp -r kafka_2.12-2.2.0 /opt/kafka
#for installing filebeat
sudo apt-get install filebeat
#to open filebeat configuration
/etc/filebeat/filebeat.yml
#to start data pipeline
sudo service filebeat start
sudo service logstash start
/opt/kafka/bin/kafka-console-consumer.sh --bootstrap-server 
to create a pipeline
sudo  /etc/logstash/conf.d/apache-daily-access-log




