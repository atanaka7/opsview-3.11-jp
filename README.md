Opsview Community Edition 3.11の日本語化
========================================

ここで公開しているファイルは、Opsview Community Edition 3.11を日本語化するためのファイル群です。

ja.po
-----

opsview-webで利用する日本語用の言語ファイルです。
RPMを利用してopsview-webをインストールしている場合は、
  /usr/local/opsview-web/lib/Opsview/Web/I18N/
以下にコピーして利用してください。

nagios_japanese_with_opsview.patch
----------------------------------

opsview-baseには、Nagios 3.2.3が含まれています。
この含まれているNagiosを日本語化するには、opsview-baseをコンパイルする時にこのパッチファイルを利用することが必要です。

このパッチは、ももーいさんが公開して下さっている[Nagios 3.2.3用のパッチ](http://www.momo-i.org/chapter5/nagios-3x.html)をベースに、Opsviewのパッチとの競合が無いようにしたものです。
ももーいさん、ありがとうございます。

opsview-base-3.11.1.5817-1.ct5.JP.src.rpm
-----------------------------------------

RPMで利用される場合は、このSRPMを利用してRPMを作成して本家のopsview-baseの代わりにインストールすることで、Nagiosが日本語化された状態になります。
合わせてja.poを配置してください。
