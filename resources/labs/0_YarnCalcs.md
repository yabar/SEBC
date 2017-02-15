Assume that there are many data analysts using the cluster. They frequently query small data.
I tried to tune down the container size to increase quantity and support multiple map-reduce applications (query).

```
YARN NM Properties	
yarn.nodemanager.resource.cpu-vcores	16
yarn.nodemanager.resource.memory-mb	114892.8
YARM RM Properties	
yarn.scheduler.minimum-allocation-vcores	1
yarn.scheduler.maximum-allocation-vcores	4
yarn.scheduler.increment-allocation-vcores	1
yarn.scheduler.minimum-allocation-mb	256
yarn.scheduler.maximum-allocation-mb	1024
yarn.scheduler.increment-allocation-mb	256
Task Container Settings	
mapreduce.map.memory.mb	256
mapreduce.map.java.opts.max.heap	800
mapreduce.map.cpu.vcores	1
mapreduce.reduce.memory.mb	1024
mapreduce.reduce.java.opts.max.heap	800
mapreduce.reduce.cpu.vcores	1
```

