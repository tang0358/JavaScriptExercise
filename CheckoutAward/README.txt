1.��װ��һ��id������������jQuery���д��
	function $(id){
		return 	document.getElementById(id);
		      }

2.value��ȡ�������ı������ݣ�
	$("btn").onclick = function(){
			if($("txt").value == "С��")   //value��ȡ����ֵ
				alert("��ϲ�н�");
			else
				alert("���޴���");
			}