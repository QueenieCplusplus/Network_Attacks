# Network Attacks

* Eavesdropping using tool: Network tap or span

* Spam

* Bypass FW

![](https://ichef.bbci.co.uk/news/976/cpsprodpb/2B87/production/_90934111_1-1.jpg)

543 --- Packet Filter (Static Packet/Stateful or Dynamic Packet)

544 --- Proxy (Web level/App level/Circut level)

545 --- Scanning (Port/FIN/TCP seq) using tool: Nessus/Nmap
 
550 --- Tool (tcpdump)


# Eavesdropping, 竊聽

this attack is particularly easy in wireless LANs, where no physical connections are necessary, and it is advantageous for an attacke to remain invisible (unaddressable) on the network.

![eavesdrop](https://cdn2.iconfinder.com/data/icons/man-and-door/351/door-022-512.png)

* Prevention

(1) Encrption on network level or app level

(2) Traffic padding to prevent identify time

(3) Reroute to anonymize its origin

(4) Mandate trusted routed for data (the info is only traversing trusted network domain)

# Spam, 垃圾郵件（罐頭早餐肉）

spammers manipulate the content and keywors in therir msg.

![spam](https://blog.trendmicro.com.tw/wp-content/uploads/2011/10/spam.jpg)

* Prevention

to do a filter to mail server (Mail Transfer Agent & Mail User Agent) by administrator, to config a blacklist of spam src.

# Overlapping Fragment bypass FW, 穿透防火牆的攻擊

the leak that FW has is that it only inspect the 1st fragment of a fragmented packets. Hacker sends out a 1st harmless fragment, which will satisfy the packet filter. Other packets followed wil then overwrite the 1st fragement with malicios data.

![FW](https://thetechwin.files.wordpress.com/2019/03/ngfw.png?w=1000)

* Remark

IP fragmentation is an internet protocol process that breaks packets into smaller fragments, so that the resulting pieces can pass through a link with a smaller maximum transmission unit (MTU) than the original packet size.

The fragments are reassembled by the receiving host.

* Prevention

a solution to this problem is for TCP/IP stacks not to allow fragments to overwrite each other.

