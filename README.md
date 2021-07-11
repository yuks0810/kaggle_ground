# kaggle_ground
kaggleのコンペなどで使用する作業場所
[kaggle/python](https://hub.docker.com/r/kaggle/python)imageをdocker_hubから利用しているため、必要なライブラリはインストールされている。
常に`:latest`タグのimageを使用するようにdocker-compose.ymlで設定

## docker-compose コマンド使用する場合

```
$ docker-compose up -d --build
$ docker-compose exec jupyter bash
```
