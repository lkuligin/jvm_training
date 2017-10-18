# jvm_training
## Useful command line tools
All examples are for certain pid=65229
Getting a heap dump from command line (and analyze with <b>VisualVM</b> with some useful plugins installed):
```
jmap -dump:file=heap.prof 62559 
```
Launching Java Mission Control (the analysis tool):
```
jmc
```
Heap size:
```
jinfo -flag MaxHeapSize 62559```
All jvms running on the machine (with flags, etc.):
```
jps
jps -v
```
Starting with a flight recorder (you should pay for it if you use it in production and analyze with JMC):
```
java -XX:+UnlockCommercialFeatures -XX:+FlightRecorder - jar target/...
```
Easy switch between java versions:<br>
```
jenv versions
jenv shell 9
```
