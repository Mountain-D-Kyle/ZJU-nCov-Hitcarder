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
<ul>   
...  
...  
...  
</ul>   
这一段，复制到form.txt  
覆盖掉原来的表，  
手动打卡一次后即可继续自动打卡  
