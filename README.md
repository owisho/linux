# linux #
### 向linux传输文件大小受限的处理办法 ###   
在本地（windows环境）使用winrar软件将本地文件分卷压缩成zip格式     
例如：java.z01,java.z02,java.zip    
将文件上传至linux服务器指定目录，比如upload，在此目录中执行ll命令    
可以看到java.z01,java.z02,java.zip文件    
使用zip -F java.zip --out fix.zip命令将文件修复（其实为合并分卷）    
注意F为大写    
在服务器上unzip fix.zip即可    
