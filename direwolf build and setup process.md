

sudo apt-get install git
sudo apt-get install gcc
sudo apt-get install g++
sudo apt-get install make
sudo apt-get install cmake
sudo apt-get install libasound2-dev
sudo apt-get install libudev-dev
sudo apt-get install libavahi-client-dev

cd ~
git clone https://www.github.com/wb2osz/direwolf
cd direwolf
git checkout dev
mkdir build && cd build
cmake ..
make -j4
sudo make install
make install-conf