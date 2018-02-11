# CGroup Commands
  * Start CGroup by executing ``` service cgconfig start ```
  * Create the corresponding directory using mkdir.
    * ``` mkdir /cgroup/memory ```
  * Mount the directory using mount command.
    * ``` mount -t cgroup -o memory memory /cgroup/memory ```
  * list the files to see the memory control bindings.
  
