centos7��װ������
��װcentosϵͳ����

yum install -y automake autoconf libtool gcc gcc-c++ 
yum install -y libpng-devel libjpeg-devel libtiff-devel
��װleptonica

wget http://www.leptonica.org/source/leptonica-1.72.tar.gz
tar xvzf leptonica-1.72.tar.gz
cd leptonica-1.72/ 
./configure 
make && make install
��װtesseract-ocr

wget https://github.com/tesseract-ocr/tesseract/archive/3.04.zip
unzip 3.04.zip
cd tesseract-3.04/ 
./configure
make && make install 
sudo ldconfig


## 4.0��װ
1. ����tesseract-ocrԴ��
git clone -b master https://github.com/tesseract-ocr/tesseract.git tesseract-ocr
2. ��װg++
yum?install?gcc?gcc-c++?make
3. ��װautoconf automake libtool libjpeg-devellibpng-devel libtiff-devel zlib-devel
yum install autoconf automake libtool
yum install libjpeg-devel libpng-devel libtiff-devel zlib-devel
4. ��װleptonica
wget http://www.leptonica.org/source/leptonica-1.76.0.tar.gz
��ѹ�� ����Ŀ¼������ִ��:
./configure
make
make install
������ɺ�ʹ��vim������������������
vim /etc/profile
export LD_LIBRARY_PATH=$LD_LIBRARY_PAYT:/usr/local/lib
export LIBLEPT_HEADERSDIR=/usr/local/include
export PKG_CONFIG_PATH=/usr/local/lib/pkgconfig

�����ִ�У� source /etc/profile
5.???�����1�����ص�tesseract-ocrĿ¼����ִ���������
./autogen.sh
./configure
make
make install
6.???��װpytesseract
pip install pytesseract
