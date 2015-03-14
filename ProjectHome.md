it's a service menu designed for dolphin

it can print your file :
photos
text
ps
pdf (1)
libreoffice files (2)


you can create a list of files to print and print then directly from dolphin


1 for pdf it has still problems
2 experimental



INSTALLATION

sudo apt-get install subversion ; sudo apt-get install  libreoffice-java-common openjdk-7-jre

double click to select the code , right click on selection , copy and paste on a konsole.

```
cd /tmp/ ; svn checkout http://lprinter-qt.googlecode.com/svn/trunk/ lprinter-qt-read-only ; cd lprinter-qt-read-only/;sudo cp "$PWD"/usr/bin/lprinter-qt /usr/bin/lprinter-qt  && sudo chmod +x /usr/bin/lprinter-qt && sudo cp "$PWD"/usr/share/kde4/services/lprinter-qt.desktop  /usr/share/kde4/services/ServiceMenus/lprinter-qt.desktop  && sudo cp "$PWD"/usr/bin/lprinter-qt-office /usr/bin/lprinter-qt-office  && sudo chmod +x /usr/bin/lprinter-qt-office && sudo cp "$PWD"/usr/share/kde4/services/lprinter-qt-office.desktop  /usr/share/kde4/services/ServiceMenus/lprinter-qt-office.desktop  && kbuildsycoca4 
```




UNISTALL

```
sudo rm /usr/bin/lprinter-qt-office ; sudo rm /usr/bin/lprinter-qt ; sudo rm /usr/share/kde4/services/ServiceMenus/lprinter-qt.desktop ; sudo rm /usr/share/kde4/services/ServiceMenus/lprinter-qt-office.desktop 
```