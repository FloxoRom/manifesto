## FlokoROMを継承したROM
基本的にはFlokoROMと同等の特徴を持ったカスタムROMです。
現在Alpha版であるため、後述の問題点含めその他未知のバグを含む可能性があります。

### 将来的な予定
* ROMの名称変更(継承しているとはいえ非公式であるため)

### 既知の問題点
* OmniSwitchが使用不可(設定から消えた)
* アプリの詳細画面がエラーで開けない

### 連絡先
Cugryが管理しています。何かあれば以下へ
* [Twitter](https://twitter.com/Cugry)
* [Github](https://github.com/Cugry)

## 以下コピペ

## How to build

### Basic

Read:

* [AOSP Guide](https://source.android.com/setup/build/requirements)
* [LineageOS wiki](https://wiki.lineageos.org/devices/kebab/build)

### Download the sources

Initialize repo:

```sh
repo init -u https://github.com/FloxoRom/manifesto.git -b 12.1
```

Sync(Download):

```sh
repo sync -j$(nproc) -c --no-clone-bundle --no-tags
```

### Build

```sh
export ALLOW_MISSING_DEPENDENCIES=true
```

```sh
. build/envsetup.sh
```

```sh
brunch <device> 2>&1 | tee ~/log/floko_$(date '+%Y%m%d_%H-%M-%S').log
```

## Contribute

To submit new features/patches, please send us a Pull Request on our GitHub. We will review and merge.
```sh
repo init -u https://github.com/FloxoROM/manifesto.git -b 12.1
```
