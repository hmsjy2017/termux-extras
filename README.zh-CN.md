# Termux Extras
  语言：简体中文 | [English](README.md)
## 关于
Termux 并非 Linux 环境，Linux arm64 软件不能在 Termux 上正常运行，重新编译才能使用。这个存储库里有一些我为 Termux 适配的软件。
## 安装
- 如果 `sources.list.d` 目录不存在，则创建它：
```
mkdir $PREFIX/etc/apt/sources.list.d
```
- 添加 apt 存储库
```
echo "deb [trusted=yes] https://termux-extras.iamsjy.com termux extras" > $PREFIX/etc/apt/sources.list.d/termux-extras.list

对于中国大陆用户，推荐使用速度更快的节点：
echo "deb [trusted=yes] https://public.sourcegcdn.com/tony/termux-extras termux extras" > $PREFIX/etc/apt/sources.list.d/termux-extras.list
```
- 更新 apt 源列表
```
apt update
```
## 卸载
执行以下命令：
```
rm $PREFIX/etc/apt/sources.list.d/termux-extras.list
```

## 注意
如果 apt 存储库没有用 gpg 密钥签名，必须添加 `[trusted=yes]` 来信任存储库才能使用。
