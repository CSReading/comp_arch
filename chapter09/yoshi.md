### 9-3
#### 問
- プログラムに一個のif-then-else命令が含まれています. 
    - 条件が真だった時, いくつの分岐命令が実行されますか？
    - 条件が偽だった時, いくつの分岐命令が実行されますか？
#### 答
- 下記のようなコードを考える.
    ```
    if (hoge){
        thenのコード
    } else {
        elseのコード
    }

    次のステートメント
    ```
- assembly としては以下のような形で表現できる.
    ```
        cmp hoge
        bne lab1
        thenのコード
        jmp lab2
    lab1: elseのコード
    lab2: 次のステートメントのコード
    ```
- よって分岐は真の時は2回, 偽の時は1回（jumpは無条件分岐として分岐命令に含めた）

### 9-8
#### 問
- プログラマは時々間違って、「アセンブラ言語」ということがあるが何が間違っているか？正しい用語は？
#### 答
- アセンブリ言語が正しい.
- アセンブラは, アセンブリ言語をプロセッサが実行できるバイナリコードに変換するソフトウェアのことであり, 言語というには相応しくない.
