# EMDC-ACCIO
EMDC OS GPU-support serverless computing with minimize I/O cost
   
# Daily record
## 22/01/09
### OpenWhisk Container memory extension   
core/invoker/src/main/resources/application.conf:60   
Original maximum container-pool used memory 1GB -> Change to 10GB   
   
common/scala/src/main/resources/application.con:458~460   
container minimum/maximum memory size 128MiB/512MiB -> Change to 128MiB/5120MiB   
   
## Before Create   
### Microbench
Checking code that GPU context sharing between processes   
Only same pid condition can share GPU context   
   
### Container utilization script
Check currently running container's CPU, memory utilization in real-time   
