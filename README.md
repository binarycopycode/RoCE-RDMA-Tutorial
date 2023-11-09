# RoCE-RDMA-Tutorial

it is extended fromRDMA-Tutorial and can work in the RoCE rdma network

https://github.com/jcxue/RDMA-Tutorial

refer to https://github.com/CarpenterLee/rdma_examples

local test enviroment:

ubuntu 22.04 (virtual machine)

gcc 12.1

# compile and use
`make` or `make debug`

server terminal:  `./rdma-tutorial port`
client terminal:  `./rdma-tutorial server_ip  port`

do not forget `sudo rdma link add rxe_name type rxe netdev xxx` in ubuntu
