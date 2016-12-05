1.封装了一个id函数，类似于jQuery里的写法
	function $(id){
		return 	document.getElementById(id);
		      }

2.value获取表单输入文本框内容：
	$("btn").onclick = function(){
			if($("txt").value == "小王")   //value获取表单的值
				alert("恭喜中奖");
			else
				alert("查无此人");
			}