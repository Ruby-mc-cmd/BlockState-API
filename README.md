# Minecraft Java Datapack用ブロック情報取得ライブラリ

ブロックの情報を取得し、`storage`の`yrh.blockstate` に保存するためのライブラリです。

## 使用方法

取得したいブロックの座標で以下の関数を実行します。

### 1. BlockStateを取得
```mcfunction
#yrh.blockstate:blockstate
```
ブロックの状態 (`age` や `attached` などの BlockState) を取得します。

### 2. NBTデータを取得
```mcfunction
#yrh.blockstate:data
```
ブロックの NBT データを取得します。

### 3. BlockIDを取得
```mcfunction
#yrh.blockstate:id
```
ブロックの ID を取得します。

### 4. 上記すべてをまとめて実行
```mcfunction
#yrh.blockstate:all
```
- BlockState、NBTデータ、BlockID をまとめて取得します。
- 座標指定一回ですべての情報を `storage` に保存可能です。

## 補足
- `storage` は任意のデータ名に変更可能  
- 必要に応じて関数を組み合わせて、効率的にブロック情報を管理できます
