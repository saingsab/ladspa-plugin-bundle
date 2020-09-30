### About
ladspa-plugin-bundle is a archive repository from ladspa the original software is at ladspa.org.
This plugin work with Ardour (DAW).

### Install
#### 1 Install Ladspa SDK
Build and install SDK 
```
cd ladspa_sdk_1.15
make -j4
sudo make install
```
#### 2 Install cmt
CMD is a plugin install with bellow comment.
```
cd cmt_1.17 
make -j4
sudo make install
```

Note: make -j4 the 4 is meand your number of core processor of your computer.