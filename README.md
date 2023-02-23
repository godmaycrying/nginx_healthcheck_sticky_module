# ***nginx_healthcheck_sticky_module***

## **描述**
本项目收集自：  
[***zhouchangxun/ngx_healthcheck_module***](https://github.com/zhouchangxun/ngx_healthcheck_module)    
与  
[***nginx-sticky-module-ng***](https://bitbucket.org/nginx-goodies/nginx-sticky-module-ng/src/master/)    
并参考：  
[***yaoweibin/nginx_upstream_check_module***](https://bitbucket.org/nginx-goodies/nginx-sticky-module-ng/src/master/)    
对其进行源码修改，同步最新版本nginx，制作patch。  

## **使用方法**
```shell
cd nginx-release-1.23.x
patch -p1 < ${ngx_healthcheck_module_path}/nginx_healthcheck_for_nginx_1.23+.patch
auto/configure --add-module=${ngx_healthcheck_module_path} --add-module=${ngx_sticky_module_path}
```