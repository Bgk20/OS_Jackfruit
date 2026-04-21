Test Case 1: Container Creation
Command: sudo ./engine start alpha ../rootfs-alpha /bin/sh
Output: Container started and minimal filesystem visible using ls /

Test Case 2: Multiple Containers
Command: sudo ./engine start beta ../rootfs-alpha /bin/sh
Output: Multiple containers running simultaneously

Test Case 3: Memory Workload
Command: sudo ./engine run gamma ../rootfs-alpha /bin/memory_hog
Output: Memory allocation increasing (8MB, 16MB, ...)

Test Case 4: Kernel Module
Command: ls /dev/container_monitor
Output: Device file created successfully
