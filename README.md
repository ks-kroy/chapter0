# chapter0
## 概要
「第0章」を「序章」にするやつ。  
¥chapter{hoge}としたときに、それが「第0章」の場合、「序章 hoge」ってなります。  

## 使い方
1. この機能を使いたいtexファイルがあるディレクトリにchapter0.styを置く。
2. texファイルの適切な場所に¥usepackage{chapter0}を入れる。
3. ¥chapter{}を始める前に¥setcounter{chapter}{-1}を入れる。
4. ¥setcounter{chapter}{-1}を書いた以降で最初の¥chapter{hoge}が「序章 hoge」になる。
5. 以降の¥chapter{fuga}は「第1章 fuga」のようになる。  
3をしなければ、いつも通り「第1章」から始まります。

## サンプル
test.texをplatex,dvipdfmxするとtest.pdfになります。
¥documentclass{jbook}でしか試してません。
