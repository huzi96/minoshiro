#ģ���ļ��ṹ

-------------
```
templates/	//ģ��Ŀ¼
	class.json
	class1/		//ģ���ļ���1
	class2/		//ģ���ļ���2
	...
	
class.json	//ģ������嵥, json��ʽ
	����[{name: "����", src: "bussiness/", description: ""},
		 {name: "��Լ", src: "simplicity/", description: ""}]

class1/		//�����ļ���
	manifest.json
	item1/
	item2/
	...
	
manifest.json	//������ģ���嵥
	����[{name: "�������" ,src: "pku_1/", description: "",
		  size: "1200x800"}, ... ]

item1/		//ģ���ļ���
	main.json
	thumbnail.png	//����ͼ
	demo/		//������ʾ����Դ
	origin/		//�������ɳ�Ʒ����Դ
	
main.json	//ģ�����ļ�����¼�����������������Ϣ
	{
		demo_width:960 , demo_height: 400,
		origin_width: 9600, origin_height: 4000,
		bg: {
				manualable: false	//�Ƿ���ֶ����ñ���
				src: ["bg1.png","bg2.png", ... ],	//Ĭ�ϱ����������ж���
		},
		elements: [element1, element2, ... ],	//���������飬ÿ��element��һ��JS������������
		texts: [text1, text2, ... ]		//�������飬ÿ��text��һ��JS������������
	}

//element����
element = {
		src: "shape.png",	//�ò����ļ�
		x: 30, y: 30, regX: 0, regY: 0 , ...	//��������ͬeaselJS
}

//text����
text = {
		font: "Courier_New",	//��������
		content: "Study in Germany\nLand of Ideas",	//�������ݣ�������\n
		size: 14	//�����С��ֵ��ʾ
		style: "bold"	//����(bold, italic, etc)
		dir:0,	//����0��1��
		reg: 1,		//�ο��㡣0����1����2����3���ϡ��ο������겻�䣬��x,y���Ը���
		letter-spacing:0	//�ַ����
		x:y:regX:....	//��������ͬeaselJS
}
```