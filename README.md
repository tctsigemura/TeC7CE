# Tokuyama Educational Computer Ver.7 (TeC7CE)

TeCのCPUを実装する学生実験用のVHDLソースです．
CPU内部が実装してありません．
Cpu.vhdの内容を自分で作成して完成してください．

約50MHz(RAMが逆相なので実質100MHz)で動作させます．
組み合わせ回路に許される遅延は基本的に20ns以内です．
RAMとのインタフェース部分は10ns以内です．
真面目に設計しないと制約を満たすことができません．

```
+ README.md                   このファイル自身
|
+ Vhdl -------+               演習用に配布する設計データ
|             |
|             + Cpu.vhd       このファイルに CPU の機能を＊＊自分で＊＊実装する
|             |
|             + TeC.vhd       TeC のトップレベルを記述した VHDL
|             |
|             + Console.vhd   コンソールパネルの機能を実装した VHDL
|             |
|             + Ram.vhd       TeC主記憶用の256バイトRAMを記述したVHDL
|             |
|             + Dcm.vhd       外部 9.8304MHz クロックから 49.1520MHz を発生
|             |
|             + TeC7a.ucf     TeC7aボード用の制約ファイル
|             |
|             + TeC7.bit      配布設計データのコンパイル結果
|
+ VhdlExample +               Cpu.vhd の実装例
|             |
|             + Cpu.vhd       CPU の実装例
|             |
|             + Sequencer.vhd CPU の制御回路実装例
|             |
|             + TeC7.bit      実装例のコンパイル結果
|
+ Doc --------+               資料
              |
              + BlockDiagram  トップレベル(TeC.vhd)を図で表現したもの
```