# Python_Lectures
A (very) Brief Introduction to Python3
---

## 需要安装的软件和一些基本设置:
- 安装 Anaconda3
- 设置 Jupyter notebook 的默认打开位置

### 安装 Anaconda3
1. 下载 Anaconda3
    - 官方网站： https://www.anaconda.com/download/

    如果下载速率过于慢，请移步国内镜像地址下载：
    - 中国科学技术大学镜像站： https://mirrors.ustc.edu.cn/anaconda/archive/
    - 清华大学镜像站：https://mirrors.tuna.tsinghua.edu.cn/help/anaconda/

  打开连接之后，最后一项是对应的最新版本的`Anaconda3`，**请注意** 安装文件对应的系统（`Linux`，`Mac`, `Windows`）以及相应的`32位`还是`64位`版本。


2. 安装 Anaconda3
Windows系统用户直接双击下载后的 `.exe`文件，用管理员身份运行。一路点`Next`即可。

【建议】可以不安装在 C 盘，建议安装在一个相对较大的磁盘分区里，比如 `D:\anaconda3`。

### 设置 Jupyter notebook 的默认打开位置
1. Windows系统用户，请在 `https://github.com/LePingKYXK/Python_Lectures` 连接上点击`Clone or download`按钮，然后再点击`Download ZIP`，即可下载此教程的所有（压缩格式）文件。将其解压到一个文件夹里。

2. 鼠标双击 `Anaconda Prompt`，打开命令行，输入 `jupyter notebook --generate-config` 命令。
这行命令会在 `C:\Users\[YOUR_NAME]\.jupyter`目录下，产生一个 `jupyter_notebook_config.py` 文件。
如果你用的是`中文版 Windows`系统，请点击 `C盘`-->`用户`-->`[你的名字]`-->`.jupyter`，找到 `jupyter_notebook_config.py` 文件。

3. 用 `Notepad++` 打开此文件，搜索找到如下行：
```python
## The directory to use for notebooks and kernels.
#c.NotebookApp.notebook_dir = ' '
```
修改成：
```python
## The directory to use for notebooks and kernels.
c.NotebookApp.notebook_dir = '你的硬盘目录'
```
- **【注意】 请去掉 c.NotebookApp.notebook_dir 这一行前面的 # 号；**
- **【注意】 这里“你的硬盘目录”可以是你存放文件的任何目录，只要你方便找到就好；**
- **【注意】 c.NotebookApp.notebook_dir = '你的硬盘目录' 单引号不要删除。**

更多参数的设置请看官方连接： https://jupyter-notebook.readthedocs.io/en/stable/config.html

4. 将第 1 步中解压的教程文件夹放在第 3 步 **你的硬盘目录** 下面

5. 在 `Anaconda Prompt`命令行中输入`jupyter notebook`，即可运行 `Jupyter notebook`。它会在你的浏览器中打开。你可以看到打开的页面就是你刚刚在第 3 步设置的目录位置。

6. 用鼠标双击此教程的 `Introduction_to_Python3.ipynb` 文件，即可在浏览器中打开并运行。
