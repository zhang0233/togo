# togo
<!-- saved from url=(0027)https://e.zufe.edu.cn/zc/zx -->
<html><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    
    <title>浙江财经大学健康通行码</title>
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
    <link rel="stylesheet" href="./浙江财经大学健康通行码_files/main.css">
<script src="./浙江财经大学健康通行码_files/jquery-1.7.2.min.js.下载"></script><script type="text/javascript" src="./浙江财经大学健康通行码_files/jquery.qrcode.min.js.下载"></script><script>
    jQuery(function(){

        jQuery('#output').qrcode({
            render	: "table",
            width: 170,
            height: 170,
            text	: "https://e.zufe.edu.cn/infoplus/form/enull/render",
            render: "canvas", //也可以替换为table
            foreground: "#1E90FF",
            background: "#FFF"
        });
        border();
        showTime();
    })
    function border() {
        var jz="已接种";
        var bor=document.getElementById('border');
        if("已接种"==jz){
            bor.setAttribute("src","/zc/resources/jkm/images/border.png");
            /*bor.style.top="-2px";
            bor.style.width="299px";
            bor.style.left="34px";
            bor.style.position="absolute";
            var pList=document.querySelectorAll(".qr p");
            pList[0].style.color="#676767";
            pList[1].style.color="#929191";*/
        }else {
            bor.setAttribute("src","/zc/resources/jkm/images/border.png");
        }
    }
    //获取系统时间
    function showTime() {
        nowtime = new Date();
        year = nowtime.getFullYear();//年
        month = nowtime.getMonth() + 1;//月
        day = nowtime.getDate();//日
        hour = nowtime.getHours();//时
        minutes = nowtime.getMinutes(); //分
        seconds = nowtime.getSeconds(); //秒
        //文字增加空格
        document.getElementById("div_timer").style = "white-space:pre;";
        //显示时间
        document.getElementById("div_date").innerText = p(month) + "月" + p(day) + "日 ";
        document.getElementById("div_timer").innerText = p(hour) + ":" + p(minutes) + ":" + p(seconds);
    }

    setInterval("showTime()", 1000);

    //月日时分秒小于10补0
    function p(s) {
        return s < 10 ? '0' + s : s;
    }

</script></head>





<body class="blue-bg">

<div class="content-box">
    <div class="now-date" id="div_date">10月06日 </div>
    <div class="now-time" id="div_timer" style="white-space: pre;">16:14:00</div>
    <div class="sss">
        <div class="link-btn" style="padding-top: 18px;">
            <a href="https://e.zufe.edu.cn/zc/zx" class=""><img src="./浙江财经大学健康通行码_files/an1.png"></a>
        </div>
        <div class="top-title">
            <div id="kongge">&nbsp;</div>
            <p style="font-size:1.0rem;">姓名：张志远</p>
            <p style="font-size:13px;">单位：会计学院（MPACC学院）</p>
        </div>

    </div>
    
        <div class="qr">
            
                <div id="output" style="width: 170px;margin: 0px auto;margin-bottom: 20px;margin-top: 5px;position: relative">
                    <img id="border" src="./浙江财经大学健康通行码_files/border.png">
                <canvas width="170" height="170"></canvas></div>
                <p style="font-size:20px;color: #E5BE60;">新冠疫苗接种情况
                    <span style="color: #3685EE;font-size: 20px;">已接种</span>
                </p>
                <p id="rqText" style="color:goldenrod;font-size:15px;margin:10px 0px 0px 43px;">第一针 2021-04-21 第二针 2021-06-15</p>
            
            
        </div>
    

    
        
            <div class="time">更新时间：2021-10-06 16:12:36</div>
            <div class="time">有效期：2021-10-06 00:00—24:00</div>
        
    <div style="text-align:center;padding-top: 20px">
        <a href="https://e.zufe.edu.cn/infoplus/form/JSXNYQSB/start?back=1&amp;x_posted=true">通行码申请</a>&nbsp;&nbsp;&nbsp;&nbsp;
        <a href="https://e.zufe.edu.cn/infoplus/form/FXSQ/start?back=1&amp;x_posted=true">学生返校申请</a>&nbsp;&nbsp;&nbsp;&nbsp;
        <a target="_blank" href="https://e.zufe.edu.cn/zc/getList?account=190110890727">查看申请记录</a>
    </div>
    <div style="margin: auto;width: 134px">
        <a target="_blank" href="https://xc.caict.ac.cn/#/login"> 通信大数据行程卡</a>
    </div>
</div>

</body></html>
