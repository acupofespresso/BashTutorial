# Bash 极简教程

## 1. 什么是 Bash？

Bash（Bourne Again Shell）是一种常见的 Linux 命令行解释器。

## 2. 基本命令

```bash
# 显示当前路径
pwd

# 列出文件和目录
ls

# 切换目录
cd 目录名

# 创建文件
touch 文件名

# 创建目录
mkdir 目录名

# 删除文件
rm 文件名

# 删除目录（包含内容）
rm -r 目录名

# 显示文件内容
cat 文件名

# 复制文件或目录
cp 源文件 目标文件
cp -r 源目录 目标目录

# 移动或重命名文件
mv 源文件 目标文件
```

## 3. 变量

```bash
# 赋值
name="张三"

# 输出变量
echo $name
```

## 4. 条件判断

```bash
if [ 条件 ]; then
    命令
elif [ 条件 ]; then
    命令
else
    命令
fi
```

示例：

```bash
if [ -f "test.txt" ]; then
    echo "文件存在"
else
    echo "文件不存在"
fi
```

## 5. 循环

```bash
# for 循环
for i in 1 2 3; do
    echo "第 $i 次"
done

# while 循环
count=1
while [ $count -le 3 ]; do
    echo "第 $count 次"
    count=$((count + 1))
done
```

## 6. 函数

```bash
function say_hello {
    echo "你好，$1"
}
say_hello "小白"
```

## 7. 运行 Bash 脚本

```bash
# 赋予脚本执行权限
chmod +x script.sh

# 运行脚本
./script.sh
```

## 8. 其他常用命令

```bash
# 查找文件
find /路径 -name "*.txt"

# 搜索文本内容
grep "关键字" 文件名

# 显示进程
ps aux

# 终止进程
kill 进程ID

# 显示磁盘使用情况
df -h

# 显示目录大小
du -sh 目录名
```

## 9. 结束语

这是一个极简的 Bash 入门教程，掌握这些内容，你就能写一些基本的 Bash 脚本了！
