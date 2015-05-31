# inject\_classes v1.0 #
2012-10-24

将自己写的class混编(注入)到需要反编译的apk(mix/inject classes2apk)

功能

---

  1. 将自己写的class文件变成android的dex格式
  1. 将dex格式反编译为smali代码
  1. 合并这些smali代码到apk反编译的smali目录

使用方法

---

`_inject_classes {class目录} {apk反编译的smali目录}`

例如:
```
_inject_classes D:\TestSmaliInject\build\classes D:\TestSmali\smali
```

# onekey-decompile-apk v1.0.1 #
2012-10-22

将apktool降到1.4.1(原来是1.4.3), 只有这个版本能进行SmaliDebugging http://d-kovalenko.blogspot.com/2012/08/debugging-smali-code-with-apk-tool-and.html

# build\_sign\_install v1.0 #
2012-10-22

一步到位打包apk(签名, 安装)工具(onekey build-sign-install apk)

功能

---

  1. 打包apktool反编译出来的文件为apk
  1. 通过d2j-apk-sign签名apk
  1. adb install签名后的apk

使用方法

---

`_build_sign_install {apktool反编译输出的文件夹位置}`

例如:
```
_build_sign_install myapp
```