# Termux Extras
## About
This repo has some software not available in the Termux's official repository. All of them are compiled and packaged by me.
## Install
Create `sources.list.d` directory if it does not exist
```
mkdir $PREFIX/etc/apt/sources.list.d
```
Add the apt Repository
```
echo "deb [trusted=yes] https://termux-extras.iamsjy.com termux extras" > $PREFIX/etc/apt/sources.list.d/termux-extras.list
```
Update apt source lists
```
apt update
```
## Remove
Execute the command below to remove the apt repository.
```
$PREFIX/etc/apt/sources.list.d/termux-extras.list
```

## Note
`[trusted=yes]` is not needed if the repo has been signed with a gpg key
