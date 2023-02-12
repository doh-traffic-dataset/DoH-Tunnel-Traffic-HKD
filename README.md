# The DoH-Tunnel-Traffic-HKD dataset

* The dataset contains PCAP files (DoH-Pcaps.zip) of DoH tunnel traffic generated by dnstt [1], tcp-over-dns [2], and tuns [3].

* The dataset also includes CSV files (DoH-CSVs.zip) of statistical traffic features extracted from PCAP files by DoHlyzer [4].

* The "Total-48h-Augmentation.csv" includes traffic flows of dnstt 46080, tcp-over-dns 30040, tuns 29040, augmented assuming 20 client PCs.

* If your papers use the dataset, please cite the following paper.

* Rikima Mitsuhashi, Yong Jin, Katsuyoshi Iida, Takahiro Shinagawa, and Yoshiaki Takai, 
"Malicious DNS Tunnel Tool Recognition using Persistent DoH Traffic Analysis,"
*in IEEE Transactions on Network and Service Management*, 2022.<br>
https://ieeexplore.ieee.org/document/9924534 (Early Access)

# Network connections and capturing point

![network](https://user-images.githubusercontent.com/101712711/173388419-2981578d-7157-42e9-a6b3-1ebe67f44d9c.png)


* The destination of all tunnel tools is a suspicious DNS server.

* The dnstt directly connects to a DoH server because it supports a DoH protocol.

* On the other hand, the tcp-over-dns and tuns use DoH proxy to convert conventional DNS into DoH.

# Appendix - The CIRA-CIC-DoHBrw-2020 and DoH-Tunnel-Traffic-HKD combined dataset

* The dataset contains three CSV files:  l1-total-add.csv, l2-total-add.csv, and l3-total-add.csv.

* The CSV files include traffic flows of Non-DoH 897493, DoH 374803, Normal DoH 19807, Suspicious DoH 354996, dns2tcp 167486, dnscat2 35770, iodine 46580, dnstt 46080, tcp-over-dns 30040, and tuns 29040.
 
* If you use the CSV files, please be sure to cite previous studies for both datasets in your paper.
    1. https://ieeexplore.ieee.org/document/9251211 (CIRA-CIC-DoHBrw-2020 [5])  
    2. https://ieeexplore.ieee.org/document/9924534 (DoH-Tunnel-Traffic-HKD)

* Note that the "l1-total-add.csv" is currently too large to open in Microsoft Excel.
  Use a text editor such as Vim to view its contents.

# References
* [1] dnstt</t>  (https://www.bamsoftware.com/software/dnstt/)
* [2] tcp-over-dns</t> (https://analogbit.com/software/tcp-over-dns/)
* [3] tuns</t> (https://github.com/lnussbaum/tuns, and https://www.loria.fr/~lnussbau/tuns.html)
* [4] DoHlyzer</t> (https://github.com/ahlashkari/DoHlyzer)
* [5] CIRA-CIC-DoHBrw-2020</t> (https://www.unb.ca/cic/datasets/dohbrw-2020.html)
