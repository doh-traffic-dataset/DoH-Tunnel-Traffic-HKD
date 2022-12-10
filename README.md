# The DoH-Tunnel-Traffic-HKD dataset

* The dataset contains packet capture (pcap) of DoH tunnel traffic generated by dnstt [1], tcp-over-dns [2], and tuns [3].

* The dataset also contains traffic features and traffic flows (csv) extracted by DoHlyzer [4].

* "Total-48h-Augmentation.csv" has traffic flows consisting of dnstt 46080, tcp-over-dns 30040, tuns 29040.

* If your papers use the dataset, please cite the following paper.

* Rikima Mitsuhashi, Yong Jin, Katsuyoshi Iida, Takahiro Shinagawa, and Yoshiaki Takai, 
"Malicious DNS Tunnel Tool Recognition using Persistent DoH Traffic Analysis,"
in IEEE Transactions on Network and Service Management, 2022.<br>
https://ieeexplore.ieee.org/document/9924534 (Early Access)

# Network connections and capturing point

![network](https://user-images.githubusercontent.com/101712711/173388419-2981578d-7157-42e9-a6b3-1ebe67f44d9c.png)


* The destination of all tunnel tools is a suspicious DNS server.

* The dnstt directly connects to a DoH server because it supports a DoH protocol.

* On the other hand, the tcp-over-dns and tuns use DoH proxy to convert conventional DNS into DoH.

# References
* [1] dnstt</t>  (https://www.bamsoftware.com/software/dnstt/)
* [2] tcp-over-dns</t> (https://analogbit.com/software/tcp-over-dns/)
* [3] tuns</t> (https://github.com/lnussbaum/tuns, and https://www.loria.fr/~lnussbau/tuns.html)
* [4] DoHlyzer</t> (https://github.com/ahlashkari/DoHlyzer)
