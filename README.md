<div align="center">

# apt-from-url

URLで指定したdebファイルをインストールできる、aptラッパー

<br>
<br>
</div>

## ⬇️ インストール
```bash
sudo curl -L "https://raw.githubusercontent.com/PenguinCabinet/apt-from-url/main/apt-from-url" | sudo tee /usr/local/bin/apt-from-url 
```
```bash
sudo chmod +x /usr/local/bin/apt-from-url
```

### 依存関係
* curl
* apt

## 🔨 使い方
`/tmp`ディレクトリにdebファイルをダウンロードし、`apt install -f`でインストールします。
```bash
sudo apt-from-url install "https://example.com/package.deb"
```

第三コマンドライン引数以降は展開され、aptに渡されます。
```bash
sudo apt-from-url install "https://example.com/package.deb" -y
```

install以外のコマンドも使用できます
```bash
sudo apt-from-url reinstall "https://example.com/package.deb"
```

## 🎫 LICENSE

[MIT](./LICENSE)

## ✍ Author

[PenguinCabinet](https://github.com/PenguinCabinet)
