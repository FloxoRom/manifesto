## LAST Update : 2023-02-24, Security Patch : 2023-02-05
* [FlokoROM v4(unofficial,Android 11.0) is available.](https://github.com/FloxoRom/manifesto/tree/11.0)

## FlokoROMを継承したカスタムROM
開発終了となったFlokoROMと同等の特徴を持ったカスタムROMです。
[crDroid](https://crdroid.net/)をベースに、いくつかの変更が加えられています。[詳しくはこちら](https://wiki.maud.io/ja/floko/v4)  
様々な環境でテストしている訳ではないので未知のバグを含む可能性があります。  
OmniSwitchは動作不能なので消しました

### 将来的な予定
* ROMの名称変更(継承しているとはいえ非公式であるため)

### 既知の問題点
* 

### 連絡先
Cugryが管理しています。何かあれば以下へ
* [Twitter](https://twitter.com/Cugry)
* [Github](https://github.com/Cugry)
* Discord : Cugry#6038
## 以下コピペ

## How to build

### Basic

Read:

* [AOSP Guide](https://source.android.com/setup/build/requirements)
* [LineageOS wiki](https://wiki.lineageos.org/devices/kebab/build)

### Download the sources

Initialize repo:

```sh
repo init -u https://github.com/FloxoRom/manifesto.git -b 12.1 --git-lfs
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
