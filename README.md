# ipmi-wrapper
Time saver for ipmitool when pxe booting servers

## Prerequisites 

- A working instalation of [ipmitool](http://sourceforge.net/projects/ipmitool/). Typically this can be installed in linux with the integrated package manager. For redhat and derivatives try ```yum install ipmitool```.
- I've only tested under the bash shell so you might need this.

## Usage

Put your password into an environment varible with the ```set-ipmi-pass.bash``` script:

    $ source ./set-ipmi-pass.bash 
    Enter IPMI password:

Then you can use the ipmi comand:

    ipmi <host> <command>
   
    host      hostname or IP address of controller
    command	  <native ipmitool command> e.g. help
    command	  console | bootnet | reboot"
