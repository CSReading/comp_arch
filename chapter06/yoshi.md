### 6-1
#### 問
- サンプルシステムはフォン・ノイマン・アーキテクチャか
#### 答
- ハーバードアーキテクチャ
- 命令を格納するメモリと,データを格納するメモリが分離しているため.

### 6-6
#### 問
- 図6-4の回路はなぜ単なる無限ループとして暴走しないのか
#### 答
- クロックと同期する形で、一つの命令が完了したのちに次のインクリメントが行われる. そのためプログラムカウンタは次のクロックパルスが来るまで更新されないため.

### 6-11
#### 問
- 図6-8で, add命令の時にマルチプレクサM1が入力に選ぶのはどの値ですか
#### 答
- 32 bit adderの出力値.
- マルチプレクサM1はALUの計算が参照する命令メモリのaddressに影響を与えるようなjump命令の時にのみALUのM3の値を参照する.
