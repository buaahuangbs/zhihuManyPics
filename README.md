# zhihuManyPics

* chrome插件
* 当一个回答里包含上百张图片时, 难以一次性上传, 并且编辑起来很麻烦
* 可以先在word中编辑好
* 然后将docx文件读取到剪贴板, 直接复制到回答框中
* 以此来简化知乎传图步骤

## 使用说明
* 添加到chrome扩展
* 打开知乎问题页面
* 点击扩展browser action选择docx文件
   1. 新问题
        自动将docx内容填入答题编辑器
   2. 有草稿
        保留原草稿, 另起一行将docx内容填入答题编辑器
   3. 已回答
        先点击编辑, 将答题编辑器打开后同有草稿处理

## 程序流程
* 将docx文件转为html格式
* 将html文本中的图片上传到知乎服务器, 得到图片地址
* 生成新的html文本
* 把html文本放入剪贴板
* 查找当前页面中的答题编辑器, 并粘贴html文本