# 自動応援ツール
このツールは自社の採用を応援したいと思いつつなかなか毎日画面開いてボタンを押すオペレーションをこなすことができない人に、
快適に応援をしてもらうためのツールです。

## 利用方法
### 簡易版
1. [recruiting-supporter](https://github.com/yohei-takeda/recruitment-supporter/raw/master/recruiting-supporter) をダウンロード
2. 以下実行：
```
// to authenticate using facebook account, parameter "signin_method" should be "facebook". Otherwise, keep it empty.
./recruiting-supporter <recruitment_page_url> <company_name> <userId> <password> <signin_method>
```

### ソースからコンパイル
1. Goをインストール (http://golang.jp/install 参照)
2. webdriver, 必要なgoライブラリをインストール
webdriver(今はchromeのみサポートです）：
```
# for mac
brew tap homebrew/cask
brew cask install chromedriver
```
agoutiをインストール
```
go get github.com/sclevine/agouti
```
3. ファイルを実行
//TODO いずれもっと簡略に！
```
git clone https://github.com/yohei-takeda/recruitment-supporter.git
cd ./recruiting-supporter
go build
// to authenticate using facebook account, parameter "signin_method" should be "facebook". Otherwise, keep it empty.
./recruiting-supporter <recruitment_page_url> <company_name> <userId> <password> <signin_method>
```

### 参考：
https://qiita.com/0829/items/c1e494bb128ade5f0872
