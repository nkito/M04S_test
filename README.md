# M04S_test
Test code for Phomemo M04S printer

This code is based on the following pages.

- [Phomemo M834 A4 thermal printer への Python での bluetooth 出力](https://qiita.com/cure_honey/items/1cef2b11291bafbe9d76)
- [Poooli L3 感熱紙プリンタへの Python からの出力　備忘録](https://qiita.com/cure_honey/items/e82a85ef8ca8ed26210a)

This code uses ``minilzo.so``. Following is the steps to obtain it.
~~~
wget http://www.oberhumer.com/opensource/lzo/download/minilzo-2.10.tar.gz
tar xvf minilzo-2.10.tar.gz
cd minilzo-2.10
gcc -I. -shared -fPIC -O2 -o minilzo.so minilzo.c
~~~
It comes from [Poooli L3 感熱紙プリンタへの Python からの出力　備忘録](https://qiita.com/cure_honey/items/e82a85ef8ca8ed26210a)
