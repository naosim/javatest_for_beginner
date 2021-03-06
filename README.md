# java入門_チェックKATA

ルールとか
- 下記の問題を解く際に、IDEを使うのはNGです。メモ帳等を使ってください。
- 前準備: こんなディレクトリを作ってから始めてください。

```
ex  + main - java
    |
    + test - java
```

- 採点基準:
  - IDEに貼り付けた時にシンタックスエラーがなく、正しく動作すること
  - ただし以下は減点対象外
    - スペルミス
    - import文 (書かなくてもOK)


## 問題1: 構文
以下の仕様に従いクラスを作成しなさい。  
※仕様にない部分は自由でOKです。

仕様:
- Hogeクラス
  - パッケージはhoge

  
- Barインターフェース
  - パッケージはbar
  - Barインターフェースはbarメソッドを定義している
  - barメソッドは引数にint型をとる
  - barメソッドの戻り値はint型である

  
- Pooクラス
  - パッケージはpoo
  - Pooクラスはパブリックなインスタンスメソッドpoo1を実装している
  - poo1は引数にint型をとり、例外Exceptionをスローする可能性がある
  - poo1の戻り値はboolean型である
  - Pooクラスはパブリックなスタティックメソッドpoo2を実装している
  - poo2は引数にintをとり、戻り値はString型である

  
- Fooクラス
  - パッケージはfoo
  - FooクラスはHogeクラスを継承している
  - FooクラスはBarインターフェースを実装している
  - Fooクラスはフィールドにファイナルでpooインスタンスを持っている
  - Barインターフェースの実装の中で、Pooクラスのpoo1メソッドを呼び出す
  - Barインターフェースの実装の中で、Pooクラスのpoo2メソッドを呼び出す

## 問題2: fizzbuzz
pooクラスの中にパブリックなインスタンスメソッドfizzbuzzを作成しなさい。  
fizzbuzzメソッドは引数をint型、戻り値をStringがとする

## 問題3: fizzbuzzのテスト
問題2のfizzbuzzのテストを書いてください。  
テストは1〜15までの値でやってください。
