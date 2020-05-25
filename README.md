

*****************************兼容已知其它工具的字典格式,字典中如有中文，字典须为UTF-8编码********************


1.在原版基础上做了优化，对界面、菜单功能做了修改;

2.增加了随机user-agent功能、字典多选功能、中文编码访问功能;

3.字典可以单选，也可以多选，可以浏览选中结合右侧勾选;

4.为了兼容其它工具的字典，修改了fuzz逻辑，最终的字典格式如下：

   4.1 payload可以写在一个文件中，也可以写在多个文件中。
   4.2 payload 可以写死后缀，格式如:/a/b/info.php，这种情况，请勾选 [Use Blank Extension]
   4.3 字典中每一行的payload，也可以写成动态后缀,格式如：/a/b/info{ext},
         然后在[File extension]中指定后缀，如：php或php,jsp或php,asp,aspx

   4.4 如果选中 Standard start point，而payload在字典中已经写好，
         请勾选 [Brute Force  Dirs] 及 [Brute Force Fils]及 [Use Blank Extension]，File extension可以不填写，
         这样就是使用字典中的payload进行目录fuzz+文件fuzz，否则单独fuzz目录或文件。


*********************整体功能和原版几乎一样，可以在网上搜搜Dir Buster教程，本地熟悉一下即可***********