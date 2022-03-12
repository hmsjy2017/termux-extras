# Termux Extras
 Languages: [简体中文](README.zh-CN.md) | English
## About
This repo has some software not available in the Termux's official repository. All of them are compiled and packaged by me.
## Packages
- [ossutil](https://github.com/aliyun/ossutil) - A user friendly command line tool to access AliCloud OSS.
- [transfer](https://github.com/Mikubill/transfer) - Large file transfer tool with multiple file transfer services support
- [nali](https://github.com/zu1k/nali) - An offline tool for querying IP geographic information and CDN provider.
## Install
- Create `sources.list.d` directory if it does not exist
```
mkdir $PREFIX/etc/apt/sources.list.d
```
- Add the apt Repository
```
echo "deb [trusted=yes] https://termux-extras.iamsjy.com termux extras" > $PREFIX/etc/apt/sources.list.d/termux-extras.list

For Chinese users: 
echo "deb [trusted=yes] https://public.sourcegcdn.com/tony/termux-extras termux extras" > $PREFIX/etc/apt/sources.list.d/termux-extras.list
```
- Update apt source lists
```
apt update
```
## Remove
Execute the command below to remove the apt repository.
```
rm $PREFIX/etc/apt/sources.list.d/termux-extras.list
```

## Note
`[trusted=yes]` is needed if the repo hasn't been signed with a gpg key.
