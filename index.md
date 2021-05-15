<!DOCTYPE html>
<html lang="en">
 
    <head>
  <meta charset="utf-8">
  <meta http-equiv="pragma" content="no-cache">
  <meta http-equiv="Cache-Control" content="no-cache, must-revalidate">
  <meta http-equiv="expires" content="0">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0 user-scalable=0">
        <title>时间旅行者</title>
        <style>
            * {
                font-family: '微软雅黑', sans-serif;
                box-sizing: border-box;
            }
 
            body {
                display: flex;
                align-items: center;
                justify-content: center;
                min-height: 100vh;
                background: #ebf5fc;
            }
 
 body {
 
 	font-family: -apple-system, BlinkMacSystemFont,
 		"Segoe UI", "Roboto", "Oxygen", "Ubuntu", "Cantarell",
 		"Fira Sans", "Droid Sans", "Helvetica Neue",
 		sans-serif;
 
 	text-align: center;
 	background-color: #346271;
 	background-image: radial-gradient(ellipse 720px 100% at top center, #278572, #271956);
 	background-attachment: fixed;
 }
            .container {
                position: relative;
                display: flex;
                justify-content: space-around;
                align-items: center;
                width: 400px;
                flex-wrap: wrap;
            }
 
            .container .card {
                width: 320px;
                margin: 20px;
                padding: 40px 30px;
                background: #ebf5fc;
                border-radius: 40px;
                
            }
 
            .container .card:hover {
                box-shadow: inset -6px -6px 10px rgba(255, 255, 255, 0.5),
                    inset 6px 6px 20px rgba(0, 0, 0, 0.05);
            }
 
            .container .card .imgBx {
                position: relative;
                text-align: center;
            }
 
            .container .card .imgBx img {
                max-width: 120px;
            }
 
            .container .card .contentBx {
                position: relative;
                margin-top: 20px;
                text-align: center;
            }
 
            .container .card .contentBx h2 {
                color: #32a3b1;
                font-weight: 700;
                font-size: 1.4em;
                letter-spacing: 2px;
            }
 
            .container .card .contentBx p {
                color: #32a3b1;
            }
 
            .container .card .contentBx a {
                display: inline-block;
                padding: 10px 20px;
                margin-top: 15px;
                border-radius: 40px;
                color: #32a3b1;
                font-size: 16px;
                text-decoration: none;
                box-shadow: -4px -4px 15px rgba(255, 255, 255, 1),
                    4px 4px 15px rgba(0, 0, 0, .1);
            }
 
            .container .card .contentBx a:hover {
                box-shadow: inset -4px -4px 10px rgba(255, 255, 255, 0.5),
                    inset 4px 4px 10px rgba(0, 0, 0, .1);
            }
 
            .container .card .contentBx a:hover span {
                display: block;
                transform: scale(0.98) 2s;
            }
 
            .container .card:hover .imgBx,
            .container .card:hover .contentBx {
                transform: scale(0.98);
				transition: 1s ease-in-out;
            }
			.bottom {
				margin-top: 3.125rem;
				
				bottom: 0px;
			
				color: #fff;
				font-size: 0.6625rem;
				text-align: center;
				
			}
			#logo {
				
			}
			.kong{
				height: 20px;
			}
			.card{
				opacity: 1;
				filter:Alpha(opacity=100);
				transition: opacity 2s;
			}
			.readmore{
				 opacity: 0;
				 filter:Alpha(opacity=0);
			}
			.info{
				color: floralwhite;
				padding: 1.25rem;
				transition: 3s ease-in-out;
			}
			.tokeninfo{
				text-align: left;
			}
			.hide {
				display: none;
			}
			
        </style>
    </head>
 
    <body>
        <div class="container">
            <div class="card" id="pro1">
               
                <div class="contentBx"  id="token">
                    <h2>时间旅行者</h2>
                    <p id="info1">2009年6月28日，著名物理学家斯蒂芬·霍金举行了一场派对，邀请时间旅行者参加。不过，霍金在派对结束后才寄出请柬。毫无疑问，这是对时间旅行者的一次终极考验。不幸的是，时间旅行者对霍金的派对不理不睬，没有一人参加。霍金将这场派对视为一项实验，没人赏脸则是一个证据，证明时间旅行不可能实现。</p><p id="info2">但是真的如此吗？</p>
                    <a href="#" id="info3"><span onclick="more()">启动时光机</span></a>
                </div>
            </div>
			
			 
			<div class="bottom">
          <div id="logo"></div>
		  <div >喵族实验室</div>
		  </div>
            
        </div>
    </body>
 
