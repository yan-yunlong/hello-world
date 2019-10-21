
1.将两个字符利用字符串对象的方法变成一个字符,显示在页面id为h1的元素中
答:
		<script type="text/javascript">
			var a = '111';
			var b = '222';
			var c = a.concat(b);
            h1.innerHTML = (c);
		</script>
2.一个富豪想存87万,给理财顾问写了87w,请自动生成存储870000的方法,显示在页面id为h2的元素中
答:
        <script>
             var str = '87';
             var estr = str.padEnd(6,'0');
             document.getElementById('h2').innerHTML= estr;
        </script>
3.一个数字79387.348的工程款,保留两位小数存入,显示在页面id为h3的元素中
答:
	    <script type="text/javascript">
			var num = new Number(79387.348);
			document.getElementById('h3').innerHTML = num.toFixed(2);
		</script>
4.一张图片是一个相对路径img/head/,icon/1.jpg,我只需要拿到它的文件夹目录后显示在页面id为h4的元素中
答:
<script type="text/javascript">
			var h4 = document.getElementById('h4');
			var img = 'img/head/icon/1.jpg';
			h4.innerHTML = img.substr(-5,5);
		</script>
5.用户输入验证码,无论大小写输入都会正确的方法,显示在页面id为h1的元素中,显示在页面id为h4的元素中
答:
	<script type="text/javascript">
			var nstr = prompt('输入验证码');
            var h4 = document.getElementById('h4');
            h4.innerHTML = nstr.toLocaleUpperCase();
		</script>