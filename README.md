# onscripter
fork of http://onscripter.osdn.jp/onscripter.html

ONScripter

0. はじめに

	高橋直樹氏作の NScripter 用に作成されたスクリプトを独自に解釈して実行します。


1. 動作環境

	libjpeg 6b, bzip2-1.0.6, SDL-1.2.15, SDL_image-1.2.12, SDL_mixer-1.2.12, SDL_ttf-2.0.11, 及び SMPEG-0.4.5 が動作する環境です。
	Linux 4.9.6 + Xvnc4 + g++ (gcc 6.3.0) で開発しています。
	Linux, Windows 8 (Visual Studio 2017 C++), Xperia (Android 8.0.0), iPad2 Air (iOS 12.1) 上で動作確認をしています。
	その他、MacOS X, MacOS 9, Android(Nexus One, Emulator), iPhone, iPad, PSP, FreeBSD, Solaris(on SPARC), Tru64 UNIX, OS/Warp, iPod, PocketPC, Playstation3, Wii, GP2X, NetWalker, Dreamcast 上での動作報告をいただいています。


2. コンパイル・起動方法

	コンパイル・起動方法は以下の通りです。
	ただし、onscripter を実行する場所に default.ttf, スクリプト, アーカイブがなければいけません。
	詳しくは同梱の www/onscripter.html を参照してください。

	Linux もしくは FreeBSD, Solaris の場合
	$ make -f Makefile.Linux
	$ onscripter

	Windows の場合 (DOS プロンプトで)
	$ https://onscripter.osdn.jp/win/ を参考に SDL, SDL_image, SDL_mixer, SDL_ttf, smpeg, Lua, bzip2 をインストールしてください。
	$ ONScripter.sln を Visual Studio で開いてビルドしてください。
	$ onscripter.exe

	MacOS X の場合
	$ make -f Makefile.MacOSX
	$ onscripter

	Zaurus (SL-5500, SL-A300, SL-B500, SL-C700) の場合
	別のマシン(Linux 等)上でクロスコンパイル
	$ make -f Makefile.ARMLinux
	Zaurus の Qtopia 上から実行
	$ onscripter

	それ以外のプラットフォームでは、Makefile.Linux を雛形にして Makefile.### を作ってください。

	ONScripter は、カレントディレクトリの 0.txt もしくは nscript.dat を自動的に読み込み、それにしたがってカレントディレクトリの arc.sar もしくは arc.nsa を読み込みます。


3. 連絡先

	本ソフトウェアに関する問い合わせは

	ogapee@aqua.dti2.ne.jp

	まで電子メールにてお願いします。
