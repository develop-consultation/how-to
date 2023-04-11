# Dockerインストール

## 前提条件
* OSはWindows11

## 1. Windos機能有効化
Windowsの機能の有効化または無効化を開く  
* 以下機能にチェックをつける  
  * Hyper-v  
  * Linux用Windowsサブシステム  
  * 仮想マシンプラットフォーム  
![Windowsの機能①](images/Windowsの機能①.png)  
![Windowsの機能②](images/Windowsの機能②.png)

OKボタン押下後、再起動  

## 2. Dockeデスクトップインストール
[Dockerデスクトップ](https://www.docker.com/products/docker-desktop/)よりダウンロード及びインストール  
![Dockerデスクトップダウンロード](images/Dockerデスクトップダウンロード.png)

## 3. Linuxカーネル更新プログラムパッケージ
[Linuxカーネル更新プログラムパッケージ](https://learn.microsoft.com/ja-jp/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package)よりダウンロード及びインストール  
![Linuxカーネル更新プログラムパッケージ](images/Linuxカーネル更新プログラムパッケージ.png)

## 4. Linux ディストリビューションのインストール
**PowerShellを管理者権限で開き実行すること**

### 4.1. 一覧取得
```
wsl --list --online
```

### 4.2. インストール
```
wsl --install -d Ubuntu-20.04
```  
![ディストリビューションのインストール](images/Linux ディストリビューションのインストール.png)  

### 4.3. ユーザ名とパスワードを設定  
Ubuntuインストール後、ユーザー設定画面が開くのでそのまま設定する  
![ユーザ名とパスワードを設定](images/ユーザ名とパスワードを設定.png)  

### 4.4. デフォルトのディストリビューションを変更  
インストール済みのディストリビューション一覧表示
```
wsl -l -v
```
デフォルトのディストリビューションを変更  

```
wsl -s Ubuntu-20.04
```
![デフォルトのディストリビューションを変更](images/デフォルトのディストリビューションを変更.png)

## 5. wsl2上でのdocker使用

### 事前準備  
エクスプローラーでubuntuのディレクトリにアクセスできるか確認
```
\\wsl$\Ubuntu-20.04
```
![wsl2上でのdocker使用事前準備](images/wsl2上でのdocker使用事前準備.png)  
Dockerデスクトップ起動  
設定画面で「Use the WSL2 based engine」が有効になっていることを確認  
![wsl2の使用①](images/wsl2の使用①.png)  
そのあと「Resources」-「WSL INTEGRATION」を選択し、<br>「Enables integration with additional distros:」以下に表示されているLinuxからDockerを使用するものの設定を有効にし、<br>「Apply & Restart」ボタン押下  
![wsl2の使用②](images/wsl2の使用②.png)  
以下コマンドをディストリビューション上で実行して**Dockerコマンド**が使えることを確認  
![wsl2の使用③](images/wsl2の使用③.png)
