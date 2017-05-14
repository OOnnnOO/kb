# apt源的GPG公钥导入

sudo apt-get update 出错

```
W: GPG 错误：https://apt.proxy.oonnnoo.com jessie InRelease: 由于没有公钥，无法验证下列签名： NO_PUBKEY 14219A96E15E78F4
```

公钥导入

```
sudo apt-key adv --keyserver pgpkeys.mit.edu --recv-key 14219A96E15E78F4
```
