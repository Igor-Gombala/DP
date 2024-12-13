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
