codeCriterion
=============

E++ Studio FE Code Criterion

写在前面：

  1.不能有无故的空格和换行
  
  2.所有缩进均为按下两个空格键或者按下一个Tab键
  
  
    eg:
      .class{
        font-size:20px;  
      }
      
  3.所有变量的命名必须语义化
  
    eg:
      saveAddress         //这样OK!
      address1 or a1 or a //这样是不得行的

HTML语言代码规范风格
===================

  + 需要写合适的注释，在div的结束符</div>后面写注释，特别是在多层嵌套的div里面.

> eg:

       <div class="Address_btn">
         div的内容~~！巴拉巴拉巴拉巴拉~~！
       </div><!--END Address_btn-->

  + p标签里面嵌套的span标签的时候，如果span里面的内容很多，则需要换行，以便看的清晰.

> eg:

       <p>
         lalallalalalallalalalalalalallalalalalalalah
         <span>
           lalalalbalablalbalabalbalabalbalabalbal
         </span>
         lalallalalal
       </p>
       
     若p标签里面的东西或者span标签里面的东西不是很多则不需要换行.

  + 没有换行的标签连在一起的时候，标签与标签之间要有空格，以便看得清晰内容属于哪一个标签。

>eg:

       <p> labala <span> haha </span> </p>

  + 在代码块的前面要写清楚这个代码块的内容作用是干什么,特别是代码块很长的情况下。

> eg：

       <!--在线人员列表-->
       <div>
       </div>
       <!--END 在线人员列表-->
    
  + 在超链接没有地址的情况下可以这么写.

> eg:

      <a href="javascript:;"></a>

CSS语言代码规范风格 
------------------

  + 在CSS文件写的最开头注释这个文件是哪一个HTML文件的样式，也可以有作者信息之类的。
    > eg:

        //Address.html的样式
        // author by xxx
        
  + 在冒号的后面留一个空格之后再写属性值。
    > eg:

        font-size: 10px;

  + 在括号的后面要注释匹配的是哪一个括号,特别是嵌套较深的情况下。
    > eg:

        .Address{
          font-size: 10px;   
        }//END .Address

  + 最好使用less的嵌套来写样式，这样可以避免混乱，不晓得这个样式对应哪一个节点（在有同样命名的类或者HTML标签）
    > eg:

        .saveAddress{
          p{
            font-size: 10px;  
          }//END p
        }//END .saveAddress

  + 在属性很多的情况下，注意分块写，而且要把影响布局的样式属性放在前面（width height margin padding..）,分的块之间需要有空行。
    > eg:

        .saveAddress{
          margin-left: 10px;
          margin-right: 10px;
          padding: 10px;

          font-size: 10px;
          color:#000;
        }//END .saveAddress 

  + 若出现等号，则等号两边要有空格。
  
  + 注意缩进对齐，代码很整齐很松散的样子比较好看，可读性也比较高。
  
javascript代码规范风格
---------------------

  + 在JS文件的最开头注意写注释
    > eg:

        //address的js文件
        //author by xxx

  + 在等号的两边有空格。
    > eg:

        var name = "xxx";

  + for循环的分号后面空格，表示分号属于前一个变量，括号(两种括号都是"()""{}")两边空格，易于阅读,}与for的第一个字母"f"对齐。
    > eg:

        for ( var i = 0; i < list.length; i++ ) {
          代码内容balabalabala 
        }//END for
        
  + 结束处要注明注释。
    > eg:

        function address () {
          代码块内容 
        }//END address

未完待续...
