Correlate message from execution using inline javascript

execution.getProcessEngineServices().getRuntimeService().createMessageCorrelation("messagename").processInstanceId(execution.getProcessInstanceId()).correlateWithResult();
