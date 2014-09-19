ciotc
=====
In the version ,the Exception Detector plays a central role in the job control. Firstly, it checks statuses of the servers in the cluster  ,that is ,whether they are in working, If not availble , it will reqeust the system to reboot the servers and then restart all the hadoop services. After that, it checks whether the hadoop services are working by the pids and service name. Finally ,it checks whether the services are in a regular status and if there are error-lvel records in service logs ,the jobDaemon service will be stopped. 
