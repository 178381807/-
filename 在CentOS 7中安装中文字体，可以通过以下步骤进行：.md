
在CentOS 7中安装中文字体，可以通过以下步骤进行：

1. 安装字体管理工具

```
yum install fontconfig mkfontscale
```

1. 创建中文字体目录

```
mkdir -p /usr/share/fonts/chinese
```

1. 将中文字体复制到中文字体目录

```
cp /path/to/chinese/fonts/* /usr/share/fonts/chinese
```

1. 生成字体索引

```
cd /usr/share/fonts/chinese
mkfontscale
mkfontdir
```

1. 刷新字体缓存

```
fc-cache -fv
```

在以上步骤中，`/path/to/chinese/fonts`是指中文字体文件所在的目录。可以将中文字体文件从Windows或其他操作系统中拷贝过来。

安装完成后，即可使用中文字体。