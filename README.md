# IMPORTANT : This is Unofficial Project.

## LAST Update : 2022-10-17, Security Patch : 2022-10-05

![FlokoROM](https://lindwurm.neocities.org/img/floko/flokowall_v4_mini.png)

# How to build

## Basic

Read:

* [AOSP Guide](https://source.android.com/setup/build/requirements)
* [LineageOS wiki](https://wiki.lineageos.org/devices/kebab/build)

## Download the sources

Initialize repo:

```sh
repo init -u https://github.com/Cugry/manifesto.git -b 11.0
```

Sync(Download):

```sh
repo sync -j$(nproc) -c --no-clone-bundle --no-tags
```

## Build

```sh
export ALLOW_MISSING_DEPENDENCIES=true
```

```sh
. build/envsetup.sh
```

```sh
brunch <device> 2>&1 | tee ~/log/floko_$(date '+%Y%m%d_%H-%M-%S').log
```
