# FC NMI test
<img width="514" height="500" alt="nmi_test" src="https://github.com/user-attachments/assets/2deaa3d4-38fc-4c87-954c-acf96abb8c35" />

ファミコン用のプログラムです。
NMI（ノン・マスカブル割り込み）でVBLANKを検出できるかを実験するために作りました。

画面の3ケタの数値は秒数です。VBLANKを60回検出すると1つ加算します。

rom.nesがROMイメージです。

build.batを実行すると、CC65でビルドします。
