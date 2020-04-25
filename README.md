**计G191 2019322035 周新易**
## 实验目的
    掌握字符串String及其方法的使用
    掌握异常处理结构
## 实验内容与要求
    利用已学的字符串处理知识编程完成《长恨歌》古诗的整理对齐工作，写出功能函数，并运行。
### 具体实验要求
    1.每7个汉字加入一个标点符号，奇数时加“，”，偶数时加“。”
    2.允许提供输入参数，统计古诗中某个字或词出现的次数
    3.考虑操作中可能出现的异常，在程序中设计异常处理程序
## 实验过程
### 《长恨歌》对齐
    将《长恨歌》字符串转为字符数组，运用for循环和if语句对《长恨歌》字符每7个分为一组，与2作余数运算判断奇偶加“，”和“。”。
```Java
 String str="汉皇重色思倾国御宇......";
        char[] str1=str.toCharArray();//将str转为字符数组
        for (int i=0;i<str.length();i++) {
        if(i%7==0){
        String strArray=str.substring(i,i+7);//截取字符i到i+7，每7个字符一组
        if(i%2==0) {
        System.out.print(strArray+",");
        }
        else {
         System.out.print(strArray+"。\r\n");
         }//奇数加“，”，偶数加“。”
        }
```
### 统计字符出现次数
    获取需要查询的字符去空格、将第0位转为字符数组，运用for循环与《长恨歌》字符数组作判等，统计次数。
```Java
Scanner a=new Scanner(System.in); //获取键盘输入
     System.out.println("请输入要查询的字："); 
     String s=a.next(); //a中除去空格的字符串
     char str2=s.charAt(0);//s中第0位字符
     int k=0;
     for(int j=0;j<str.length();j++) {
        if(str2==str1[j]) {
         k=k+1;
        }//统计出现次数
       }
       System.out.println("该字出现次数："+k); 
```
### 作异常处理
```Java
try {}catch (Exception e) {
        e.printStackTrace();
    }
```
## 流程图
![出错](https://github.com/Dolipor/Changhenge/blob/master/流程图.png)
## 实验结果
![出错](https://github.com/Dolipor/Changhenge/blob/master/流程图.png)
## 实验感悟
    通过补考对长恨歌实验的再次学习，让我掌握了字符串String及其方法的使用还有异常处理结构的添加。长时间没有触碰JAVA再到这次补考的学习，让我对JAVA加深的印象。我往后还会继续学习JAVA，不忘记课上所学内容，不断敲程序练习。
