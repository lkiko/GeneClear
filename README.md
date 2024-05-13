# GeneClear

## 使用方法 

下载GeneClear-0.0.0-py3-none-any.whl文件到本地
然后 

pip install GeneClear-0.0.0-py3-none-any.whl

### 输出帮助文件：

GeneClear -h

 #### 输出：

usage: GeneClear [options] 

runing GeneClear 
    -------------------------------------- 

options: 

  -h, --help            show this help message and exit 
  
  -v, --version         show program's version number and exit 
  
  -getpasa GETPASA      get_PASA 
  
  -getncbi GETNCBI      get_NCBI 
  
  -vgo VISUALIZATION_GO 
  
Visualization_GO 
                        

使用方法详见CSDN或知乎https://zhuanlan.zhihu.com/p/660795982

## GO富集可视化！

### 查看配置文件：
GeneClear -vgo ?

[Visualization_GO] 

#脚本适用于TBtools的GO富集可视化 

TB_file = TBtools file 

Class_dic = Biological process:#0095d9,Molecular function:#f39800,Cellular component:#d7003a 

top = 20 

savefile = save file (*.png, *.pdf, *.svg) 

### 文件说明：

TB_file = TBtools file

#TBtools的GO聚类结果文件

Class_dic = Biological process:#0095d9,Molecular function:#f39800,Cellular component:#d7003a

#三种类型的颜色配置

top = 20

#保留富集程度最高的前20个

savefile = save file (*.png, *.pdf, *.svg)

#保存文件 svg方便后续拼图或者精修！

### 配置文件重定向：
GeneClear -vgo ? >total.conf

GeneClear -vgo ? >> total.conf

### 运行：
GeneClear -vgo total.conf
![all](https://github.com/lkiko/GeneClear/assets/57740432/2ff063f4-8f70-4132-9fcb-112c5547a3d2)


