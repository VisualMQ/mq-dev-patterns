
# How to Connect IBM Cloud MQ using JMS 



## Simplify Steps



1.   export path to ccdt.json

     ```shell
     export MQCCDTURL=file:///Users/xyz/Documents/dev/mqsamples/mq-dev-patterns/ccdt.json
     ```

2.   Build sample with Maven

     ```shell
     mvn clean package
     ```

3.   Put messages to MQ

     ```shell
     java -cp target/mq-dev-patterns-0.1.0.jar: com.ibm.mq.samples.jms.JmsPut
     ```

4.   Get message from MQ

     ```shell
     java -cp target/mq-dev-patterns-0.1.0.jar: com.ibm.mq.samples.jms.JmsGet
     ```





## Help



#### How to set up ccdt.json?

1.   Download your Queue Manager connection info in JSON CCDT format.

     ![image-20210812190149480](assets/image-20210812190149480.png)

2.   Rename this to 'ccdt.json' and replace the existing one in current folder.



#### How to set up env.json?

1.   Host and Port: You can find your Queue Manager's Hostname and Port in "Configuration" page.

     <img src="assets/image-20210812190944308.png" alt="image-20210812190944308" style="zoom: 33%;" />

2.   Channel: You can find these inside your ccdt.jsonfile

3.   APP_USER and APP_PASSWORD: the user name and api key of your IBM account

