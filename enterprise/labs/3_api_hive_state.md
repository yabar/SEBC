stop
```
[donald@ip-172-31-11-136 yum.repos.d]$ curl -X POST -u admin:admin 'http://ec2-54-169-70-53.ap-southeast-1.compute.amazonaws.com:7180/api/v15/clusters/Yabar/services/hive/commands/stop'
{
  "id" : 122,
  "name" : "Stop",
  "startTime" : "2017-02-17T04:25:14.470Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
```
start
```
[donald@ip-172-31-11-136 yum.repos.d]$ curl -X POST -u admin:admin 'http://ec2-54-169-70-53.ap-southeast-1.compute.amazonaws.com:7180/api/v15/clusters/Yabar/services/hive/commands/start'
{
  "id" : 126,
  "name" : "Start",
  "startTime" : "2017-02-17T04:25:51.932Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
```

