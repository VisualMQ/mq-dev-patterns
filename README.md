

## How to Connect IBM Cloud MQ using JMS (Simplify Version)



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

