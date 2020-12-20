# navigation.reg
**よくわからずに使うとパソコンが壊れる可能性があります。**  
windowsのエクスプローラのレジストリの設定。  
レジストリを書き換えるたPCが壊れる可能性があります（UUIDの重複が起こったときくらいだろうど→そんなことあるの？）。
PC壊れるのが怖かったらレジストリエディタ使って一つ一つ追加するのがいいと思う。

## Download
UUID: 10A8FB89-C66C-B776-65FE-943BDA2BF8AB
### 追加方法
1. `Download.reg`内のファイルパスを書き換え。
> `C:\\Users\\user\\icon\\download.ico`はアイコンファイルの場所に書き換え。  
> `C:\\Users\\user\\Downloads`は自分のダウンロードフォルダに書き換え。
1. `Download.reg`をダブルクリック。

### 削除方法
1. `Download - Remove.reg`をダブルクリック。

## 情報まとめ
間違ってる情報があるかもしれません。
### HKEY_CURRENT_USER\Software\Classes\Wow6432Node\CLSID
32bitアプリケーション用？
> 使わなさそうだから消した。`HKEY_CURRENT_USER\Software\Classes\CLSID`と内容は多分同じ。
### HKEY_CURRENT_USER\Software\Classes\CLSID
呼び出すための情報が入っている？パスとか。

### HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\HideDesktopIcons\NewStartPanel
デスクトップにどのアプリケーションのアイコンを表示するかを設定している。0が表示、1が非表示っぽい。
> ここ書き換えるとゴミ箱とか消せる。

### HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\Desktop\NameSpace
アプリケーションの名前？どこで使用しているのかは不明。
