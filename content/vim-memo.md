+++
date = "2016-05-03T14:43:32+09:00"
draft = true
title = "vim コマンドのメモ"

+++

vim 使えるようになろうと何度か挑戦するもことごとくコマンドを忘れてemacsでいいか...ってなるので自分が覚えたコマンドだけをメモとして残す。

## 移動

h j k l

← ↓ ↑ →

* 0  : 行等
* gg : ファイルの先頭
* G  : ファイルの末尾
* 行番号G : 行番号に移動
* %  : 対応するカッコに移動

## ノーマルモード -> 挿入モード

* i : カーソル手前の位置から
* A :行末から

## 削除

* x  : delete
* dw : 単語削除・単語直後の空白も削除する(deは空白残す) 
* d$ : カーソル位置から行末まで消す
* dd : 行全体を消す

## 検索

* /hoge : 前方にhogeを検索, nで次, Nで逆方向, ctl-oで元の位置に戻る
* ?hoge : 逆方向に検索

## 置換

* :s/foo/bar : 行内の最初のfooをbarに置き換え
* :s/foo/bar/g : 行内のすべてのfooをbarに置き換え
* :%s/foo/bar/g : ファイル内のすべてのfooをbarに置き換え

## 外部コマンド実行

:!コマンド