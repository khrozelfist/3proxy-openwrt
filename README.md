###### Update the PKG_VERSION and PKG_SOURCE_VERSION from
https://github.com/3proxy/3proxy

Compile 3proxy with [openwrt-ci.yml](https://github.com/KFERMercer/OpenWrt-CI/blob/master/openwrt-ci.yml)
===
Add the following line above [Space cleanup](https://github.com/KFERMercer/OpenWrt-CI/blob/master/openwrt-ci.yml#L38)
```bash
- name: Git Clone
        run: |
          git clone https://github.com/khrozelfist/3proxy-openwrt feeds/packages/net/3proxy
```
Add the following line into [Generate configuration file](https://github.com/KFERMercer/OpenWrt-CI/blob/master/openwrt-ci.yml#L72)
```
          CONFIG_PACKAGE_3proxy=y
```
