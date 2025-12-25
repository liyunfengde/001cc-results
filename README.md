# 001cc-results
include dctcp,dcqcn,timely,PRTT

fct.txt
sip, dip, sport, dport, size (B), start_time, fct (ns), standalone_fct (ns)
0b000401 0b000101 10000 100 150000000 2000000000 44300942 12580160
仿真第 2 秒时，从节点 4 的 10000 端口到节点 1 的 100 端口，发起了一次 143 MB 的 RDMA 流传输，实际耗时 44.3 毫秒（受拥塞影响），而无拥塞时理论上仅需 12.6 毫秒。


qlen.txt
time: 2000000000  # 仿真时间：2000000000 ns = 2秒
0 1 5 3 1 0        # 交换机ID=0，端口ID=1：0KB出现5次，1KB出现3次，2KB出现1次，3KB及以上0次
0 2 8 2 0          # 交换机ID=0，端口ID=2：0KB出现8次，1KB出现2次，2KB及以上0次
time: 2100000000  # 下一个dump时间：2100000000 ns = 2.1秒
0 1 6 2 1 1        # 交换机0端口1的最新统计
...
