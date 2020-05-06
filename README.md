# flask-react

用flask启动react程序
```
--dist
    |---main.exe
    |---static(这个文件里面的内容，是react build文件内的内容)
          |--static
          |--favicon.ico
          |--index.html
          |--index.js

```


## 步骤：
1. 下载exe文件(如何是mac，请按照`打包流程`自行打包可执行文件)
2. 获取react编译好的程序：npm run build，这时，前端项目会多出一个build文件夹
3. 把build文件的内容拷贝到static文件夹即可

## 运行：
运行exe文件，浏览器访问127.0.0.1:5000

### 打包流程：

1. pip install pyinstaller
2. pyi-makespec -F  main.py
   如果想要打包成文件夹， 则把 -F 改成 -D
3. pyinstaller main.spec
