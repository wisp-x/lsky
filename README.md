<p align="center"><a href="https://www.lskys.cc" target="_blank"><img width="650"src="http://cdn.xlogs.cn/lskys.jpg"></a></p>

### 简介：
***
兰空，为个人站长、开发者、写博文爱好者开发的图床程序。同时可用作网络云相册。

### 安装需求：
***

* PHP版本 &gt; 5.3
* Curl支持
* Mysqli支持
* Rewrite

### 安装教程：
***
注意：暂不支持虚拟主机，数据库需要是innodb引擎


1. 下载兰空，上传至web运行环境，解压。
2. 设置运行目录为 public。
3. 配置Rewrite规则：
    ##### Nginx：
    <pre>
    location / {
        if (!-e $request_filename) {
        	rewrite ^(.*)$ /index.php?s=$1 last; break;
    	}
    }
    </pre>

    ##### Apache:
    Apache直接使用.htaccess即可

4. 访问首页，未安装自动跳转至安装页面，根据页面提示安装即可。

### Issues
***
你可以直接提交Lssues来说明你的问题，如果有建议请戳<a target="_block" href="http://www.lskys.cc/feedback.html">这里</a>提交

### 更新日志
***
每个版本更新的内容都会记录在此处：<a href="https://www.lskys.cc/record.html">http://www.lskys.cc/record.html </a>

### 联系我
***
QQ：1591788658<br>
Email: 1591788658@qq.com<br>
Blog: <a target="_block" href="http://www.xlogs.cn">www.xlogs.cn</a>

### 开源许可
***
<a target="_block" href="https://opensource.org/licenses/Apache-2.0">Apache 2.0</a>

Copyright (c) 2017 Wispx.
