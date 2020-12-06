# mkmydist
現在のxfce環境をインストールディスク&ライブ環境化します

## 注意
PinguyBuilderでは個人情報等のファイルが残る可能性が高いので **ディストーションとしての配布には向きません**

## 必要なパッケージ
PinguyBuilderがインストールされている必要があります。　

### ubuntu20.04の場合、依存関係をさらに取得する必要があります
PinguyBuilderに必要なxresprobeのダウンロード

 <https://launchpad.net/ubuntu/+source/xresprobe/0.4.24ubuntu9/+build/1274262/+files/xresprobe_0.4.24ubuntu9_amd64.deb>
 
PinguyBuilderのダウンロード

<https://sourceforge.net/projects/pinguy-os/files/ISO_Builder/pinguybuilder_5.2-1_all.deb/download>


## 使い方
`bash ./makemy-dist.sh`　　
でスクリプトを実行します。あとは自動的に設定ファイルのコピー、クリーンアップ、iso生成を実行します。予めOSの名前を変更してください。完成すると/home/PinguyBuilder/PinguyBuilderディレクトリ内にisoファイルがあります

### OS名の変更方法
`/usr/lib/os-release`
上記のパスにあるファイルの `PRETTY_NAME` の項目を自分のOSの名前に変更します。それ以外の場所を変えると正常に作動しなくなる可能性があるので注意して下さい。
