---
layout: post
title: prepare-to-read
---

### [yamanetoshi](https://github.com/RHGReadingOkinawa/rhgreadingokinawa.github.com/issues/6)

#### 環境設定について

とりあえずソースを入手。Git リポジトリに 1.7.3 が含まれていると嬉しいのですが。

    $ git clone https://github.com/ruby/ruby

git tag 見てみるに

    v1_6_8
    v1_7_1
    v1_8_0

とのこと。[「Rubyソースコード完全解説」を読む(1)](http://rubyist.g.hatena.ne.jp/muscovyduck/20071109/p1) によると

- [http://i.loveruby.net/ja/rhg/ar/ruby-rhg.tar.gz](http://i.loveruby.net/ja/rhg/ar/ruby-rhg.tar.gz)

から入手可能とのことで wget で入手。

    $ wget http://i.loveruby.net/ja/rhg/ar/ruby-rhg.tar.gz

展開。

    $ tar zxvf ruby-rhg.tar.gz
    $ cd ruby-rhg

一応コンパイルしておいて

    $ ./configure
    $ make

一応 make は正常終了しているようです。

    make[1]: Leaving directory `/home/rms/tmp/RHG/ruby-rhg/ext/digest/rmd160'
    make[1]: Entering directory `/home/rms/tmp/RHG/ruby-rhg'
    gcc -g -O2 -rdynamic   main.o  libruby.a -ldl -lcrypt -lm   -o ruby
    make[1]: Leaving directory `/home/rms/tmp/RHG/ruby-rhg'


タグを作成。

    $ gtags -v

これで準備完了でしょうか。make したのは一応 make しないと作成されないファイルがあるかも、という配慮によります。必要かどうかは不明です。
