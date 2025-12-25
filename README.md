# 001cc-results
include dctcp,dcqcn,timely,PRTT

fct.txt
sip, dip, sport, dport, size (B), start_time, fct (ns), standalone_fct (ns)
0b000401 0b000101 10000 100 150000000 2000000000 44300942 12580160
仿真第 2 秒时，从节点 4 的 10000 端口到节点 1 的 100 端口，发起了一次 143 MB 的 RDMA 流传输，实际耗时 44.3 毫秒（受拥塞影响），而无拥塞时理论上仅需 12.6 毫秒。
