# GadgetViewer-install-manual

1. install gtk-2.0
```shell
sudo apt install libgtk2.0-dev
```


2. install GadgetViewer (you need hdf5 first)
```shell
sudo wget https://github.com/jchelly/gadgetviewer/releases/download/1.1.3/gadgetviewer-1.1.3.tar.gz

sudo tar xvfz gadgetviewer-1.1.3.tar.gz

sudo ./configure --prefix=/opt/gadgetviewer/1.1.3 --with-hdf5=/opt/hdf5/1.10.1

sudo make -j12

sudo make install
```


3. Edit ~/.bashrc
```shell
export PATH=/opt/gadgetviewer/1.1.3/bin:$PATH
```


4. test run
```shell
gadgetviewer
```
