### awk 使用

##### 实例
```shell script
touch a.txt
echo DBNAME.A.20220426.001 >> a.txt
```
获取里面的日期值：
```shell script
cat a.txt | awk -F '.' '{print $3'}
```
- `-F '.' `指定分割符为.
- `{print $3'}` 打印第3列 