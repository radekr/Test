1. vm.swappiness (Linux Swapping) 
   sysctl vm.swappiness=1

2. noatime - reduce disk io (X)

3. reserve space - (X)

4. maximun file descriptor and process - ulimit -a 
   open files                      (-n) 1024
   max user processes              (-u) 59433
   ulimit -n 10000
   
5. Test forward and reverse host lookups for correct resolution (X)

6. name service cache deamon - nscd 
   yum install nscd && service nscd start

7. network time protocol daemon - ntpd 
   yum install ntp && service ntpd start
    
8. echo never > /sys/kernel/mm/redhat_transparent_hugepage/defrag 
