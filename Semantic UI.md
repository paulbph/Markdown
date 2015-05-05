Semantic UI是什麼?  
=================
*	一個前端開發的framework 
*	使RWD(Responsive Web Design)自適應網頁開發變得方便
*	RWD簡單說是設計在各種裝置上適合瀏覽的網頁  

Semantic UI的優點
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
			![img1](images/SUdemo7.jpg	"demo")
		* Vertically Divided Grid
			![img1](images/SUdemo8.jpg	"demo")
		* Celled Grid
			![img1](images/SUdemo9.jpg	"demo")
		* Internally Celled Grid
			![img1](images/SUdemo10.jpg	"demo")



2.Tag套用樣式限制少並簡潔
--------------
*   button
	
	![img1](images/SUdemo4.jpg	"demo")
*   label

	![img1](images/SUdemo5.jpg	"demo")
*   list

	![img1](images/SUdemo6.jpg	"demo")


與Bootstrap的差異
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

	* 其他特色:
		* Nestable
		
			![img1](images/SUdemo30.jpg	"demo")
			
			* 用Semantic UI實現相同效果
			
					<div class="ui grid">
						<div class="twelve wide column">
							Level1: 12 column
							<div class="ui grid">
								<div class="eleven wide column">
									Level2: 11 column
								</div>
								<div class="five wide column">
									Level2: 5 column
								</div>
							</div>
						</div>
					</div>

		* Offsets

			![img1](images/SUdemo29.jpg	"demo")

			* 用Semantic UI實現相同效果
			
					<div class="ui grid">
						<div class="four wide column">
							four wide column
						</div>	
						<div class="eight wide column">
						
						</div>
						<div class="four wide column">
							four wide column
						</div>
					</div>
		* Column ordering
		 
			![img1](images/SUdemo31.jpg	"demo")
			
			* 用Semantic UI實現相同效果
			
					<div class="ui grid">
						<div class="right floated twelve wide column">
							twelve wide column
						</div>	
						<div class="left floated four wide column">
							four wide column
						</div>
					</div>
	
2. Tag套用樣式
	*   button
		
		![img1](images/SUdemo17.jpg	"demo")
	*   label
	
		![img1](images/SUdemo18.jpg	"demo")
	*   list
	
		![img1](images/SUdemo19.jpg	"demo")
	


Friday首頁 RWD試作
=====================
* 電腦
![img1](images/SUdemo20-1.jpg	"demo")
![img1](images/SUdemo20-2.jpg	"demo")

* Sidebar Menu
	* 手機
	
	![img1](images/SUdemo21.jpg	"demo")

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
	* 平版
	
	![img1](images/SUdemo22.jpg	"demo")
	
		<div id="hidemenu" class="three wide computer only column" style="padding-left:0px;padding-right:0px;">
			<div class="hidemenu small ui vertical  menu">
			  <a class="header item"><h4 class="center aligned">商品分類</h4></a>
			  <a class="item">品味「創」策展</a>
			  ........
			</div>
		</div>

* Column wide set
	* 平版
	
	![img1](images/SUdemo24.jpg	"demo")
	* 手機

	![img1](images/SUdemo26.jpg	"demo")

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
	* 平版
	
	![img1](images/SUdemo25.jpg	"demo")
	
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
	* 電腦
	
	![img1](images/SUdemo27.jpg	"demo")
	* 平版
	
	![img1](images/SUdemo28.jpg	"demo")

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