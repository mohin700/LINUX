# Manually Instal Linux Desktop Applications (APPs)

#### Download POSTMAN/Others Packge (tar.gz in formet) 
#### Postman link: [Download](https://www.postman.com/downloads)

### extract Postman package:
``` 
tar -xzf Postman-linux-x64-VERSION-NAME.tar.gz
```

### If already have installed previous version first remove it.
```
sudo rm -rf /opt/Postman
```

### Move Postman directory to opt/ directory
```
sudo mv Postman /opt
```

### Create a Symbolic Links
```
sudo ln -s /opt/Postman/Postman /usr/local/bin/postman
```

### Run Postman through the terminal
```postman```


### Create a desktop file for Postman App
```
sudo gedit /usr/share/applications/postman.desktop
```

### Add following lines
```
[Desktop Entry]
Type=Application
Name=Postman
Icon=/opt/Postman/app/resources/app/assets/icon.png
Exec="/opt/Postman/Postman"
Comment=Postman GUI
Categories=Development;Code;
```

