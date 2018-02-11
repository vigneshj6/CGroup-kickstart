# CGroup-kickstart
To get to know about cgroup


## Steps to get a contained guest os to experiment with:
>note : We are using ubuntu as host os and centos as our guest os
  * Install lxc on ubuntu by using following command
    * sudo apt-get install lxc
  * Start lxc service
    * sudo service lxc-net start
  * Install yum package manager to install centos minimal os
    * sudo apt-get install yum
  * Get the guest os by following command
    * Template of the command ``` lxc-create -n container_name -t container_template ```
    * sudo lxc-create -n centos-sample -t centos
    ```{r, engine='bash', count_lines}
        Complete!
        Fixing rpmdb location ...
        Download complete.
        Copy /var/cache/lxc/centos/x86_64/6/rootfs to /var/lib/lxc/centos-sample/rootfs ... 
        Copying rootfs to /var/lib/lxc/centos-sample/rootfs ...
        Storing root password in '/var/lib/lxc/centos-sample/tmp_root_pass'
        Expiring password for user root.
        passwd: Success

        Container rootfs and config have been created.
        Edit the config file to check/enable networking setup.

        The temporary root password is stored in:

                '/var/lib/lxc/centos-sample/tmp_root_pass'


        The root password is set up as expired and will require it to be changed
        at first login, which you should do as soon as possible.  If you lose the
        root password or wish to change it without starting the container, you
        can change it from the host by running the following command (which will
        also reset the expired flag):

                chroot /var/lib/lxc/centos-sample/rootfs passwd


    ```

