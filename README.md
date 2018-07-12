# upgrade framework for private cloud

- upgrade objects:
Hypervisor
Host agent
Management Node
...

- upgrade modes:
cold upgrade
hot upgrade
first time deployment
...

- upgrade strategy:
HA upgrade
reversely upgrade
DPM like upgrade
...

https://developer.nvidia.com/compute/cuda/9.2/Prod/local_installers/cuda_9.2.88_396.26_linux
http://cn.download.nvidia.com/tesla/396.26/NVIDIA-Linux-x86_64-396.26.run 
yum install kernel-devel
yum update kernel
reboot
install g++

!!rolling upgrade!!
https://yq.aliyun.com/download/2860   core of elastic cloud, the elastic scheduling based on hot migration, alicloud
scope and challenge:
not only ECS
add hot migration to current ECS solution
define the behavior border of virtual compute, network, storage and management/ops within hot-migration to support more complex product and scenario
hot-migration architecture based on data driven(monitor/event/load). Pre_Analysis-->Plan-->Strategy-->Action-->Rollback


!!migration scheduling!!: 
BtrPlace: 
http://www.btrplace.org
https://rd.springer.com/content/pdf/10.1007%2F978-3-319-14313-2_42.pdf
https://team.inria.fr/DAESD/files/2012/05/Fabien-BtrPlace.pdf
mVM: http://www.btrplace.org/pubs/kherbache-tcc17.pdf
