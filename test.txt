2025/05/20
ファイルの作成：デスクトップはあまりよくない。ドキュメントなどに作成するとよい。
プロジェクトの開始：ターミナルに"flutter create 任意の名前"を入力。ターミナルは Ctrl+@ で開く。
画面表示：ウィジェットで構成されている。入れ子できる。
実行：Runをクリックすると実行される。main関数から実行される。
StatelessWidget：ステートを持たない。ウィジェットのベースとなるクラス。クラス作るときはいったんこれを継承するっぽい。class クラス名 extends StatelessWidget{なんやかんや}
MaterialApp：引数にいろいろ指定できる。return MaterialApp(title:タイトル,home:ホーム);

授業内で使用したコード↓

import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Flutter Demo',
      home: Scaffold(
        appBar: AppBar(title: Text('Hello Flutter!')),
        body: Text('Hello,Flutter World!!', style: TextStyle(fontSize: 32.0)),
      ),
    );
  }
}
