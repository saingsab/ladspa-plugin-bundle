### About
ladspa-plugin-bundle is a archive repository from ladspa the original software is at ladspa.org.
This plugin work with Ardour (DAW).

### Install
#### 1 Install Ladspa SDK
Build and install SDK 
```
cd ladspa_sdk_1.15/src
make
sudo make install
```
After make comment should see the following message in your terminal
```
Peak output: 27349.5
---------------------------------------------
First listen to the white noise input signal:
---------------------------------------------
sndfile-play ../snd/noise.wav
Playing ../snd/noise.wav
-------------------------
Compare to plugin output.
-------------------------
Should be a noise band around 6000Hz, repeated quietly after 1s.
sndfile-play /tmp/test.wav
Playing /tmp/test.wav
Test complete.
```
Successfully installation whould show the following message
```
mkdir -p /usr/lib/ladspa/
mkdir -p /usr/include/
mkdir -p /usr/bin/
cp ../plugins/* /usr/lib/ladspa/
cp ladspa.h /usr/include/
cp ../bin/* /usr/bin/
```
#### 2 Install cmt
CMD is a plugin install with bellow comment.
```
cd cmt_1.17/src/
make
sudo make install
```

Note: make -j4 the 4 is meand your number of core processor of your computer.