# fsping
Determine the rtt latency of a local or distributed filesystem.
# Example:

@lxplus126 fsping> ./fsping --server
FSPING reflector /afs/cern.ch/user/d/dvanders/git/fsping prefix lxplus126
524384 bytes from lxplus126.syn 13 bytes to lxplus126.ack seq=1
524385 bytes from lxplus126.syn 13 bytes to lxplus126.ack seq=2
524385 bytes from lxplus126.syn 13 bytes to lxplus126.ack seq=3
524384 bytes from lxplus126.syn 13 bytes to lxplus126.ack seq=4
524385 bytes from lxplus126.syn 13 bytes to lxplus126.ack seq=5
524385 bytes from lxplus126.syn 13 bytes to lxplus126.ack seq=6
524385 bytes from lxplus126.syn 13 bytes to lxplus126.ack seq=7
524384 bytes from lxplus126.syn 13 bytes to lxplus126.ack seq=8
524384 bytes from lxplus126.syn 13 bytes to lxplus126.ack seq=9
524384 bytes from lxplus126.syn 13 bytes to lxplus126.ack seq=10
--- All done ---

@lxplus025 fsping> ./fsping --prefix lxplus126 --size=$((512*1024))
FSPING client lxplus126 524288 bytes of data 10 pings
524384 bytes to lxplus126.syn 13 bytes from lxplus126.ack seq=1 time=59.18 ms
524385 bytes to lxplus126.syn 13 bytes from lxplus126.ack seq=2 time=43.18 ms
524385 bytes to lxplus126.syn 13 bytes from lxplus126.ack seq=3 time=94.05 ms
524384 bytes to lxplus126.syn 13 bytes from lxplus126.ack seq=4 time=20.43 ms
524385 bytes to lxplus126.syn 13 bytes from lxplus126.ack seq=5 time=51.39 ms
524385 bytes to lxplus126.syn 13 bytes from lxplus126.ack seq=6 time=33.79 ms
524385 bytes to lxplus126.syn 13 bytes from lxplus126.ack seq=7 time=31.25 ms
524384 bytes to lxplus126.syn 13 bytes from lxplus126.ack seq=8 time=33.78 ms
524384 bytes to lxplus126.syn 13 bytes from lxplus126.ack seq=9 time=37.66 ms
524384 bytes to lxplus126.syn 13 bytes from lxplus126.ack seq=10 time=42.73 ms
--- lxplus126 fsping statistics ---
10 writes sent, 10 received
rtt min/avg/max = 20.429/44.744/94.045 ms
