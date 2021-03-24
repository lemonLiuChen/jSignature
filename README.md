# jSignature 实现手写板签名demo
[Demo](https://lemonliuchen.github.io/jSignature/)  


**初始化**  
`// UndoButton: true/false 撤销按钮， lineWidth线条的粗细，color： 线条颜色 ` 
 `$('#signature').jSignature({'UndoButton': false, lineWidth:2, color: '#000'}); `  

**新增了设置线条粗细和颜色的方法，使用方法如下：**  

`$('#signature').jSignature("setLineWidth", "4"); // 设置线条粗细  `  
 `$('#signature').jSignature("setColor", "#1EAFE9"); // 设置线条颜色`

**判断是否签名:**  
if ($("#signature").jSignature("getData", "native").length == 0) {
  //如果等于0，就说明没有签名或者签名已经被清除
}
