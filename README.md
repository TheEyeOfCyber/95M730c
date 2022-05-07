<a href="https://imgbb.com/"><img src="https://i.ibb.co/7YCnBpJ/20220507-104628-0000-removebg-preview.png" alt="20220507-104628-0000-removebg-preview" border="0"></a>
======
<h1> 95M730c  </h1>
Python based tool used to collect the imsi and for its modification according to your need. it helps to capture the packets to understand the gsm and collection sms & numbers.
</br>
Tested on last Kali Linux Version 5.15.0-kali2-amd64 + Ubuntu Jammy Jellyfish (development branch) on [07th May of 2022]
<h2> Disclaimer :- </h2>
<p2>This program was made to understand how GSM network works. Not for bad hacking ! We are not responsible for any illegal activity !</p2>
======
<h2> Requirements :- </h2>
<p2>
•kali linux
 </br>
•Rtl-sdr with antenna (or) Hackrfone
</p2>
<h2> Installation </h2>

git clone https://github.com/TheEyeOfCyber/95M730c/
sudo apt-get install python-pyshark

Install Gr GSM : ( For receiving GSM transmissions )

sudo add-apt-repository -y ppa:ptrkrysik/gr-gsm
sudo apt-get update
sudo apt-get install gr-gsm
If gr-gsm failled to setup. Than follow those this : https://github.com/ptrkrysik/gr-gsm/wiki/Installation

Install Kalibrate : ( For finding frequencies )

sudo apt install build-essential libtool automake autoconf librtlsdr-dev libfftw3-dev
git clone https://github.com/steve-m/kalibrate-rtl
cd kalibrate-rtl
./bootstrap && CXXFLAGS='-W -Wall -O3'
./configure
make
sudo make install
