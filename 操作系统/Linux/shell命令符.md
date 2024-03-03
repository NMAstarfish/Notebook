# 格式
`command [-options] [parameter]
命令  命令选项【可选】 命令参数【可选】

# 路径
`./`  表示相对路径
`..`  表示上一级路径
`-`  表示上一个路径

# 常用命令
pwd ：显示当前目录
ls ：显示当前目录下文件
cd ：切换路径
cd.. ：返回上一级路径
mkdir ：新建目录
rmdir ：删除目录
touch ：新建文件
cp ：复制文件
rm ：删除文件
cat ：将文件内容显示到终端
clear ：清除屏幕内容


# 权限
可以使用a,u,g,o指定给什么用户修改权限

# 压缩和解压(gzip,bzip,tar)

## gzip
查看压缩文件:
$ gzip -l pwd.1.gz 
解压文件:
$ gzip -kd pwd.1.gz   //该压缩文件是以.gz结尾的单个文件 
压缩文件:
$ gzip -k mypwd.1   //得到了一个.gz结尾的压缩文件


tar 常用选项： 
⚫ -c(create)：表示创建用来生成文件包 。 
⚫ -x：表示提取，从文件包中提取文件。 
⚫ -t：可以查看压缩的文件。 
⚫ -z：使用 gzip 方式进行处理，它与”c“结合就表示压缩，与”x“结合就表示解压缩。 
⚫ -j：使用bzip2方式进行处理，它与”c“结合就表示压缩，与”x“结合就表示解压缩。 
⚫ -v(verbose)：详细报告tar处理的信息。 
⚫ -f(file)：表示文件，后面接着一个文件名。 -C <指定目录> 解压到指定目录。

把目录dira压缩、打包为dira.tar.bz2文件: 
$ tar cjvf dira.tar.bz2 dira