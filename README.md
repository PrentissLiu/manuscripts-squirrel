
<div align="left">
    <a href="https://alist.nn.ci"><img height="100px" alt="logo" src="icon.ico"/></a>
<div>



# dezooomify-rs-brilliant

一个批量生成[http://gallica.bnf.fr](http://gallica.bnf.fr)下载链接以供dezooomify-rs下载图片的脚本

## 适用网站

目前仅适用于法图[http://gallica.bnf.fr](http://gallica.bnf.fr) 批量下载，其他网站尚未支持。

不过若需要下载的网站URL路径与法图路径规则相似，可以修改`config.ini`的`url`参数生成批量下载的下载链接。


## 使用说明
下载release文件并解压

1. 双击打开amazing-button.exe
2. 根据提示生成bat文件
3. 双击bat文件下载图片

注意config.ini是配置文件，不可以删除和更改名称.可以修改该文件内参数.


## config.ini参数：

- `url`：使用`<id>`和`<picnum>`替换原链接中的一系列图片的ID，比如将：

	`https://gallica.bnf.fr/ark:/12148/btv1b8304060b/f1.item.r=pelliot%204640.zoom` 

	替换为：`https://gallica.bnf.fr/iiif/ark:/12148/<id>/f<picnum>/info.json`


- `start_num`:开始下载的图片标号，对应上述链接中的`<id>`起始值

- `run_exe ` :Windows里`dezoomify-rs.exe`文件名