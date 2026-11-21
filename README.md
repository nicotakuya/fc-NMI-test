# NMI(Non Maskable Interrupt) test for FC
<img width="781" height="450" alt="vblank" src="https://github.com/user-attachments/assets/676858a3-ee15-4a21-9c2d-b0c43d50dd58" />

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
