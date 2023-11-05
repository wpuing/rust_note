**参考链接****：**

* 安装：[https://juejin.cn/post/7263731372606832697](https://juejin.cn/post/7263731372606832697)
* vs插件：[https://visualstudio.microsoft.com/zh-hans/visual-cpp-build-tools/](https://visualstudio.microsoft.com/zh-hans/visual-cpp-build-tools/)
**1.配置环境变量**

需要配置两个环境变量 **RUSTUP_HOME** **CARGO_HOME**，用于自定义安装位置，官方推荐的安装方式默认安装在C盘，个人觉得不是灵活（占地方）,配置这两个参数后可以自定义安装位置，为后续的版本升级等提供便利

* **RUSTUP_HOME（****设置rustup的安装路径****）**
  ![图片](D:\code\rust\rust_note\img\install\rustup_home.png)


* **CARGO_HOME（****设置cargo的安装路径****）**
  ![图片](D:\code\rust\rust_note\img\install\cargo_home.png)


**2.下载安装包**

* **注意：**
部分电脑可能会存在vs插件未存在，建议先下载插件，然后傻瓜式安装

* **访问官网（中文网）：**[https://www.rust-lang.org/zh-CN/tools/install](https://www.rust-lang.org/zh-CN/tools/install)
  ![图片](D:\code\rust\rust_note\img\install\official_website.png)


下载之后的得到一个文件：rustup-init.exe

**3.安装**

* **环境检测警告**
  ![图片](D:\code\rust\rust_note\img\install\wrn.png)


如果已安装插件，则不管他，直接输入 **y**

* **选择安装方式**
  ![图片](D:\code\rust\rust_note\img\install\insta_mdth.png)


安装器安装之前后检测系统配置，是否已存在所需的环境变量，如图，由于已经配置过之后会显示出环境变量；安装前让用户选择安装方式

1）继续安装（默认）

2）自定义安装

3）取消安装

选择输入 **2**

* **配置选择**
  ![图片](D:\code\rust\rust_note\img\install\choice-01.png)


默认的是msvc,这边选择安装gnu, 可以使用Debug模式进行调试。

选择输入：**x86_64-pc-windows-gnu**

![图片](D:\code\rust\rust_note\img\install\choice-02.png)


是否选择默认的工具，回车选择默认 **stable**

![图片](D:\code\rust\rust_note\img\install\choice-03.png)


是否选择其他的工具和配置，回车选择默认 **default**

![图片](D:\code\rust\rust_note\img\install\choice-04.png)


是否修改环境变量 path, 选择输入 **y**

![图片](D:\code\rust\rust_note\img\install\choice-05.png)


提供其他的安装

1）继续安装 （默认）

2）自定义安装

3）退出安装

可以看出，上面的默认信息已经设置为我们所需要的gnu、stable等配置信息，所以，这时候选择继续安装，选择输入 **1**

![图片](D:\code\rust\rust_note\img\install\choice-06.png)


继续安装之后，直接等待自动下载所需的各种配置、工具等。当出现

**Rust is installed noe. Great!**

则表示安装成功！

**4.验证**

* **rustc**
```plain
rustc --version
```

![图片](D:\code\rust\rust_note\img\install\check-01.png)


* **cargo**
```plain
cargo --version
```

![图片](D:\code\rust\rust_note\img\install\check-02.png)


输入命令后出现版本信息则表示安装成功！