</html>
<script src="https://cdn.bootcss.com/jquery/3.4.1/jquery.min.js"></script>
<script>
	var svg_logo='<svg t="1620957931218" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="1354" width="20" height="20"><path d="M441.131 746.831838c-46.687222 0-84.664463-38.153241-84.664463-85.054325 0-7.835095 6.311463-14.176232 14.110744-14.176232s14.110744 6.340114 14.110744 14.176232c0 31.258521 25.314408 56.702883 56.442975 56.702883 31.12959 0 56.442975-25.444362 56.442975-56.702883 0-7.835095 6.311463-14.176232 14.110744-14.176232s14.110744 6.340114 14.110744 14.176232C525.795462 708.678597 487.817199 746.831838 441.131 746.831838zM582.238438 746.831838c-46.687222 0-84.664463-38.153241-84.664463-85.054325 0-7.835095 6.311463-14.176232 14.110744-14.176232s14.110744 6.340114 14.110744 14.176232c0 31.258521 25.314408 56.702883 56.442975 56.702883s56.442975-25.444362 56.442975-56.702883c0-7.835095 6.311463-14.176232 14.110744-14.176232s14.110744 6.340114 14.110744 14.176232C666.903924 708.678597 628.92566 746.831838 582.238438 746.831838zM257.690307 484.579724a55.16 55.414 0 1 0 112.885951 0 55.16 55.414 0 1 0-112.885951 0ZM652.79318 484.579724a55.16 55.414 0 1 0 112.885951 0 55.16 55.414 0 1 0-112.885951 0ZM793.887316 753.918931c-2.122239 0-4.272107-0.470699-6.297137-1.494982l-56.442975-28.351442c-6.972488-3.515918-9.797706-12.016132-6.311463-19.021365 3.486244-6.977604 11.975202-9.857055 18.933364-6.340114l56.442975 28.351442c6.972488 3.515918 9.797706 12.016132 6.311463 19.021365C804.043163 751.039479 799.0691 753.918931 793.887316 753.918931zM850.344617 671.93643l-56.442975 0c-7.799281 0-14.110744-5.978903-14.110744-13.813999s6.311463-13.813999 14.110744-13.813999l56.442975 0c7.799281 0 14.110744 5.978903 14.110744 13.813999S858.143898 671.93643 850.344617 671.93643zM223.170659 753.918931c-5.181784 0-10.155847-2.879451-12.636227-7.835095-3.486244-7.005232-0.661025-15.504423 6.311463-19.021365l56.442975-28.351442c6.959186-3.515918 15.433818-0.636467 18.933364 6.340114 3.486244 7.005232 0.661025 15.504423-6.311463 19.021365l-56.442975 28.351442C227.442766 753.448231 225.292898 753.918931 223.170659 753.918931zM229.467796 671.93643l-56.442975 0c-7.799281 0-14.110744-5.978903-14.110744-13.813999s6.311463-13.813999 14.110744-13.813999l56.442975 0c7.799281 0 14.110744 5.978903 14.110744 13.813999S237.2681 671.93643 229.467796 671.93643zM1019.674566 569.634049c-6.969418-59.677497-19.385645-115.954705-36.791283-168.021201 3.388011-3.430988 6.197881-7.498443 7.549606-12.416227 36.51705-133.866856 48.464624-344.538522-17.390289-384.711677-7.950724-3.017591-17.84564-4.484945-30.260843-4.484945-69.272599 0-203.683829 48.036901-243.246098 62.766717-2.261403 0.848282-4.017315 2.372938-5.918531 3.710338-55.184367-22.864726-115.952658-35.522442-181.931386-35.522442-65.310539 0-125.354363 12.336412-179.929891 34.501229-1.454051-0.87898-2.651264-2.07517-4.289502-2.689125-39.562269-14.729816-173.973499-62.766717-243.246098-62.766717-12.416227 0-22.310119 1.467354-30.260843 4.484945C-11.897552 44.659123 0.050022 255.330789 36.567072 389.197645c0.982329 3.573221 2.737218 6.702348 4.850248 9.532682-17.841547 52.889196-30.62103 110.092453-37.723472 170.903722-37.923008 316.297593 225.772924 453.625111 507.989847 453.625111C792.240892 1023.25916 1057.597574 885.931641 1019.674566 569.634049zM942.505476 56.343719c3.36243 0 5.539925 0.249675 6.876302 0.470699 15.037817 16.46731 24.859058 132.677829-0.544374 262.091462C903.792513 226.11367 840.245049 151.702264 761.353814 101.7621 826.797377 79.580911 908.150573 56.343719 942.505476 56.343719zM77.618183 56.814418c1.336376-0.221024 3.513872-0.470699 6.876302-0.470699 33.857599 0 113.327999 22.57412 178.266071 44.456517-77.878208 48.872904-140.766693 121.432211-185.711305 212.0326C53.131591 185.889352 62.818786 73.020797 77.618183 56.814418zM895.749696 828.402988c-77.500626 87.799729-217.487595 138.153289-384.064977 138.153289-169.329949 0-305.656721-50.354583-383.157346-138.153289-57.309676-64.92477-79.242213-149.705885-66.978452-251.986778C96.762338 274.871969 257.689283 87.657496 511.684719 87.657496c243.566378 0 416.737642 187.214473 451.951059 488.758715C975.899539 678.697103 953.059371 763.478218 895.749696 828.402988z" p-id="1355" fill="#e6e6e6"></path></svg>'
	
	
	logo.innerHTML=svg_logo
	var pro1info='<h2>时间旅行者</h2><p>2009年6月28日，著名物理学家斯蒂芬·霍金举行了一场派对，邀请时间旅行者参加。不过，霍金在派对结束后才寄出请柬。毫无疑问，这是对时间旅行者的一次终极考验。不幸的是，时间旅行者对霍金的派对不理不睬，没有一人参加。霍金将这场派对视为一项实验，没人赏脸则是一个证据，证明时间旅行不可能实现。<p>不过大喵我是相信时间旅行的，霍金没有等来客人也许是其他原因，比如人类文明太短暂，或者当天堵车没能及时赶到，所以我决定在区块链上重新做这个实验，区块链公开透明，不可篡改，且只需要传送少量数据，比传送一个人过来更容易操作。</p><h3>实验内容</h3><p>时间旅行者在我发币之前联系我，或者在我发币之前给我发送一笔交易，并且备注一个暗号。</p><h2>TIME代币</h2><div class="tokeninfo"><p>代币名称：时间旅行者；</p><p>代币符号：TIME（BSC）;</p><p>总发行量：1000亿；</p><p></p>其中500亿奖励给时间旅行者，500亿提供流动性。正如霍金实验一样，时间旅行者应该在我按下发币按钮之前来敲我的门，或者我收到一个特殊的交易（发币之前24小时内的第一笔带暗号的交易），我和500亿代币会一直等待时间旅行者出现。暗号我会在发币之后给出。</div>'
	function more(){
		$(".card").addClass("readmore");	
			info1.innerHTML="时光机正在启动...."
			info2.innerHTML=""
			info3.innerHTML="点火成功"
		setTimeout(function(){info()},2000); 
		
		
	}
	function info(){
		$("#pro2").addClass("hide");
	$("#pro1").removeClass("card readmore");
	$("#pro1").addClass("info")
	
	
	token.innerHTML=pro1info	
	}
	
</script>
	
