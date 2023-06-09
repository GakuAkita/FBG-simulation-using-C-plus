# FBG Simulation

### モード結合理論を用いたFBGの反射スペクトルの計算に用いたスクリプトです。<br>
まず私が作った[モード結合理論の講義](https://www.youtube.com/watch?v=TqTylSkIf_Q)を紹介しておこうと思います。モード結合理論の概要を説明しています。
pythonは基本的にfor文が非常に遅く、numpyを使うことでfor文を使わずにかければそれで良かったですが、計算過程が複雑でできませんでした。<br>
そこで、計算処理が早いC++を用いて行列の計算は行い、計算結果をcsvで出力しグラフ化はpythonで行うというような方法でシミュレーションしました。C++はfor文やそれだけに限らず処理が速いそうです。<br>
<br>
C++で高速に計算を行う方法を探す中で、Eigenというライブラリの存在を知りました。使うには特定のフォルダをダウンロードする必要がありますが、それも含めてセットアップの手順は[この動画](https://www.youtube.com/watch?v=XmtNr1TuO-E)が参考になりました<br>
Source.cppがVisual Studioを用いて私が書いたコードです。コピーしてすぐ使えるようなものではないと思うので、あくまでこのスクリプトは参考程度にして、0から手を動かしながら自分なりに書いていくことをおすすめします。
