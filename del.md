以下是整理好的Markdown格式内容：

Miniconda安装步骤
1. 创建安装目录
```bash
mkdir -p ~/miniconda3
```
2. 下载安装脚本
```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda3/miniconda.sh
```
3. 执行安装
```bash
bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
```
4. 清理安装脚本
```bash
rm ~/miniconda3/miniconda.sh
```

Conda环境管理命令
- 创建指定Python版本的虚拟环境
```bash
conda create -n 环境名称 python=版本号
```
- 查看环境状态
```bash
conda env status
```
- 列出所有虚拟环境
```bash
conda env list
```
- 删除指定虚拟环境
```bash
conda remove --name myenv --all
```

其他命令与路径说明
- 检查`librga.so`文件系统位置
```bash
可使用find命令查找
find / -name librga.so 2>/dev/null
```
- RKNN-Toolkit2相关路径
  - 示例路径：`~/work/test/rknn-toolkit2-1.5.2/examples/onnx/yolov5`
  - 根目录路径：`~/work/test/rknn-toolkit2-1.5.2`
- 安装依赖包
```bash
pip3 install -r doc/requirements_cp36-1.5.2.txt
```
- 配置交叉编译工具路径
```bash
export PATH=$PATH:/home/u3test3/work/gcc/gcc-linaro-7.5.0-2019.12-x86_64_aarch64-linux-gnu/bin/
```

如果需要进一步调整格式或补充内容，可以随时告诉我哦~<br><br>百度AI生成，内容仅供参考
