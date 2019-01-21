# img_decide

Decide The Image By Model

学習モデルをもとに画像ファイルから特定の顔を認識します。

事前に OpenCV の haarcascade_frontalface_default.xml を用意しておくこと。

## 環境

* Windows 10 x64 1809
* Python 3.6.5 x64
* Power Shell 6 x64
* Visual Studio Code x64
* Git for Windows x64

## 構築

プロジェクトを clone してディレクトリに移動します。

```powershell
> git clone https://github.com/kerobot/img_decide.git img_decide
> cd img_decide
```

プロジェクトのための仮想環境を作成して有効化します。

```powershell
> python -m venv venv
> .\venv\Scripts\activate.ps1
```

念のため、仮想環境の pip をアップグレードします。

```powershell
> python -m pip install --upgrade pip
```

依存するパッケージをインストールします。

```powershell
> pip install -r requirements.txt
```

環境変数を設定します。

> CASCADE_FILE_PATHを設定

```powershell
> copy .\.env.sample .\.env
> code .\.env
```

## 実行

modelディレクトリにモデルファイルを配置し、判定する画像ファイルを指定して実行します。

> 判定結果の表示

```powershell
> python .\img_decide.py "./origin_image/画像ファイル.jpg"
```
