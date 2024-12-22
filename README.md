# Typora_Unlocker

进入[NodeInject](./NodeInject)编译

``` shell
cd ./NodeInject && cargo build
```

将编译后的可执行文件复制到typora文件夹下，并切换，执行复制的文件

```shell
sudo cp ~/.NodeInject/target/debug/node_inject /usr/share/typora/
sudo /usr/share/typora/node_inject
```

这里出现如下信息，则到目前为止，没有任何问题。

```shell
extracting node_modules.asar
adding hook.js
applying patch
packing node_modules.asar
done!
```

切换回 [license-gen](./license-gen)，生成license

```shell
cd ./license-gen/ && cargo build
./target/debug/license-gen
```

打开typora，输入邮箱和许可证。
幸运的话，就可以了。

***自用记录，如有侵权请联系删除***

该内容参考链接：
+ [https://github.com/L1ne-cd/Typora_Unlocker](https://github.com/L1ne-cd/Typora_Unlocker)
+ [https://github.com/DiamondHunters/NodeInject_Hook_example](https://github.com/DiamondHunters/NodeInject_Hook_example)
+ [https://github.com/DiamondHunters/NodeInject](https://github.com/DiamondHunters/NodeInject)
+ [https://seektao.cc/archives/typora-install-activation](https://seektao.cc/archives/typora-install-activation)
