## wavely
### nuclei模版管理工具
由于没找到一款比较好用的poc管理器，，便自己开发了这个，目前仅提供安装包下载。


![main](imgs/1.png)
### ✨ 功能
- [x] 实现 `nuclei` `poc` 管理的桌面应用，对 `nuclei` 模版的增删查改操作
- [x] 支持 `nuclei` 扫描
- [x] 实现多任务、并行扫描
- [x] 查看 `nuclei` 模版请求响应包
- [x] 支持自定义 `nuclei` `DNSLOG` 服务器
- [x] 支持自定义扫描速率
- [x] 支持`http代理`（http、https、socks5）
- [x] 支持`MacOS`、`Windows`和`Linux`操作系统
- [x] 使用全新`nuclei v3`检测引擎
- [x] 兼容`yamlv2`和`yamlv3` nuclei template
- [x] 支持主题切换
- [x] 支持多种 `nuclei` 模版导入方式
- [x] 支持 `nuclei` 模版去重导入
- [x] 基本支持国际化【简体中文/英文】
- [x] 扫描任务停止功能
- [x] 支持配置持久化
- [x] 支持api扫描
## 安装
#### MacOS
1. 下载相应压缩包并解压，解压文件夹中包含 `Wavely.app`和 `Applications文件夹`。
2. 将`Wavely.app`拖到`Applications文件夹`中
3. 终端执行:`sudo xattr -d com.apple.quarantine /Applications/Wavely.app`

#### Windows

##### 安装程序安装
-  使用 `Wavely-amd64-installer.exe.zip`
##### 手动安装
-  下载`Wavely_1.5.4_windows_amd64.exe
`文件，得到exe文件，保存到自定义文件夹中即可。

## 快速使用
#### POC导入
##### 在App中导入POC（带POC去重）
- 点击`从文件夹中导入`按钮，选择`nuclei poc文件目录`。

![alt text](imgs/14.png)

> 也可支持手动导入POC（不带POC去重）【不建议使用】
> 1. 打开 `Wavely`，将初始化数据库和poc配置目录。
> 2. 将nuclei poc文件复制到以下文件夹中：
    - **MacOS**：/Users/$USER/.wavely/templates
    - **Windows**：.wavely/templates
> 3. 打开 `Wavely`，进入**设置**->**模版**->点击**更新按钮图标**。
![main](imgs/13.png)


#### 功能展示
##### 模版管理

![main](imgs/1.png)
##### 扫描任务
- 选择thinkphp的poc进行扫描

![main](imgs/2.png)
##### 扫描结果
- 扫描结果
- 可复制扫描结果

![main](imgs/3.png)


####  编辑nuclie模版
- 编辑模版

![main](imgs/8.png)

- 匹配请求包（需扫描匹配POC成功时才可看到请求响应包）

![main](imgs/9.png)

- 匹配响应包（需扫描匹配POC成功时才可看到请求响应包）

![main](imgs/10.png)

#### 添加Nuclei模版
![main](imgs/11.png)

#### App设置
- 切换POC编辑器主题

![main](imgs/4.png)

- 添加HTTP代理

![main](imgs/5.png)

- POC扫描参数设置

![main](imgs/6.png)

- 模版导入功能

![main](imgs/7.png)

### 常见问题
##### Windows启动时闪现弹出命令框
为正常现象，不影响App的功能
#####  Macos 无法打开App
由于没有使用apple证书签名app，可能会提示解除安全验证：`软件显示禁止符号` 或 `无法验证软件身份` 或 `提示已损坏故不能正常打开`，请参考：

##### 方案1
执行如下命令即可：
``` bash
sudo xattr -d com.apple.quarantine Applications/Wavely.app
```
##### 方案2
``` bash
chmod 755 /Users/$USER/Desktop/Wavely_darwin_arm64_1.5.2.app/Contents/MacOS/Wavely
```

# 免责声明
本工具仅面向合法授权的企业安全建设行为，如您需要测试本工具的可用性，请自行搭建靶机环境。 为避免被恶意使用，本项目所有收录的poc均为漏洞的理论判断，不存在漏洞利用过程，不会对目标发起真实攻击和漏洞利用。 在使用本工具进行检测时，您应确保该行为符合当地的法律法规，并且已经取得了足够的授权。请勿对非授权目标进行扫描。 如您在使用本工具的过程中存在任何非法行为，您需自行承担相应后果，我们将不承担任何法律及连带责任。

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=perlh/wavely&type=Date)](https://star-history.com/#perlh/wavely&Date)

# 捐赠
如果 Wavely 对您帮助很大，您可以通过以下方式支持我们：

### 赞赏码赞助
![main](imgs/sponsor.jpg)