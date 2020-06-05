# 7 畳み込みニューラルネットワーク

## 7.2 畳み込み層

入力サイズ、カーネルサイズ、パディングサイズ、ストライドの値から出力サイズが決定される。基本的には、整数値で出力できる様に各層について調整する必要があることに注意。

## 7.3 プーリング層

学習するパラメータが存在し無い。プーリングのウィンドウサイズとストライドはハイパーパラメータ。

## 7.4 Convolution/Pooling レイヤの実装

Image To Column: 画像配列要素を一次元に変換して、効率的に行列計算を行える様にデータを一時的に取り出す。ストライドの関係上、データ抽出の重複が起きるためメモリを消費するが、行列計算の効率化による恩恵が大きい。

![img2col](https://qiita-user-contents.imgix.net/https%3A%2F%2Fqiita-image-store.s3.ap-northeast-1.amazonaws.com%2F0%2F299928%2F63062447-0d72-7e71-93b1-a978de00ea79.png?ixlib=rb-1.2.2&auto=format&gif-q=60&q=75&w=1400&fit=max&s=37bf20b92187d4bc787d3d6a9803f52f)

### 参考
* [畳み込み演算とim2col](https://qiita.com/nishiha/items/540db2e4eef66ed567da)
