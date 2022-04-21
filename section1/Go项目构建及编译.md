# Go项目构建及编译

````
src：源代码文件
pkg：包文件
bin：相关bin文件
````

1. 建立工程文件夹goproject


2. 在工程文件夹中建立src，pkg，bin文件夹


3. 在GOPATH中添加goproject路径 如E:/goproject


4. 如工程中有自己的包examplepackage，那么在src文件夹下建立以包名命名的文件夹，如examplepackage


5. 在src文件夹下编写主程序代码 goproject.go


6. 在examplepackage文件夹中编写examplepackage.go和包测试文件examplepackage_test.go


7. 编译调试包
   ````
   go build examplepackage
   go test examplepackage
   go install examplepackage
   ````
   这时在pkg文件夹中可以发现会有一个相应的操作系统文件夹如windows_386z，在这个文件夹中会有examplepackag文件夹，在该文件中有examplepackage.a文件


8. 编译主程序
    ````
    go build goproject.go
    ````
    成功后会生成goproject.exe文件

至此一个Go工程编辑完成。