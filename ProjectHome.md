Python生成Excel封装，使用xlwt实现


使用举例：
```
from XLSWriter import XLSWriter

xlswriter = XLSWriter(u'陕西.xls')
xlswriter.writerow(['姓名', '年龄', '电话', 'QQ'], sheet_name=u'基本信息')
xlswriter.writerow(['张三', '30', '13512345678', '123456789'], sheet_name=u'基本信息')
    
xlswriter.writerow(['学校', '获得学位', '取得学位时间'], sheet_name=u'学习经历')
xlswriter.writerow(['西安电子科技大学', '学士', '2009'], sheet_name=u'学习经历')
xlswriter.writerow(['西安电子科技大学', '硕士', '2012'], sheet_name=u'学习经历')
    
xlswriter.writerow(['王五', '30', '13512345678', '123456789'], sheet_name=u'基本信息')
# don't forget to save data to disk
xlswriter.save()
```