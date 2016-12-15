##JavaScript数据类型
number，字符串，null，undefined，布尔，数组，对象

###1.number

    1;//整数
    1.1;//浮点数
    -1;//负数
    12e2;//科学计数法12*100
    NaN;//not a number,计算
    Infinity;//无限大
可直接做四则运算

    1+1;//加减法2
    4/2;//基本乘除法1
    5%2;//取余1
    0/0;//NaN
    1/0;//Infinity
###2.字符串
	双引号"",或者单引号'',包裹的各种数据
	'',//表示空字符串
###3.null
	空的值，未赋值，不是0，也不是''
###4.undefined
	值未定义,判断函数参数是否传递
###5.布尔
	false;
	true;
	2>3;//运算表示,false
	2<3;//true
	//比较运算或者逻辑运算获得,&&,!,||,>=,===
###6.数组
创建数组,第一种，[]，创建代码可读性高

	var i = [1,null,undefined,'hello',true];//可含各数据类型
	var k = new Array(1,2,3);
访问数组，从0开始

	i[3];//hello
	k[3];//undefined，索引未定义
###7.对象
键值对，无序集合


	var person = {       //声明对象person
    	name: 'Tom',
    	age: 13,
    	isSingle: true,
    	hobbits: ['ridding','swimming','cooking'],
    	dislike: null    //最后无','结束
	}
访问对象属性

	person.name;//Tom
