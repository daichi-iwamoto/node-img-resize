# node-img-resize
nodeで画像をリサイズするモジュール
`src/img`ディレクトリにある画像を一括でリサイズできます

## 使用方法

### 1.clone
このリポジトリを任意のディレクトリに`clone`してきてください

### 2.モジュールインストール（初回時のみ）
```bash= 
npm install 
```

### 3.リサイズしたい画像を設置
リサイズしたい画像を`/src/img/`に入れてください

### 4.コマンドを実行
コマンドに引数を渡すことでサイズを指定します

#### 横幅を指定して縦横比固定リサイズ
横幅を指定する場合は引数に`w`と、横幅のサイズ(px)を指定してください
下記は横幅`180px`でリサイズしたい場合のコマンドです
```bash= 
# 横幅:180px, 縦幅:auto
npm run resize w 180
```

#### 縦幅を指定して縦横比固定リサイズ
縦幅を指定する場合は引数に`h`と、縦幅のサイズ(px)を指定してください
下記は縦幅`100px`でリサイズしたい場合のコマンドです
```bash= 
# 横幅:auto, 縦幅:100px
npm run resize h 100
```

#### 縦・横幅を指定してリサイズ
縦・横幅を指定する場合は引数に`wh`と、サイズ(px)を指定してください
下記は横幅`180px` 縦幅`100px`でリサイズしたい場合のコマンドです
```bash= 
# 横幅:180px, 縦幅:100px
npm run resize wh 180 100
```

`/dist/img/`にリサイズされた画像が出力されます
