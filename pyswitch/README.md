# PySwitch

PySwitch 是一个为 Windows 安装了多个 Python 环境提供快速切换的软件。

## 使用

### 使用帮助

您在首次运行 pys 时，请先进行初始化（双击软件/pys --init），然后添加 Python 环境（使用 pys -a version=path）。
接着您就可以使用 pys 在 windows 上愉快的切换 Python 环境了。


### 参数文档

> -h/--help       : 使用帮助
> 
> -v/--version    : 软件版本信息
> 
> -a/--add        : 添加 Python 环境（version=path）
> 
> -r/--remove     : 删除 Python 环境 (version)
> 
> -u/--use        : 切换系统运行 Python 环境
> 
> --init          : 初始化
> 
> --py-version    : 当前系统运行 Python 版本 

### 使用范例
```bash
python pys.py -u 3.7.2
```

* **注意：**需要以管理员权限运行

## config.conf
* env_path  ：pys.exe 所在目录
* [py_envs] ：py_envs 为电脑所安装的 python 环境（版本 = 安装路径）

## 编译 exe
1. 安装 pyinstaller （pip install pyinstaller）
2. 编译 pyinstaller -F -c -i favicon.ico pys.py

## pys.exe 安装
1. 下载 pys.exe 文件到本地
2. 双击 pys.exe 进行初始化
3. 添加已经安装 Python 环境
4. 为 pys.exe 添加管理员权限，属性 -> 兼容性 -> 以管理员身份运动

![添加管理员权限](./images/set_admin.png)

## pys.exe 使用

```bash
pys -u 3.7.2
```