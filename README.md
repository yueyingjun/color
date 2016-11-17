# 颜色渐变和透明度   
## 颜色的透明度  
1. rgba()  `a` 代表的透明通道,取值范围 0-1    
   `通过改变整体容器的透明度来实现透明,但是他会影响容器里面的内容`    


    opacity:0~1
    filter:alpha(opacity=0~100)
2. background:transparent     
   可以直接使用改值,实现完全透明
3. background-color:hsla(120,65%,75%,0.3);    
   色调(H)、饱和度 (S)、亮度(L)三个颜色通道的变化以及它们相互之间的叠加来得到各式 各样的颜色的,HSL即是代表色调,饱和度,亮度三个通道的颜色   
  3.1 取值说明:Hue(色调),取值范围为:(0-360,) 0(或360)表示红 色,120表示绿色,240表示蓝色,当然可取其他数值来确定其它颜 色;  
  3.2 Saturation (饱和度)的值形式为百分比(0%:gray ,100%:full color);  
  3.3 Lightness (亮度)值形式也为为百分比(0%:black,100%: white);  
  3.4 Alpha(透明度)的取值(0 -1)
   
## 渐变  
### 线性渐变
1.  background: linear-gradient(red, blue,green,yellow);  
  1.1 平均分布的渐变,只需要在参数里面,写入相应的颜色值就可以   
2.  background: linear-gradient(red 0%, blue 10%,green 70%,yellow 80%);  
  2.1 颜色以及颜色停靠的位置 只需要在颜色的后面写上百分比即可  
  **注意:相应的颜色以及他所对应的位置是一个参数,用`空格`隔开,多个参数之间用 `,` 隔开**
3. 设置渐变的角度  
  3.1  background: linear-gradient(to left top,red 0%, blue 10%,green 70%,yellow 80%);  
  **通过关键字的方式:  to 方向**    
  3.2  background: linear-gradient(45deg,red 0%, blue 10%,green 70%,yellow 80%);  
  **通过设置角度的方式**  
### 径向渐变
1. background: radial-gradient(red, green, blue);
2. background: radial-gradient(red 0%, green 50%, blue); 
3. 改变渐变的形状  
  3.1 background: radial-gradient(circle 50px at 120px 120px,red 0%, green 50%, blue);  
   circle 形状    50px   渐变的区间    at 120px 120px 渐变起始位置
  3.2 background: radial-gradient(ellipse 50px 30px at 120px 120px,red 0%, green 50%, blue);  
   椭圆的大小需要两个半径作为约束
   
### 重复渐变  
   background: repeating-radial-gradient(red, yellow 10%, green 15%);
   
 
   
   
   
   
   
   


