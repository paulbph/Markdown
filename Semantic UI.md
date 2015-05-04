Semantic UI是什麼?  
=================
*	一個前端開發的framework 
*	使RWD(Responsive Web Design)自適應網頁開發變得方便
*	RWD簡單說是設計在各種裝置上適合瀏覽的網頁  

Semantic UI有什麼優點?
=====================

1.好用的Grid system
--------------
* grid system 將一列區分為16個欄位共16等份
* 宣告不同的class達到不同的寬度與排列效果
* 宣告的class名稱可依需求作微調
 
	* 宣告方式
	
			<div class="ui grid">
			</div>

			<div class="ui page grid">
			</div>

			<div class="ui two column grid">
			</div>

		![img1](images/SUdemo1.jpg	"demo")
		
		![img1](images/SUdemo3.jpg	"demo")
		
		![img1](images/SUdemo2.jpg	"demo")

	* Grid樣式
		* Divided Grid
		* Vertically Divided Grid
		* Celled Grid
		* Internally Celled Grid



2.Tag套用樣式限制少並簡潔
--------------
*   button
	
	![img1](images/SUdemo4.jpg	"demo")
*   label

	![img1](images/SUdemo5.jpg	"demo")
*   list

	![img1](images/SUdemo6.jpg	"demo")

3.獨特實用的元件
---------------
* Divider

	![img1](images/SUdemo7.jpg	"demo")
* Flag 

	![img1](images/SUdemo8.jpg	"demo") ![img1](images/SUdemo9.jpg	"demo")
* Step

	![img1](images/SUdemo10.jpg	"demo")
* Advertisement

	![img1](images/SUdemo11.jpg	"demo")![img1](images/SUdemo12.jpg	"demo")
* Feed

	![img1](images/SUdemo13.jpg	"demo")![img1](images/SUdemo14.jpg	"demo")
* Comment、Rail、Reveal、Card、Item、Statistic、Dimmer、 Rating、 Shape....etc.
 


與Bootstrap的差別?
=====================
1.	grid system
	* 欄位數
		* grid system 將一列區分為12個欄位共12等份,  
		* 用不同的prefix class配上不同數字達到不同的寬度與排列效果	
		* 不同名稱的prefix class對應不同的裝置
		![img1](images/SUdemo15.jpg	"demo")
	* 宣告方式
	 
			<div class="container">
				...
			</div>	
			<div class="container-fluid">
			  ...
			</div>

		![img1](images/SUdemo16.jpg	"demo")
			
	* Grid樣式:無
	
2. Tag套用樣式限制
	*   button
		
		![img1](images/SUdemo17.jpg	"demo")
	*   label
	
		![img1](images/SUdemo18.jpg	"demo")
	*   list
	
		![img1](images/SUdemo19.jpg	"demo")
3. 獨特的元件
	* Jumbotron
	
	


DEMO  
=====================



原始碼
=====================
* Sidebar Menu

		<div class="ui labeled icon left inline vertical sidebar menu" style="width:50%">
		<a class="item">
			<div class="ui small input" style="">
				<input placeholder="商品搜尋" type="text" style="width:30px;">
					<button class="ui red icon button">
						<i class="search icon"></i>
					</button>
			</div>
		</a>

		<a class="header item" style="background-color:#F00000;color:white;">
		MENU
		</a>
		.......
		<a class="header item" >
	        商品分類
	      </a>
			<div class="sub menu">
			 <a class="item">
				品味「創」策展
			 </a>
			  .....
			</div>
		.......
		</div>

		<div class="pusher">
			//page content
		</div>

* Menu hide
	
		<div id="hidemenu" class="three wide computer only column" style="padding-left:0px;padding-right:0px;">
			<div class="hidemenu small ui vertical  menu">
			  <a class="header item"><h4 class="center aligned">商品分類</h4></a>
			  <a class="item">品味「創」策展</a>
			  ........
			</div>
		</div>

* Submenu arrange

		<div class="ui one column grid">				
			<div class="column">
				<h5 style="margin:0px 0 0 0px;">手機</h5>				
				<ul class="items">
					<li class="lrow">ZenFone2</li>
					<li class="rrow">HTC M9</li>
					<li class="lrow">HTC 620/62</li>
					<li class="rrow">LG AKA</li>
					<li class="lrow">iPhone6 Plu</li>
					<li class="rrow">iPhone6</li>
				</ul>
			</div>
			..........
		</div>

* Column wide set

		<div class="ui padded grid">
			<div class="sixteen wide mobile eight wide tablet four wide computer column">
				<img class="ui image" src="s_1917709_a40598eac1_o.jpg">
				<div class="value">【XD-Design】Tovo 萬能瑞士刀 </div>
				<div style="float:left;"><h4>$599</h4></div>
				<div style="float:right;" >搶購</div>					
			</div>
			..................
		</div>		

* AD不同裝置設定
	
		<!--computer only-->
			<div class="three wide computer only column">
				<div class="header">會員活動</div>
				<div class="ui image">
					<img src="635b10.jpg">
				</div>
			</div>
			
		<!--tablet only-->
			<div class="ui hidden divider"></div>
				<div class="four wide tablet only column">
					<div class="header">達人專欄</div>
					<div class="ui image">
						<img src="6d1ff5.jpg">
					</div>
				</div>
				<div class="four wide tablet only column">
					<div class="ui image">
						<img src="dbebd6.jpg">
					</div>
				</div>
				<div class="four wide tablet only column">
					<div class="ui image">
						<img src="a52aa6.jpg">
					</div>
				</div>
				<div class="four wide tablet only column">
					<div class="header">會員活動</div>
					<div class="ui image">
						<img src="635b10.jpg">
					</div>
				</div>
				<div class="ui hidden divider"></div>
		<!--mobile only-->
				<div class="sixteen wide mobile only column">
					<div class="header">達人專欄</div>
					<div class="ui fluid image">
						<img src="6d1ff5.jpg">
					</div>
				</div>
				<div class="sixteen wide mobile only column">
					<div class="ui fluid image">
						<img src="dbebd6.jpg">
					</div>
				</div>
				<div class="sixteen wide mobile only column">
					<div class="ui fluid image">
						<img src="a52aa6.jpg">
					</div>
				</div>
				<div class="sixteen wide mobile only column">
					<div class="header">會員活動</div>
					<div class="ui fluid image">
						<img src="635b10.jpg">
					</div>
				</div>
				<div class="ui hidden divider"></div>
		<!---->

* equal height stretched row

		<div class="equal height stretched row">
			<div class="sixteen wide mobile four wide tablet three wide computer column">
				<img class="ui " src="10d27c.jpg">
			</div>
					
			<div class="sixteen wide mobile twelve wide tablet thirteen wide computer column">
				<div class="ui computer grid">
					<div class="sixteen wide mobile four wide tablet three wide computer column">
						<img class="ui image" src="s_2166115_5a989d7c63_o.jpg">
						<div class="value">【STARMIMI】水彩花草滿版印樣洋裝 ＊SM (</div>
						<div style="float:left;"><h4>$484</h4></div>
						<div style="float:right;" >搶購</div>
					</div>
					...................	  		
				</div>
			</div>
		</div>