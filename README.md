# DP
This would be about dissertation thesis.

1.instalovanie vsetkych potrebných balickov
a)najprv je potrebne updatovat a upgradovat povodne balicky servera
sudo apt update
sudo apt upgrade -y
b)Instalacia Gitu na server pre moznost klonovania repozitara(Na serveri to bolo uz naistalovane)
sudo apt install git
d)Instalacia pythonu pre potreby backendu vo frameworku Flask
sudo apt install python3 python3-pip

2.Klonovanie git repozitara cez ssh tunel
a)Vytvorenie dvojice klucov
ssh-keygen -t rsa -b 4096 -C " email@gmail.com"
cat ~/.ssh/id_rsa.pub
b)Nastavenie ssh kluca na svojom profile
settings --> SSH and GPG keys --> New SSH key
-kde skopirujeme cely obsah suboru id_rsa.pub
c)Overenie funcnosti SSH pripojenia
ssh -T git@github.com
d)Samotne klonovanie git repozitara vo ~/dp/
git clone https://github.com/Igor-Gombala/DP.git


3. Instalacia NS-3
1. wget https://www.nsnam.org/releases/ns-allinone-3.43.tar.bz2
2. sudo apt update
3. sudo apt install g++ python3 cmake ninja-build git gir1.2-goocanvas-2.0 python3-gi python3-gi-cairo python3-pygraphviz gir1.2-gtk-3.0 ipython3 tcpdump wireshark sqlite3 libsqlite3-dev qtchooser openmpi-bin openmpi-common openmpi-doc libopenmpi-dev doxygen graphviz imagemagick python3-sphinx dia imagemagick texlive dvipng latexmk texlive-extra-utils texlive-latex-extra texlive-font-utils libeigen3-dev gsl-bin libgsl-dev libgslcblas0 libxml2 libxml2-dev libgtk-3-dev lxc-utils lxc-templates vtun uml-utilities ebtables bridge-utils libxml2 libxml2-dev libboost-all-dev ccache qt5-qmake qtbase5-dev qtbase5-dev-tools libqt5svg5-dev libqt5webenginewidgets5 libqt5webchannel5-dev qtwebengine5-dev
4. tar xfj ns-allinone-3.43.tar.bz2
5. cd ns-allinone-3.43/
6. ./build.py --enable-examples --enable-tests
7. cd ns-3.42/
8. Preoverenie spravnosti instalacie je mozne spustit tieto skusobne subory:
    a) ./ns3 run hello-simulator
    b) ./ns3 run first.cc
    c) ./ns3 run second.cc
