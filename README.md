# JKCMS手册
>JKCMS是本人做的一个简单的基于ThinkPHP的后台管理系统，注意只是后台管理系统，没有前台哦，前台需要自己写的

### index.php
* 定义系统的根路径：ROOT_PATH

`define("ROOT_PATH", dirname(__FILE__));`

### Html静态页面
`$this->buildHtml("index",ROOT_PATH."/");`

### JKCMS目录说明：
* admintpl            后台模板
* tpl                 前台目录
* core                系统核心目录
* app/                项目目录
* dbbak               数据库备份目录，要可写
* runtime             
* Public              公共文件目录。
* index.php           首页目录
* upload              上传目录 


### 常见函数
* get_ip()     //获取IP函数
* array_iconv($fContents, $from='gbk', $to='utf-8')   //自动转换字符集 支持数组转换
* block($k,$cache=true)     //碎片获取函数
* adv($k,$cache=true)      //广告获取函数
* password($password,$salt='')         //系统文本加密函数
* sendemail($to,$subject,$content)      //系统邮件发送函数
* rand_string($len=6,$type='',$addChars=''         //产生随机字串
* remove_xss($val)         //系统过滤xss函数
* seo_keyword($content)     //seo关键词替换，注意要包含在闭合标签中。支持 标签内的 文本不替换。
