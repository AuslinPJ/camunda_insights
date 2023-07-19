### Correlate message from execution using inline javascript

```
execution.getProcessEngineServices().getRuntimeService().createMessageCorrelation("messagename").processInstanceId(execution.getProcessInstanceId()).correlateWithResult();
```
  ![image](https://github.com/AuslinPJ/camunda_insights/assets/31402534/b1107d79-9925-4388-8164-7323f47a0bd3)



### Correlate message from task using inline groovy

```
String taskId = task.getId();
String instance_id = task.getProcessInstanceId();

task.getProcessEngineServices().getRuntimeService().createMessageCorrelation("messagename").processInstanceId(instance_id).correlateWithResult();
```

