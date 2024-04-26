# Read me

The original idea is from  
https://vivid-wanderer.medium.com/java-profiling-using-visualvm-848a4dd626bc

# Remote debug

JVM args are

```
"-Dcom.sun.management.jmxremote",
"-Dcom.sun.management.jmxremote.ssl=false",
"-Dcom.sun.management.jmxremote.authenticate=false",
"-Dcom.sun.management.jmxremote.local.only=false",
"-Dcom.sun.management.jmxremote.port=1099",
"-Dcom.sun.management.jmxremote.rmi.port=1099",
"-Djava.rmi.server.hostname=127.0.0.1"
```

Run

```
kubectl port-forward pod-test-123 1099 -n test
```