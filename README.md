pdfAreaExtraction
=================

V 1.0 
------
功能
------
实现研报pdf文件中图片的截取，并且能够将图片信息（pdf名称，图片的title，资料来源）写入csv文件中

实现思路
-------
本次图片截取是先通过正则匹配的方式识别 图/表 数字 xxxxx 和 资料来源 xxxxxx 两行字符串，并且定位两行字符串在pdf中的文字坐标
然后通过Rectangle类截取文字坐标确定的矩形区域，即可得到图片，并且将相关信息写入csv文件

pdf格式要求
----------
pdf中的图片或表格 需要以：图/表/图表 的形式开始，资料来源部分得以：资料来源/资料/来源 的形式结束

效果展示
---------
#提取之后的全部文件夹<br>
![image](https://github.com/hooser/pdfAreaExtraction/blob/master/images/totalPackage.JPG)<br><br><br>
#单个文件夹内部<br>
![image](https://github.com/hooser/pdfAreaExtraction/blob/master/images/innerPackage.JPG)<br><br><br>
#原始的pdf页面<br>
![image](https://github.com/hooser/pdfAreaExtraction/blob/master/images/pdfPages.JPG)<br><br><br>
#提取效果<br>
![image](https://github.com/hooser/pdfAreaExtraction/blob/master/images/jietu.JPG)<br><br><br>

