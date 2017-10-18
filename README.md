# jvm_training
## Useful tools
All examples are for certain pid=65229
Getting a heap dump from command line (and analyze with <b>VisualVM</b> with some useful plugins installed):<br>
```jmap -dump:file=heap.prof 62559 ```<br>
Launching the analysis tool:```jmx```<br>
Heap size:```jinfo -flag MaxHeapSize 62559```<br>
All jvms running on the machine:```jps```<br>
