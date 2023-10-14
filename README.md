
<div align="left">
    <a href="https://github.com/PrentissLiu/manuscripts-squirrel"><img height="100px" alt="logo" src="icon.ico"/></a>
<div>



# Manuscripts Squirrel

一个简单易用的命令行写卷下载工具

这个项目最初发布名为`dezoomify-rs-brilliant`，是为了解决批量输入命令行过于麻烦的问题。

可以提[issue](https://github.com/PrentissLiu/manuscripts-squirrel/issues/new).

## Supported Sites

1. 法国国家图书馆 [https://gallica.bnf.fr/](https://gallica.bnf.fr/)
   
2. 国际敦煌项目（International Dunhuang Project）
   -  [http://idp.bl.uk/](http://idp.bl.uk/) 
   -  [http://idp.bl.fr/](http://idp.bl.fr/) 
   -  [http://idp.bbaw.de/](http://idp.bbaw.de/)

3. 故宫博物院 [https://www.dpm.org.cn/](https://www.dpm.org.cn/)
   -  [故宫名画记](https://minghuaji.dpm.org.cn/) 和 [数字文物库](https://digicol.dpm.org.cn/) 的链接不支持下载.



## Usage
下载release文件并解压

1. 双击打开`Manuscripts Squirrel.exe`
2. 根据提示生成bat文件
3. 双击bat文件下载图片

如果是国际敦煌项目的下载方式则用本工具本身下载，不需要双击bat文件.



## Advanced Settings：

对于`config.ini`配置文件，我们可以修改参数.

法国国家图书馆 [https://gallica.bnf.fr/](https://gallica.bnf.fr/) 
- `url`：使用`<id>`和`<picnum>`替换真实链接中的一系列图片的ID，比如：

	`https://gallica.bnf.fr/iiif/ark:/12148/<id>/f<picnum>/info.json` 中`<id>`对应真实链接中的`btv1b8304060b`,`<picnum>`对应图片序列号.


- `start_num`:开始下载的图片标号，对应上述链接中的`<picnum>`起始值.

- `run_exe ` :Windows里`dezoomify-rs.exe`文件名.

故宫博物院 [https://www.dpm.org.cn/](https://www.dpm.org.cn/) 的参数：

- `url_gugong`：故宫下载的URL网址，用于替换网页中的`id`链接适配。比如将：

	`https://en.dpm.org.cn//tilegenerator/dest/files/image/<id>` 将其中的`<id>`替换为真实链接中的`/8831/2008/1180/img0014.xml`.

## Version History


- v2.0 新增支持：国际敦煌项目和故宫博物院
- v1.3 初次发布，支持法图图片的批量下载
  

## Known Issues

国际敦煌项目中点击`Large Image`按钮的的目前不可以解析下载，需要寻找能点击打开`Large Image`的页面.


## Authors

Code with ❤️  by [Prentiss](https://github.com/PrentissLiu) .

Contributing for Testing and interface language by [FlyingSquirrel](http://hamsterstowerofbabel.net/)

Thanks for [dezoomify-rs](https://github.com/lovasoa/dezoomify-rs), the wonderful image zoom downloader.
