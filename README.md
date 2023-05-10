# Camunda Server

## Start process

Sample camunda server to show how http connector is working. When it starts it serves 8080 port and manages Camunda cockpit.

To login into Cockpit use:
```
username: demo
password: demo
```

To start sample process go to Task List

![task-list](./2023-05-10_22-34.png)

And then select Start Process

![start-process](./2023-05-10_22-35.png)

Select test-http-connector process

![select-process](./2023-05-10_22-35_1.png)


## Process definition

Project includes sample process (test-http-connector.bpmn) it has a connector task.

![process](./2023-05-10_22-21.png)


## Connector dependencies 

To use a connector you need following dependencies to be included into maven:

```xml
    <dependency>
      <groupId>org.camunda.connect</groupId>
      <artifactId>camunda-connect-core</artifactId>
    </dependency>
    <dependency>
      <groupId>org.camunda.connect</groupId>
      <artifactId>camunda-connect-connectors-all</artifactId>
    </dependency>
    <dependency>
      <groupId>org.camunda.bpm</groupId>
      <artifactId>camunda-engine-plugin-connect</artifactId>
    </dependency>
```

