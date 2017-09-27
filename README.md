# antd
antd学习



###解决create-react-app慢(失败)方法
>解决方案是换源.
虽然平常使用cnpm来代替npm,但也只是使用新的指令而已，而在寻求create-react-app的相关配置希望修改registry时失败了，最后发现create-react-app指令默认调用npm，于是直接把npm的register给永久设置过来就好了，这样使用cnpm或者npm就没差别了。
```
npm config set registry https://registry.npm.taobao.org
-- 配置后可通过下面方式来验证是否成功
npm config get registry
-- 或npm info express
```
