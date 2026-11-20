# NMI(Non Maskable Interrupt) test for FC
<img width="514" height="500" alt="nmi_test" src="https://github.com/user-attachments/assets/2deaa3d4-38fc-4c87-954c-acf96abb8c35" />

NMI（ノン・マスカブル割り込み）の実験をするファミコン用プログラムです。

NMIが発生すると、チック時間カウンタを1つ加算します。メインプログラムではチック時間カウンタを監視して、値が変化したらVブランクが発生したと判断します。

画面の3ケタの数値は秒数です。Vブランクを60回検出すると1つ加算します。

100秒ごとにVブランクの検出方法(NMI/PPUステータス)を自動的に切り替えます。

## Files
・rom.nes：ROMイメージです。

・startup.asm：起動プログラムです。NMIの処理もここに入っています。

・main.c：メインプログラムです。

・build.bat：CC65でビルドするバッチファイルです。

## Movie
https://youtu.be/KFO3MBrEwLs
