# awkのメモ

### 基本

### 正規表現でマッチング 

まず、以下のようにしてファイルを作成する

> $ cat > file
> あいうえお
> かきくけこ
> さしすせそ
> たちつてと

このファイルのうち"あ"もしくは"さ"で始まる行のみ出力する

> $ cat file | awk '/^[あか]./'
> あいうえお
　かきくけこ
