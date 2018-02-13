# CGroup Commands
  * Start CGroup by executing ``` service cgconfig start ``` if this command throws error then follow the upcomming steps.
  * Create the corresponding directory using mkdir.
    * ``` mkdir /cgroup/memory ```
  * Mount the directory using mount command.
    * ``` mount -t cgroup -o memory memory /cgroup/memory ```
  * list the files to see the memory control bindings.
    * ``` ls /cgroup/memory ```
  * Install wget and stress by following commands.
    * ``` yum install wget ```
    * ``` rpm -i ftp://fr2.rpmfind.net/linux/dag/redhat/el7/en/x86_64/dag/RPMS/stress-1.0.2-1.el7.rf.x86_64.rpm ```
  
