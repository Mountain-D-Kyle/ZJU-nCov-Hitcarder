# Sample .yml

```yml
- name: Working
   uses: Long0x0/zju-ncov-hitcarder@0.0.x
      with:
         # zju account username(student  id).
         username: ${{ secrets.ZJU_USERNAME }}
         # zju account password.
         password: ${{ secrets.ZJU_PASSWORD }}
         # (optional) dingtalk_token.
         dingtalk_token: ${{ secrets.DINGTALK_TOKEN }}
         # (optional) serverchan_key.
         serverchan_key: ${{ secrets.SERVERCHAN_KEY }}
```

# 一些记录  
## 当打卡表变动时  
打开这个网页，查看源码  
https://healthreport.zju.edu.cn/ncov/wap/default/index  
将  
\<ul\>   
...  
...  
...  
\</ul\>   
这一段，复制到桌面新建的form.txt中，用UTF-8格式保存。
注意不能多或者少任意一个字符，必须是\<ul\>...\</ul\>完整的字符  
然后删掉库里的form.txt,把本地的form.txt传上去  
手动打卡一次后即可继续自动打卡  
