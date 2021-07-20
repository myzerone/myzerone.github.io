# zerone-z.github.io

# zerone-z 的博客

## 配置

由于网站已支持`https`访问，为了修改默认的引用地址为`https`，所以在`_config.yml`中加入了`url`配置项。开发、发布，注意点如下：  

### 本地文章预览

开发模式下，需要修改配置文件`_config.yml`。把`url`配置项给注释掉，防止链接跳转到外网地址。 

```vim
$ cd /..                            # 进入项目目录
$ bundle exec jekyll serve          # 启动服务
$ bundle exec jekyll serve --draft  # 启动服务并预览带有草稿的博客
```

### 发布到外网
 
发布到外网时，需移除`_config.yml`配置项`url`的注释。否则，默认的引用地址为`http`，会被浏览器识别为不安全的链接。
