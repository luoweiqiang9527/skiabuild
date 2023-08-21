# 自动构建Skia

本仓库致力于构建用于[Skija](https://github.com/HumbleUI/Skija)的二进制文件。

## 预先构建的二进制文件

预构建的二进制文件可以在 [发布版](https://github.com/HumbleUI/SkiaBuild/releases)中找到。

## 构建下一个版本的Skia

更新[.github/workflows/build.yml](https://github.com/HumbleUI/SkiaBuild/blob/master/.github/workflows/build.yml)中的`version`.

## 本地构建

```sh
python3 script/checkout.py --version m91-b99622c05a
python3 script/build.py
python3 script/archive.py
```

构建调试版本:

```sh
python3 script/checkout.py --version m91-b99622c05a
python3 script/build.py --build-type Debug
python3 script/archive.py --build-type Debug
```