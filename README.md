
### How to build ettercap-0.8.4-rc in debain based operating system(ubuntu,linuxmint,kali-linux,parrot-os etc)? ###

![Screenshot from 2021-02-02 21-19-09](https://user-images.githubusercontent.com/69615463/106626272-b8d46780-65a1-11eb-9aa3-6e04c39251be.png)


<h6>solution :</h6>

h4>Terminal Command :</h4>

+ sudo apt-get install build-essential debhelper bison check cmake flex ghostscript \
   libbsd-dev libcurl4-openssl-dev libgeoip-dev libltdl-dev libluajit-5.1-dev \
   libncurses5-dev libnet1-dev libpcap-dev libpcre3-dev libssl-dev libgtk-3-dev \
   libgtk2.0-dev
+ git clone https://github.com/Ettercap/ettercap.git
+ cd ettercap
+ mkdir build
+ cd build
+ cmake -DENABLE_TYPE_IPV6=On ..
+ make
+ sudo make install
+ ettercap -Tqslq

### How to enable ettercap-0.8.4-rc_debug mode ? ####

![Screenshot from 2021-02-02 21-51-36](https://user-images.githubusercontent.com/69615463/106626362-d9042680-65a1-11eb-8251-202d7107e0f3.png)


<h6>solution :</h6>

<h4>Terminal Command :</h4>

+ cmake -DCMAKE_BUILD_TYPE=Debug On ..
+ make && sudo make install
+ sudo ettercap -Tqslq
+ sudo ettercap -w ettecap-packets-pcap -Tqslq













