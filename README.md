# Freeplane 思维导图模板
英语（English）：Freeplane-MindMap-Template

简体中文（Simplified Chinese）：Freeplane 思维导图模板

繁体中文（Traditional Chineses）：Freeplane 思維導圖模板

# 【思维导图软件】Freeplane 安装和简单模板制作教程

https://www.bilibili.com/video/BV1AZ4y1L7ky

# 【免费开源可商用】思维导图软件 Freeplane 常见问题解决方法（不定期更新）
https://www.bilibili.com/video/BV1Pa4y1s7P4

注：关于背景颜色问题，在Freeplane的菜单界面，依次点击工具→首选项→外观→取消勾选打印使用白色背景之后，再在Freeplane的思维导图界面上的空白处点击鼠标右键，弹出右键菜单后再点击背景颜色并选择自己喜欢的颜色即可。

# 如何反哺 Freeplane 这个开源项目

Freeplane的源码链接：

https://github.com/freeplane/freeplane

Freeplane的底层语言是Java，此外还有groovy和xslt，如果有朋友想参与到Freeplane的开发当中来，给Freeplane制作更多的图文、视频教程、模板甚至是追加新功能、重做界面的话。
可以先看Freeplane的源码，并针对xslt和groovy的相关手册制作思维导图，迅速纵览全局并定位，找到问题的入手点，提高开发效率。

# Freeplane 导出文件格式 备忘录
注：这么做主要是方便在多个软件和平台下使用

PNG的文本不可复制（废话）

PDF并不是所有字体（比如思源黑体、更纱黑体这类OpenType曲线的字体（不一定是otf格式，可以是OpenType曲线的ttf字体），不转曲的话，在导出时字形就会崩）都能导出字形正常的思维导图，因此需要转曲确保在不管用什么字体的情况下都能导出字形正常的思维导图。

更纱黑体 SC Semibold的替代解决方案见此处：

解决过程：https://github.com/be5invis/Sarasa-Gothic/issues/199

替代字体：https://github.com/Seekladoom/Freeplane-MindMap-Template/blob/main/%E5%AD%97%E4%BD%93%EF%BC%88Fonts%EF%BC%89/Sarasa%20Gothic%20PDF%20SC%20Semibold.ttf

在Windows系统下，如果要规避字体版权又想直接用系统自带字体确保他人也能正常显示的话，可以直接用黑体，即simhei，也就是中易黑体。


Freeplane导出时其他方便复制文字的文件格式，这里推荐几种：

TXT、HTML、SVG、DOC


Freeplane能导出的HTML有这几种，有兴趣的朋友可以自己导出试试，看哪种符合自己的需求：

HTML文档

导出为 Java Applet…

导出为 HTML

导出为XHTML（JavaScript版）…

导出为XHTML（可点击的映射图像版）…


# Freeplane实际使用时的一些细节记录
POSITION（只有改left和right有效，上下必须在相应地方写入相关功能才能实现）

贝赛尔曲线、水平直线（这俩的二级以及之后的节点间距形状跟Freeplane的子间隔参数有关）

节点形状选择【分叉、组合】时，第1层节点依然会保持对称，但第2层节点及之后的就做不到了；选择【气泡、椭圆形、矩形、宽六角形、狭窄六角形】，每级节点都能保持对称；选择【同父节点】时，每级节点都不能保持对称。

# Freeplane开发相关 1-3.txt
https://github.com/Seekladoom/Seekladoom-MindMap/blob/main/Freeolane%E5%BC%80%E5%8F%91%E7%9B%B8%E5%85%B3%201-3.txt


# 导出图片提示内存溢出的解决方法
当Freeplane制作的思维导图的篇幅太大，在导出jpg、png提示内存溢出时，可以试着导出pdf再用其他工具（比如pdf2png、Adobe Acrobat、福昕PDF等）转jpg、png。
