# Network Attacks

* Eavesdropping using tool: Network tap or span

* Spam

* Overlapping Fragment

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

* Prevention

Firewall Filtering, 防火牆過濾 (by address || by service port)

