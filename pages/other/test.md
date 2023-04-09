# 测试页

　　希望用Markdown写个简易的博客，把想发表的东西写上来，这样至少有个实时更新的主页可以用。如果试着不错，就可以推广到更多用途。

　　github page还不太会用，写html不如写markdown方便。况且据说gitee在没钱的前提下不能自动同步github page。同步到gitee的好处是访问稳定，毕竟是打算给更多人看的。

![图1](image/README/1680774055033.png "图1标题")

<p><img src="image/README/飞热管干趴南桥.jpg" alt="foo" title="title" onerror="this.src='https://iknow-pic.cdn.bcebos.com/3bf33a87e950352a88cf131d5d43fbf2b2118b7c';this.onerror=null;"/></p>

<body>
    <h3>html展开</h3>
    <span id="content">
        这是一堆文字1<br>
        这是一堆文字2<br>
        这是一堆文字3<br>
        这是一堆文字4<br>
        这是一堆文字5<br>
        这是一堆文字6<br>
        这是一堆文字7<br>
        这是一堆文字8<br>
        这是一堆文字9<br>
        这是一堆文字10<br>
        这是一堆文字11<br>
        这是一堆文字12<br>
        这是一堆文字13<br>
        这是一堆文字14<br>
        这是一堆文字15<br>
        这是一堆文字16<br>
        这是一堆文字17<br>
        这是一堆文字18<br>
        这是一堆文字19<br>
   </span>
    <a href="javascript:;" id="btn">
        <<<收缩</a>
            <script type="text/javascript">
                //获取button按钮
                var btn = document.getElementById('btn');
                //获取p
                var content = document.getElementById('content');
                //获取p中的内容
                var str = content.innerHTML;
                //定义一个变量，表示当前的状态（收缩、展开）
                var onOff = true; // true表示展开
                btn.onclick = function() {
                    if (onOff) {
                        content.innerHTML = str.substr(0, 50) + "......";
                        btn.innerHTML = '>>>展开'
                    } else {
                        //说明当前状态是收缩的，需要展开
                        content.innerHTML = str
                        btn.innerHTML = '<<<收缩';
                    }
                    onOff = !onOff; //每点击一次，改变一次展开、收缩状态
                    return false; //阻止a标签的默认事件
                }
            </script>
</body>

</html>
