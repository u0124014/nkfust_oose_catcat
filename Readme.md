## 班級 小組名稱:第10組  非常貓貓 ##

## 小組成員:##

<table>
<tr>
<td>學號</td>
<td>組員</td>
<td>工作分配</td>
</tr>
<tr>
<td>0124014</td>
<td>陳南岑</td>
<td>利害關係人目標表、訂票基本作業表</td>
</tr>
<tr>
<td>0124058</td>
<td>張耿瑞</td>
<td>憑據處理作業表、銷售分析表</td>
</tr>
<tr>
<td>0124048</td>
<td>林宛葶</td>
<td>處理訂單紀錄表、現有座位及退票處理作業作業</td>
</tr>
<tr>
<td>0124078</td>
<td>石羽璇</td>
<td>電影基本資料作業表、使用案例圖</td>
</tr>
</table>

## 專題題目:電影劃位系統 Fun-Movie##

本系統是為方便一般民眾能夠隨時隨地運用便利商店裡的線上購票系統，進行電影時刻及座位的查詢，在最短的時間內，查詢到符合自己需求的電影及座位，不必親臨電影院，才發現僅剩視野較不佳的座位，或是已沒座位、錯過電影撥放時間等突發狀況，而一掃看電影的興致

## 利害關係人目標表 ##
<table width="1000">
<tr>
<td><center>利害關係者(參與者)</center></td>
<td><center>目標</center></td>
</tr>
<tr>
<td>管理階層</td>
<td>1.進行策略規劃<br>
2.分析銷售狀況</td>
</tr>
<tr>
<td>銷售人員(超商人員)</td>
<td>1.可以用條碼掃描，加快結帳速度<br>
2.可以進行退票處理作業</td>
</tr>
<tr>
<td>合作對象</td>
<td>1.正確記錄劃位狀況及現有座位資料<br>
2.能夠快速更新及修改電影資訊
</tr>
<tr>
<td>線上更新人員</td>
<td>1.接收合作對象提供的電影資訊並更新至系統上</td>
</tr>
<tr>
<td>系統管理者</td>
<td>1.處理訂票、退票相關資訊</td>
</tr>
<tr>
<td>顧客</td>
<td>1.查詢電影資訊<br>
2.選擇訂購填入基本資料</td>
</tr>
</table>
## 事件與使用案例表 ##
<table width="550">
<tr>
<td><center>事件名稱</center></td>
<td><center>使用案例名稱</center></td>
</tr>
<tr>
<td>1.建立與修改訂票紀錄</td>
<td>1.訂票基本資料作業</td>
</tr>
<tr>
<td>2.客戶訂購電影票</td>
<td>2.處理訂單紀錄</td>
</tr>
<tr>
<td>3.查詢與更新現有作業及退票作業</td>
<td>3.現有座位及退票處理作業作業</td>
</tr>
<tr>
<td>4.查詢與更新電影時刻</td>
<td>4.電影基本資料作業</td>
</tr>
<tr>
<td>5.列印繳費憑據</td>
<td>5.憑據處理作業</td>
</tr>
<tr>
<td>6.銷售次數</td>
<td>6.銷售分析作業</td>
</tr>
</table>
## 使用案例圖 ##
<img src="http://i.imgur.com/ihg2Xyf.jpg" title="使用案例圖"/>

## 個別使用案例的描述 ##
<h3>「訂票基本資料作業」之使用案例</h3>
<table>
<tr>
<td width="170">使用案例名稱</td>
<td colspan="2">訂票基本資料作業</td>
</tr>
<tr>
<td>使用案例描述</td>
<td colspan="2">顧客查詢電影相關資訊，顧客啟動系統新增、修改資料</td>
</tr>
<tr>
<td>主要參與者</td>
<td colspan="2">顧客</td>
</tr>
<tr>
<td>利害關係人與目標</td>
<td colspan="2">顧客：能夠正確訂票</td>
</tr>
<tr>
<td>前置條件</td>
<td colspan="2">無</td>
</tr>
<tr>
<td>後置條件</td>
<td colspan="3">正確建立、修改或刪除基本資料</td>
</tr>
<tr>
<td rowspan="9">主要成功情節</td>
<td width="170">參與者</td>
<td width="170">系統</td>
</tr>
<tr>
<td>1.顧客要購買電影票時，進入作業畫面，並啟動新增按鍵
<br>inputCustomer()</td>
<td width="170">1.1系統開啟新增訂票基本資料作業畫面</td>
</tr>
<tr>
<td>2.顧客輸入基本資料，包括客戶姓名、客戶電話、客戶身分證號碼 
<br>checkcustomerItem(customerItem)</td>
<td>2.1系統檢查輸入格式，如果有誤要求重新輸入。檢查是否有重複客戶身分證號碼，顯示「重複客戶名稱」訊息</td>
</tr>
<tr>
<td>3.輸入完畢後，選取儲存鍵，或者取消鍵或者儲存離開鍵
<br>saveCustomerItem(customerRec)</td>
<td>3.1選取儲存按鍵，系統將客戶資料存入資料庫，並自動新增訂單紀錄。如果按取消鍵，則回至新增畫面。按離開鍵將新客戶資料存入資料庫，回到作業畫面</td>
</tr>
<tr>
<td colspan="2">系統重複1-3的動作</td>
</tr>
<tr>
<td>4.如果要進行修改，選取修改按鍵，並可以依據任一個欄位進行查詢，讀取所要修改紀錄。修改完，按確認鍵
<br>modifycustomerItem(customerName,customerPhone, customerID)
</td>
<td>4.1根據輸入欄位資料，搜尋客戶記錄，並顯示至畫面</td>
</tr>
<tr>
<td rowspan="2">5.如果要進行刪除，選取刪除鍵，並可以依據任一個欄位進行查詢，取所要刪除之客戶記錄
<br>deletecustomerItem(customerName, customerPhone, customerID)</td>
<td>5.1根據輸入欄位資料，儲存客戶記錄，如果按取消鍵，則回到訂票基本資料作業畫面</td>
</tr>
<tr>
<td>5.2出現確認訊息視窗，按確認進行刪除動作，按取消則不做刪除動作</td>
</tr>
<tr>
<td>5.3回到訂票基本資料作業畫面</td>
</tr>
<tr>
<td>例外情節</td>
<td colspan="2">*a.如果有任何欄位無法輸入，或是資料無法儲存，系統需要顯示警告訊息並中止輸入
<br>NoticeError()
</td>
</tr>
<tr>
<td>其他需求</td>
<td colspan="2">無</td>
</tr>
</table>

<h3>「處理訂單記錄作業」之使用案例</h3>
<table>
<tr>
<td width="170">使用案例名稱</td>
<td colspan="2">處理訂單記錄作業</td>
</tr>
<tr>
<td>使用案例描述</td>
<td colspan="2">由顧客端傳送訂單資料至系統、系統更新劃位狀況、同步更新至購票系統</td>
</tr>
<tr>
<td>主要參與者</td>
<td colspan="2">系統管理者、合作對象</td>
</tr>
<tr>
<td>利害關係人與目標</td>
<td colspan="2">超商人員：進行結帳及資料傳達</td>
</tr>
<tr>
<td>前置條件</td>
<td colspan="2">系統更新「現有座位及退票處理作業」、顧客輸入資料且輸出完畢</td>
</tr>
<tr>
<td>後置條件</td>
<td colspan="2">超商人員將顧客訂單傳送至系統</td>
</tr>
<tr>
<td rowspan="5">主要成功情節</td>
<td>參與者</td>
<td>系統</td>
</tr>
<tr>
<td width="170">1.顧客完成訂票手續並輸出資料<br>
inputOrder()<br>
getCustomerItem(customerName,customerPhone,customerID)<br>
addMovieItem(MovieID,MovieTime,MovieSeat,price,quantity)
</td>
<td width="170">1.1系統讀取顧客輸入之基本資料(顧客姓名、身分證字號、手機)及戲院名稱、電影時刻、座位、票價、數量<br>
1.2系統在顧客選擇戲院名稱後自動顯示該戲院電話、戲院地址
</td>
</tr>
<tr>
<td>2.顧客確認所顯示資料正確無誤後按下列印憑據，可至櫃台結帳<br>
checkOrderItem(orderItem)<br>
saveOrderItem(orderRec)<br>
</td>
<td>2.1畫面顯示顧客輸入的資料待顧客確認<br>
 2.2收到顧客按下的確認鍵後，系統編譯此訂單編號<br>
2.3超商人員將此訂單資料確認輸入後，列印出附有訂單編號之憑據<br>
2.4訂單紀錄中將記憶此訂單編號以及內容</td>
</tr>
<tr>
<td>3. 系統管理者登入管理介面，掌握訂單紀錄，並確認訂單有效後將資料更新給合作對象。<br>
</td>
<td>3.1顯示系統管理者登入介面，帶系統管理者輸入系統管理者姓名、管理編號、管理類別，系統將會自動寫入管理日期<br>
3.2訂單記錄的資料由系統管理者進行座位控管、電影控管、場次控管後儲存<br>
3.3資料寫進管理紀錄中，日後查詢、校正時能迅速找到該筆資料</td>
</tr>
<tr>
<td>4.合作對象收到更新資料後系統將現有座位重新顯示於合作對象的使用介面中，便於現場購票顧客</td>
<td>4.1合作對象使用的介面將會自動出現新訂單內容，確認後系統自動更新現有座位</td>
</tr>
<tr>
<td>例外情節</td>
<td colspan="2">*a.如果有兩個使用者同時選取相同狀況且同時輸出資料，系統無法判別優先順序，則會出現錯誤訊息，警告使用者選取座位錯誤，可能有衝突。</td>
</tr>
<tr>
<td>其他需求</td>
<td colspan="2">無</td>
</tr>
</table>

<h3>「現有座位及退票處理作業」之使用案例</h3>
<table>
<tr>
<td width="170">使用案例名稱</td>
<td colspan="2">現有座位及退票處理作業</td>
</tr>
<tr>
<td>使用案例描述</td>
<td colspan="2">系統內必須有效控制座位已被選取、被購買等狀態，如有顧客退票應立即更新座位狀態，使座位能在最短時間後重新出售。</td>
</tr>
<tr>
<td>主要參與者</td>
<td colspan="2">超商人員、線上更新人員、顧客、合作對象</td>
</tr>
<tr>
<td>利害關係人與目標</td>
<td colspan="2">超商人員：處理顧客退票程序，並按流程輸入至系統<br>
線上更新人員：將顧客退票所空出位置，更新至系統，使其位置成為有效座位。<br>
顧客：可透過現有座位表，選取自己想要的位置，或是重新登入取消購票。<br>
合作對象：合作戲院必須隨時掌握現有座位狀況，以免電腦程式當機、錯誤，能立即連絡處理此狀況</td>
</tr>
<tr>
<td>前置條件</td>
<td colspan="2">無</td>
</tr>
<tr>
<td>後置條件</td>
<td colspan="2">連結「處理訂單紀錄」由刪除的座位找出該筆紀錄予以刪除。<br>
getSeat()
</td>
</tr>
<tr>
<td rowspan="5">主要成功情節</td>
<td>參與者</td>
<td>系統</td>
</tr>
<tr>
<td width="170">1.顧客於超商系統中登入基本資料。</td>
<td width="170">1.1系統畫面顯式登入界面。<br>
1.2顧客輸入完成後，系統讀取資料找尋個人紀錄。
</td>
</tr>
<tr>
<td>2.顧客選擇「現有座位及退票」進入畫面。</td>
<td>2.1系統將重新整理資料後，顯示現有座位表</td>
</tr>
<tr>
<td>3.顧客選擇預購買之座位，選取戲院名稱、座位、場次、電影時間、票價、數量，並輸出資料。 顧客列印出「憑據」並將憑據交給超商人員進行結帳拿取「票劵」。<br>
inputTicket(TicketSeat, TicketTName, TicketScreenings, TicketTime, TicketPrice, TicketQ)</td>
<td>3.1系統將顧客預購買之座位的狀態改為保留中<br>
3.2系統將畫面轉換顯示該筆訂單詳細資料待顧客確認。<br>
3.3顧客確認後系統輸出資料後該筆座位狀態改為已預訂，產生該筆訂單紀錄<br>
3.4印出票劵給顧客<br>
3.5系統將資料更新後傳送至合作對象端</td>
</tr>
<tr>
<td>4.顧客若以付款完成後預退票，至超商櫃檯處理。<br>
delete(OrderID)</td>
<td>4.1超商人員開啟系統，將此訂單編號輸入後能查詢該筆訂單資料，可從選項中點選「退票」。<br>
4.2系統收到「退票」信息後，將刪除該筆訂單編號<br>
4.3系統將該位置重新寫入「現有座位」</td>
</tr>
<tr>
<td>例外情節</td>
<td colspan="2">無</td>
</tr>
<tr>
<td>其他需求</td>
<td colspan="2">無</td>
</tr>
</table>

<h3>「電影基本資料作業」之使用案例</h3>
<table>
<tr>
<td width="170">使用案例名稱</td>
<td colspan="2">電影基本資料作業‧</td>
</tr>
<tr>
<td>使用案例描述</td>
<td colspan="2">合作對象輸入帳號密碼進入合作對象專屬頁面，輸入最新的電影資訊，按下儲存後回傳紀錄給系統管理者‧。</td>
</tr>
<tr>
<td>主要參與者</td>
<td colspan="2">合作對象／系統管理者‧</td>
</tr>
<tr>
<td>利害關係人與目標</td>
<td colspan="2">合作對象:立即的更新及修改電影資訊<br>
系統管理者：接收合作對象所輸入的電影資訊‧</td>
</tr>
<tr>
<td>前置條件</td>
<td colspan="2">無</td>
</tr>
<tr>
<td>後置條件</td>
<td colspan="2">正確建立、修改或刪除電影基本資料。</td>
</tr>
<tr>
<td rowspan="6">主要成功情節</td>
<td>參與者</td>
<td>系統</td>
</tr>
<tr>
<td width="170">1. 當合作對象上映新的電影時，合作對象需登入電影基本資料畫面，選取更新按鍵，並可以依據任一個欄位進行查詢，讀取所要更新之電影院進行資料更新‧ getNewMovieRec()
<br>getNewMovieRec()
</td>
<td width="170">1.1系統開啟更新電影基本資料畫面</td>
</tr>
<tr>
<td>2. 合作對象更新電影基本資料，包括電影名稱、分級、片長、時刻及座位‧
<br>updateNewMovieRec(newMovieID, newMovieLevel, newMovieLong, newMovieTime, newMovieSeat)
</td>
<td>2.1系統檢查更新資料格式，有錯誤時，系統會要求重新輸入<br> 2.2系統檢查是否有重複電影名稱，如果有則顯示「此部電影上映中」</td>
</tr>
<tr>
<td>3. 系統自動檢查是否為同一部電影，如果是則合作對象選擇取消更新，若否則繼續更新之
<br>checkNewMovieItem(newMovieID, newMovieLevel, newMovieLong, newMovieTime, newMovieSeat)。
</td>
<td>3.1選擇「取消更新」回到更新畫面，如果選擇「繼續更新」則繼續輸入動作</td>
</tr>
<tr>
<td>4. 更新完畢後，選取即時更新儲存按鍵 或離開鍵‧
<br>saveNewMovieRec(newMovieID, newMovieLevel, newMovieLong, newMovieTime, newMovieSeat)
</td>
<td>4.1選取儲存按鍵，系統將電影資料存入資料庫，將其資料即時更新到客戶端畫面及將記錄回傳給系統管理者‧如果選取了取消鍵，則回至更新畫面‧如果選擇離開鍵，則會離開電影基本資料作業畫面，其客戶端的資料會呈現更新前的資料‧</td>
</tr>
<td colspan="2">重複1-4的動作</td>‧
</tr>
<tr>
<td>例外情節</td>
<td colspan="2">*a. 如果輸入資料不齊全，系統需要顯示警告訊息並提醒合作對象將其資料輸入完成否則無法儲存完成更新‧
<br>NoticeError()</td>
</tr>
<tr>
<td>其他需求</td>
<td colspan="2">無</td>
</tr>
</table>

<h3>「憑據處理作業」之使用案例</h3>
<table>
<tr>
<td width="170">使用案例名稱</td>
<td colspan="2">憑據處理作業</td>
</tr>
<tr>
<td>使用案例描述</td>
<td colspan="2">顧客輸入其基本訂票資訊後依機器印出之流水編號憑據至櫃台交由店員結帳</td>
</tr>
<tr>
<td>主要參與者</td>
<td colspan="2">顧客、超商店員</td>
</tr>
<tr>
<td width="170">利害關係人與目標</td>
<td colspan="2">1.可以用條碼掃描，加快結帳速度</td>
</tr>
<tr>
<td>前置條件</td>
<td colspan="2">無</td>
</tr>
<tr>
<td>後置條件</td>
<td colspan="2">無</td>
</tr>
<tr>
<td rowspan="6">主要成功情節</td>
<td>參與者</td>
<td>系統</td>
</tr>
<tr>
<td width="170">1. 顧客在家中或到超商售票機前輸入訂票資訊<br>
inputOrder()
</td>
<td width="170">1.1 系統登入畫面</td>
</tr>
<tr>
<td>2. 顧客依訂票資訊獲得憑據之流水編號<br>
getNumber()</td>
<td>2.1 螢幕顯示售票資訊及憑據之流水編號並印出</td>
</tr>
<tr>
<td>3. 顧客拿印出之憑據至櫃檯結帳</td>
<td>3.1店員用條碼掃描憑據並把售票資訊傳至資料庫建立訂票紀錄</td>
</tr>
<tr>
<td>4. 若要新增其他選項則重複1~3動作</td>
<td>4.1 系統重複以上動作</td>
</tr>
<tr>
<td>5. 顧客退票時依印出之憑據至櫃台進行退票作業<br>
deleteOrder()</td>
<td>5.1 系統進入資料庫之畫面並刪除該人的售票資訊</td>
</tr>
<tr>
<td>例外情節</td>
<td colspan="2">無</td>
</tr>
<tr>
<td>其他需求</td>
<td colspan="2">無</td>
</tr>
</table>

<h3>「銷售分析作業」之使用案例</h3>
<table>
<tr>
<td width="170">使用案例名稱</td>
<td colspan="2">銷售分析作業</td>
</tr>
<tr>
<td>使用案例描述</td>
<td colspan="2">管理階層透過此作業系統對銷售狀況進行掌握並且擬定相關銷售策略</td>
</tr>
<tr>
<td>主要參與者</td>
<td colspan="2">管理階層</td>
</tr>
<tr>
<td width="170">利害關係人與目標</td>
<td colspan="2">1. 進行策略規劃<br>
2.分析銷售狀況</td>
</tr>
<tr>
<td>前置條件</td>
<td colspan="2">無</td>
</tr>
<tr>
<td>後置條件</td>
<td colspan="2">連結「處理訂單紀錄」由刪除的座位找出該筆紀錄予以刪除。</td>
</tr>
<tr>
<td rowspan="5">主要成功情節</td>
<td>參與者</td>
<td>系統</td>
</tr>
<tr>
<td width="170">1.總裁(管理階層)進入銷售分析作業起始畫面並登入自己的帳號開始進行銷售額的查詢。<br>
getNumber(profit)
</td>
<td width="170">1.1系統開啟銷售分析作業畫面</td>
</tr>
<tr>
<td>2.總裁依各個合作對象(電影院)及超商的銷售紀錄、銷售排行、賣出時間進行查詢<br>
checkProfit()
</td>
<td>2.1系統依照各個選項的欄位列出使用者所需的資訊</td>
</tr>
<tr>
<td>3.總裁進行登出帳號</td>
<td>3.1系統開啟帳號登入畫面</td>
</tr>
<tr>
<td>4. 透過業績的查詢對各個合作對象銷售狀況進行掌握並擬定策略</td>
<td></td>
</tr>
<tr>
<td>例外情節</td>
<td colspan="2">無</td>
</tr>
<tr>
<td>其他需求</td>
<td colspan="2">無</td>
</tr>
</table>

## 個別使用案例的活動圖 ##
<h2>「訂票基本資料作業」之活動圖</h2>
<img src="http://i.imgur.com/VLJA2YO.png" title="訂票基本資料作業之活動圖"/>

<h2>「處理訂單紀錄作業」之活動圖</h2>
<img src="http://i.imgur.com/EVqVAHe.jpg" title="處理訂單紀錄作業之活動圖"/>

<h2>「現有座位及退票處理作業」之活動圖</h2>
<img src="http://i.imgur.com/kWJYMFO.jpg" title="現有座位及退票處理作業之活動圖"/>

<h2>「電影基本資料作業」之活動圖</h2>
<img src="http://i.imgur.com/QgmtWva.jpg" title="電影基本資料作業之活動圖"/>

<h2>「憑據處理作業」之活動圖</h2>
<img src="http://i.imgur.com/JXFjJzV.jpg" title="憑據處理作業業之活動圖"/>

<h2>「銷售分析作業」之活動圖</h2>
<img src="http://i.imgur.com/jTKbZ4L.jpg" title="銷售分析作業之活動圖"/>


## 每個使用案例的名詞與概念類別列舉表 ##
<h3>「訂票基本資料作業」之概念類別列舉表</h3>
<table>
<tr>
<td width="100">名詞</td>
<td width="200">原因</td>
<td width="170">結果(是否為概念類別)</td>
</tr>
<tr>
<td>顧客</td>
<td>本系統需要記錄顧客的基本資料</td>
<td>是</td>
</tr>
<tr>
<td>身分證字號</td>
<td>顧客屬性</td>
<td>否</td>
</tr>
<tr>
<td>顧客姓名</td>
<td>顧客屬性</td>
<td>否</td>
</tr>
<tr>
<td>手機</td>
<td>顧客屬性</td>
<td>否</td>
</tr>
<tr>
<td>訂單紀錄</td>
<td>由顧客輸入的資料所產生的訂單紀錄</td>
<td>是</td>
</tr>
<tr>
<td>訂單編號</td>
<td>訂單紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>戲院名稱</td>
<td>訂單紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>電影名稱</td>
<td>訂單紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>戲院地址</td>
<td>訂單紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>場次</td>
<td>訂單紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>座位</td>
<td>訂單紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>價格</td>
<td>訂單紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>數量</td>
<td>訂單紀錄屬性</td>
<td>否</td>
</tr>
</table>

<h3>「處理訂單紀錄」之概念類別列舉表</h3>
<table>
<tr>
<td width="100">名詞</td>
<td width="200">原因</td>
<td width="170">結果(是否為概念類別)</td>
</tr>
<tr>
<td>顧客</td>
<td>本系統需要記錄顧客的基本資料</td>
<td>是</td>
</tr>
<tr>
<td>合作對象</td>
<td>本系統需要將顧客訂單紀錄即時回傳給合作對象</td>
<td>是</td>
</tr>
<tr>
<td>訂單紀錄</td>
<td>由顧客輸入的資料所產生的訂單紀錄</td>
<td>是</td>
</tr>
<tr>
<td>系統管理者</td>
<td>為顧客及合作對象之間的連結個體</td>
<td>是</td>
</tr>
<tr>
<td>管理紀錄</td>
<td>系統管理者作業時輸入的基本資料</td>
<td>是</td>
</tr>
<tr>
<td>身份證字號</td>
<td>顧客屬性</td>
<td>否</td>
</tr>
<tr>
<td>顧客姓名</td>
<td>顧客屬性</td>
<td>否</td>
</tr>
<tr>
<td>手機</td>
<td>顧客屬性</td>
<td>否</td>
</tr>
<tr>
<td>戲院名稱</td>
<td>合作對象屬性<br>訂單紀錄屬性</td>
<td>是(合作對象)<br>否(訂單紀錄)</td>
</tr>
<tr>
<td>戲院電話</td>
<td>合作對象屬性</td>
<td>否</td>
</tr>
<tr>
<td>戲院編號</td>
<td>合作對象屬性</td>
<td>否</td>
</tr>
<tr>
<td>訂單編號</td>
<td>訂單紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>座位</td>
<td>訂單紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>場次</td>
<td>訂單紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>電影名稱</td>
<td>訂單紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>戲院地址</td>
<td>合作對象屬性<br>訂單紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>價格</td>
<td>訂單紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>數量</td>
<td>訂單紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>系統管理者姓名</td>
<td>系統管理者屬性</td>
<td>否</td>
</tr>
<tr>
<td>管理編號</td>
<td>系統管理者屬性</td>
<td>否</td>
</tr>
<tr>
<td>管理類別</td>
<td>系統管理者屬性</td>
<td>否</td>
</tr>
<tr>
<td>管理日期</td>
<td>管理紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>座位控管</td>
<td>管理紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>場次控管</td>
<td>管理紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>電影控管</td>
<td>管理紀錄屬性</td>
<td>否</td>
</tr>
</table>

<h3>「現有座位及退票處理作業」之概念類別列舉表</h3>
<table>
<tr>
<td width="100">名詞</td>
<td width="200">原因</td>
<td width="170">結果(是否為概念類別)</td>
</tr>
<tr>
<td>超商系統</td>
<td>本系統顯示於超商機器時的畫面</td>
<td>否</td>
</tr>
<tr>
<td>登入界面</td>
<td>超商機器中給顧客輸入基本資料的畫面</td>
<td>否</td>
</tr>
<tr>
<td>個人紀錄</td>
<td>當顧客送出個人紀錄後，系統將搜尋此項資料是否曾有交易紀錄。</td>
<td>否</td>
</tr>
<tr>
<td>現有座位及退票</td>
<td>本系統介面，供顧客瀏覽現有的座位。若是顧客曾有交易完成的票劵，可從此畫面中點選退票。</td>
<td>否</td>
</tr>
<tr>
<td>現有座位表</td>
<td>系統後端管控座位情況的憑據</td>
<td>否</td>
</tr>
<tr>
<td>保留中</td>
<td>當顧客已選取此座位但尚未結帳時，系統將此做位狀態更換成保留中，以防重複選位的狀況。</td>
<td>否</td>
</tr>
<tr>
<td>訂單編號</td>
<td>訂單紀錄屬性<br>退票紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>戲院名稱</td>
<td>訂單紀錄屬性<br>
票劵屬性<br>
合作對象屬性</td>
<td>否</td>
</tr>
<tr>
<td>座位</td>
<td>訂單紀錄屬性<br>票劵屬性</td>
<td>否</td>
</tr>
<tr>
<td>場次</td>
<td>訂單紀錄屬性<br>票劵屬性</td>
<td>否</td>
</tr>
<tr>
<td>電影時間</td>
<td>訂單紀錄屬性<br>票劵屬性</td>
<td>否</td>
</tr>
<tr>
<td>票價</td>
<td>訂單紀錄屬性<br>票劵屬性</td>
<td>否</td>
</tr>
<tr>
<td>數量</td>
<td>訂單紀錄屬性<br>票劵屬性</td>
<td>否</td>
</tr>
<tr>
<td>訂單紀錄</td>
<td>系統用來紀錄每一筆資料的詳細狀況</td>
<td>是</td>
</tr>
<tr>
<td>票劵</td>
<td>顧客結帳後產生出有效的電影票劵</td>
<td>是</td>
</tr>
<tr>
<td>戲院地址</td>
<td>合作對象屬性<br>訂單紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>合作對象</td>
<td>使用本系統的合作戲院</td>
<td>是</td>
</tr>
<tr>
<td>超商人員</td>
<td>協助顧客結帳及退票的媒介</td>
<td>是</td>
</tr>
<tr>
<td>退票紀錄</td>
<td>系統寫入顧客退票的資料更心狀態及備查驗</td>
<td>是</td>
</tr>
</table>

<h3>「電影基本資料」之概念類別列舉表</h3>
<table>
<tr>
<td width="100">名詞</td>
<td width="200">原因</td>
<td width="170">結果(是否為概念類別)</td>
</tr>
<tr>
<td>合作對象</td>
<td>本系統需要合作對象回傳最新的電影資訊及即時的座位更新狀況</td>
<td>是</td>
</tr>
<tr>
<td>戲院名稱</td>
<td>合作對象的基本資料，重要。</td>
<td>是</td>
</tr>
<tr>
<td>戲院地址</td>
<td>合作對象屬性。</td>
<td>否</td>
</tr>
<tr>
<td>戲院電話</td>
<td>合作對象屬性。</td>
<td>否</td>
</tr>
<tr>
<td>戲院編號</td>
<td>合作對象屬性</td>
<td>否</td>
</tr>
<tr>
<td>更新時間</td>
<td>更新紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>更新座位</td>
<td>更新紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>更新場次</td>
<td>更新紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>更新電影</td>
<td>更新紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>上傳更新紀錄之戲院</td>
<td>更新紀錄屬性</td>
<td>否</td>
</tr>
</table>

<h3>「憑據處理作業」之概念類別列舉表</h3>
<table>
<tr>
<td width="100">名詞</td>
<td width="200">原因</td>
<td width="170">結果(是否為概念類別)</td>
</tr>
<tr>
<td>顧客</td>
<td>本系統需要紀錄顧客的基本資料</td>
<td>是</td>
</tr>
<tr>
<td>訂票紀錄</td>
<td>由顧客輸入資料所產生</td>
<td>是</td>
</tr>
<tr>
<td>超商店員</td>
<td>店員須把顧客之流水編號匯入</td>
<td>否</td>
</tr>
<tr>
<td>流水編號</td>
<td>憑據屬性</td>
<td>否</td>
</tr>
<tr>
<td>條碼</td>
<td>訂單紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>憑據</td>
<td>紀錄訂單紀錄之單據</td>
<td>是</td>
</tr>
</table>

<h3>「銷售分析作業」之概念類別列舉表</h3>
<table>
<tr>
<td width="100">名詞</td>
<td width="200">原因</td>
<td width="170">結果(是否為概念類別)</td>
</tr>
<tr>
<td>帳號</td>
<td>管理者屬性</td>
<td>否</td>
</tr>
<tr>
<td>職位</td>
<td>管理者屬性</td>
<td>否</td>
</tr>
<tr>
<td>銷售額</td>
<td>銷售紀錄屬性</td>
<td>否</td>
</tr>
<tr>
<td>銷售紀錄</td>
<td>各個合作對象及超商匯入的銷售資訊所產生</td>
<td>是</td>
</tr>
<tr>
<td>銷售排行</td>
<td>由合作對象匯入資料至系統</td>
<td>否</td>
</tr>
<tr>
<td>管理者</td>
<td>本系統需要紀錄管理階層的基本資料</td>
<td>是</td>
</tr>
<tr>
<td>賣出時間</td>
<td>銷售紀錄屬性</td>
<td>否</td>
</tr>
</table>

## 每個使用案例的初步類別圖 ##
<h3>訂票基本資料作業之初步類別圖</h3>
<img src="http://i.imgur.com/NSSxRMd.png" title="訂票基本資料作業之初部類別圖"/>

<h3>處理訂單紀錄之初步類別圖</h3>
<img src="http://i.imgur.com/KpjqdPx.jpg" title="處理訂單紀錄之初部類別圖"/>

<h3>現有座位及退票處理作業之初步類別圖</h3>
<img src="http://i.imgur.com/IXc0J4E.jpg" title="現有座位及退票處理作業之初部類別圖"/>

<h3>電影基本資料作業之初步類別圖</h3>
<img src="http://i.imgur.com/5N1uhJs.jpg" title="電影基本資料作業之初部類別圖"/>

<h3>憑據處理作業之初步類別圖</h3>
<img src="http://i.imgur.com/JqXcr8R.png" title="憑據處理作業之初部類別圖"/>

<h3>銷售分析作業之初步類別圖</h3>
<img src="http://i.imgur.com/KZPH5bT.png" title="銷售分析作業之初部類別圖"/>


## 最後整個系統的初步類別圖 ##
<img src="http://i.imgur.com/nsuCnuU.png" title="最後整個系統的初步類別圖"/>

## 最後整個系統的強韌圖 ##
<img src="http://i.imgur.com/ZGWCPvv.png" title="最後整個系統的強韌圖"/>

## 每個名稱事件之合約 ##
<h4>inputCustomer()合約</h4>
<table>
<tr>
<td width="170">合約：</td>
<td>inputCustomer()</td>
</tr>
<tr>
<td>操作：</td>
<td>inputCustomer()</td>
</tr>
<tr>
<td>交戶參照：</td>
<td>訂票基本資料作業</td>
</tr>
<tr>
<td>前置條件：</td>
<td>存在類別Customer之實例newCustomer</td>
</tr>
<tr>
<td rowspan="3">後置條件：</td>
<td>-檢查並確認實例newCustomer之customerName、customerPhone、customerID屬性之起始值為空白</td>
</tr>
<tr>
<td>-給定實例</td>
</tr>
<tr>
<td>-回傳整筆訂票基本資料作業</td>
</tr>
</table>

<h4>modifycustomerItem()合約</h4>
<table>
<tr>
<td width="150">合約：</td>
<td>modifycustomerItem()</td>
</tr>
<tr>
<td>操作：</td>
<td>modifycustomerItem(customerName,customerPhone,customerID)</td>
</tr>
<tr>
<td>交戶參照：</td>
<td>訂票基本資料作業</td>
</tr>
<tr>
<td>前置條件：</td>
<td>存在類別Customer之實例newCustomer</td>
</tr>
<tr>
<td rowspan="2">後置條件：</td>
<td>-根據customerName或customerPhone或customerID讀取訂票基本資料作業customerRec,並存入至類別Customer之屬性中</td>
</tr>
<tr>
<td>-回傳customerRec</td>
</tr>
</table>

<h4>inputOrder()合約</h4>
<table>
<tr>
<td width="170">合約：</td>
<td>inputOrder()</td>
</tr>
<tr>
<td>操作：</td>
<td>inputOrder()</td>
</tr>
<tr>
<td>交戶參照：</td>
<td>處理訂單作業</td>
</tr>
<tr>
<td>前置條件：</td>
<td>存在類別inputOrder之實例newOrder</td>
</tr>
<tr>
<td rowspan="3">後置條件：</td>
<td>-建立類別inputOrder之實例Od</td>
</tr>
<tr>
<td>-實例Od與實例newOrder形成關聯</td>
</tr>
<tr>
<td>- 給定實例newOrder之屬性newOrderNu 編號</td>
</tr>
</table>

<h4>getcustomerItem ()合約</h4>
<table>
<tr>
<td width="170">合約：</td>
<td>getcustomerItem ()</td>
</tr>
<tr>
<td>操作：</td>
<td>getcustomerItem(customerName,customerPhone,customerID)</td>
</tr>
<tr>
<td>交戶參照：</td>
<td>處理訂單作業</td>
</tr>
<tr>
<td>前置條件：</td>
<td>存在類別getcustomerItem 之實例newcustomerItem</td>
</tr>
<tr>
<td rowspan="3">後置條件：</td>
<td>-建立類別getcustomerItem之實例ci</td>
</tr>
<tr>
<td>-實例ci與實例getcustomerItem形成關聯</td>
</tr>
<tr>
<td>-給定實例getcustomerItem之屬性customerName顧客姓名,customerPhone顧客電話,customerID顧客身分證字號</td>
</tr>
</table>

<h4>addMovieItem()合約</h4>
<table>
<tr>
<td width="170">合約：</td>
<td>addMovieItem()</td>
</tr>
<tr>
<td>操作：</td>
<td>addMovieIte(MovieID,MovieTime,MovieSeat,price,quantity)</td>
</tr>
<tr>
<td>交戶參照：</td>
<td>處理訂單作業</td>
</tr>
<tr>
<td>前置條件：</td>
<td>存在類別addMovieItem 之實例newaddMovieItem</td>
</tr>
<tr>
<td rowspan="9">後置條件：</td>
<td>-建立類別addMovieItem之實例ami</td>
</tr>
<tr>
<td>-實例ami與實例addMovieItem形成關聯</td>
</tr>
<tr>
<td>-給定實例addMovieItem之屬性MovieID電影名稱,MovieTime電影時刻,MovieSeat座位,price票價,quantity數量</td>
</tr>
<tr>
<td>-將MovieID 存入 ami. MovieID</td>
</tr>
<tr>
<td>-將MovieTime 存入 ami. MovieTime</td>
</tr>
<tr>
<td>-將MovieSeat 存入 ami. MovieSeat</td>
</tr>
<tr>
<td>-將price 存入 ami. price</td>
</tr>
<tr>
<td>-將quantity存入 ami. quantity</td>
</tr>
<tr>
<td>- 實例addMovieItem根據MovieID,MovieTime,MovieSeat,price,quantity讀取處理訂單作業存入newmovieitem</td>
</tr>
</table>

<h4>checkOrderItem()合約</h4>
<table>
<tr>
<td width="150">合約：</td>
<td>checkOrderItem()</td>
</tr>
<tr>
<td>操作：</td>
<td>checkOrderItem(orderItem)</td>
</tr>
<tr>
<td>交戶參照：</td>
<td>電影基本資料作業</td>
</tr>
<tr>
<td>前置條件：</td>
<td>回傳MovieID,MovieTime, MovieSeat,price,quantity</td>
</tr>
<tr>
<td rowspan="3">後置條件：</td>
<td>-根據MovieID尋找newmovieitem實例，並形成關聯</td>
</tr>
<tr>
<td>-根據MovieTime尋找newmovieitem實例，並形成關聯</td>
</tr>
<tr>
<td>-回傳newmovieitem實例</td>
</tr>
</table>

<h4>saveOrderItem() 合約</h4>
<table>
<tr>
<td width="150">合約：</td>
<td>saveOrderItem()</td>
</tr>
<tr>
<td>操作：</td>
<td>操作：saveOrderItem(orderRec)</td>
</tr>
<tr>
<td>交戶參照：</td>
<td>處理訂單作業</td>
</tr>
<tr>
<td>前置條件：</td>
<td>存在類別saveOrderItem之實例newSaveOrderItem</td>
</tr>
<tr>
<td>後置條件：</td>
<td>-回傳newSaveOrderItem紀錄至實例OrderItem</td>
</tr>
</table>

<h4>getSeat()合約</h4>
<table>
<tr>
<td width="150">合約：</td>
<td>getSeat()</td>
</tr>
<tr>
<td>操作：</td>
<td>getSeat()</td>
</tr>
<tr>
<td>交戶參照：</td>
<td>現有座位及退票處理作業</td>
</tr>
<tr>
<td>前置條件：</td>
<td>存在類別getSeat之實例newSeat</td>
</tr>
<tr>
<td rowspan="3">後置條件：</td>
<td>-建立類別Seat之實例St</td>
</tr>
<tr>
<td>-實例St與實例newSeat形成關聯</td>
</tr>
<tr>
<td>-給定實例newSeat之屬性newSeatNu 編號</td>
</tr>
</table>

<h4>inputTicket()</h4>
<table>
<tr>
<td width="150">合約：</td>
<td>inputTicket()</td>
</tr>
<tr>
<td>操作：</td>
<td>inputTicket(TicketSeat, TicketTName, TicketScreenings, TicketTime,TicketPrice, TicketQ)</td>
</tr>
<tr>
<td>交戶參照：</td>
<td>現有座位及退票處理作業</td>
</tr>
<tr>
<td>前置條件：</td>
<td>存在類別getSeat之實例newSeat</td>
</tr>
<tr>
<td rowspan="7">後置條件：</td>
<td>-將TicketSeat存入st.TicketSeat</td>
</tr>
<tr>
<td>-將TicketTName存入st. TicketTName</td>
</tr>
<tr>
<td>-將TicketScreenings存入st. TicketScreenings</td>
</tr>
<tr>
<td>-將TicketTime存入st. TicketTime</td>
</tr>
<tr>
<td>-將TicketPrice存入st. TicketPrice</td>
</tr>
<tr>
<td>-將TicketQ存入st. TicketQ</td>
</tr>
<tr>
<td>-回傳newSeat紀錄至實例Seat</td>
</tr>
</table>

<h4>delete()</h4>
<table>
<tr>
<td width="150">合約：</td>
<td>delete()</td>
</tr>
<tr>
<td>操作：</td>
<td>delete(OrderID)</td>
</tr>
<tr>
<td>交戶參照：</td>
<td>現有座位及退票處理作業</td>
</tr>
<tr>
<td>前置條件：</td>
<td>存在類別delete之實例delete</td>
</tr>
<tr>
<td rowspan="2">後置條件：</td>
<td>-根據newseat實例尋找出TicketSeat, TicketTName,TicketScreenings,TicketTime, TicketPrice, TicketQ 將其資料從newseat中刪除</td>
</tr>
<tr>
<td>-傳newSeat紀錄至實例Seat</td>
</tr>

</table>

<h4>getNewMovieItem()合約</h4>
<table>
<tr>
<td width="150">合約：</td>
<td>getNewMovieItem()</td>
</tr>
<tr>
<td>操作：</td>
<td>getNewMovieItem()</td>
</tr>
<tr>
<td>交戶參照：</td>
<td>電影基本資料作業</td>
</tr>
<tr>
<td>前置條件:</td>
<td>存在類別movieItem之實例newMovieItem</td>
</tr>
<tr>
<td rowspan="3">後置條件：</td>
<td>- 建立類別movieItem之實例mi</td>
</tr>
<tr>
<td>- 實例mi與實例newmovieitem形成關聯</td>
</tr>
<tr>
<td>- 給定實例newmovieitem之屬性newMovieID最新電影名稱,newMovieLevel級別,newMovieLong片長,newMovieTime時刻,newMovieSeat座位</td>
</tr>
</table>

<h4>updateNewMovieItem()合約</h4>
<table>
<tr>
<td width="150">合約：</td>
<td>updateNewMovieItem()</td>
</tr>
<tr>
<td>操作：</td>
<td>updateNewMovieRec(newMovieID,newMovieLevel,newMovieLong,newMovieTime,newMovieSeat)</td>
</tr>
<tr>
<td>交戶參照：</td>
<td>電影基本資料作業</td>
</tr>
<tr>
<td>前置條件：</td>
<td>已開啟:Movie物件</td>
</tr>
<tr>
<td rowspan="6">後置條件：</td>
<td>-將newMovieID存入mi.movieID</td>
</tr>
<tr>
<td>-將newMovieLevel存入mi. movieLevel</td>
</tr>
<tr>
<td>-將newMovieLong存入mi.movieLong</td>
</tr>
<tr>
<td>-將newMovieTime存入mi. movieTime</td>
</tr>
<tr>
<td>- 將newMovieSeat存入mi.movieSeat</td>
</tr>
<tr>
<td>-實例newmovieitem根據newMovieID,newMovieLevel,newMovieLong,newMovieTime,newMovieSeat讀取資料庫電影基本資料newMovieRec存入實例newmovieitem</td>
</tr>
</table>

<h4>checkNewMovieItem()合約</h4>
<table>
<tr>
<td width="150">合約：</td>
<td>checkNewMovieItem()</td>
</tr>
<tr>
<td>操作：</td>
<td>checkNewMovieItem(newMovieID,newMovieLevel,newMovieLong,newMovieTime,newMovieSeat)</td>
</tr>
<tr>
<td>交戶參照：</td>
<td>電影基本資料作業</td>
</tr>
<tr>
<td>前置條件：</td>
<td>回傳newMovieID,newMovieLevel,newMovieLong,newMovieTime,newMovieSeat</td>
</tr>
<tr>
<td rowspan="3">後置條件：</td>
<td>- 根據newMovieID尋找newMovieSpec實例，並形成關聯</td>
</tr>
<tr>
<td>- 根據newMovieID尋找newMovie實例，並形成關聯</td>
</tr>
<tr>
<td>- 回傳newmovieitem之newMovieID,newMovieLevel,newMovieLong,newMovieTime,newMovieSeat屬性值</td>
</tr>
</table>

<h4>saveNewMovieRec()合約</h4>
<table>
<tr>
<td width="150">合約：</td>
<td>saveNewMovieRec()</td>
</tr>
<tr>
<td>操作：</td>
<td>saveNewMovieRec(newMovieID,newMovieLevel,newMovieLong,newMovieTime,newMovieSeat)</td>
</tr>
<tr>
<td>交戶參照：</td>
<td>電影基本資料作業</td>
</tr>
<tr>
<td>前置條件：</td>
<td>存在類別movieItem之實例newMovieItem</td>
</table>

<h4>inputOrder()合約</h4>
<table>
<tr>
<td width="150">合約：</td>
<td>inputOrder()</td>
</tr>
<tr>
<td>操作：</td>
<td>inputOrder()</td>
</tr>
<tr>
<td>交戶參照：</td>
<td>憑據處理作業</td>
</tr>
<tr>
<td>前置條件：</td>
<td>存在類別Order之實例newOreder</td>
</tr>
<tr>
<td rowspan="2">後置條件：</td>
<td>-給定實例newOrder之屬性orderID最新流水編號</td>
</tr>
<tr>
<td>-回傳OrderID</td>
</tr>
</table>

<h4>getNumber()合約</h4>
<table>
<tr>
<td width="150">合約：</td>
<td>getNumber()</td>
</tr>
<tr>
<td>操作：</td>
<td>getNumber(seatsID)</td>
</tr>
<tr>
<td>交戶參照：</td>
<td>憑據處理作業</td>
</tr>
<tr>
<td>前置條件：</td>
<td>已開啟Order物件</td>
</tr>
<tr>
<td rowspan="4">後置條件：</td>
<td>-建立類別Number的實例number</td>
</tr>
<tr>
<td>-實例number與實例newOrder形成關聯</td>
</tr>
<tr>
<td>-實例number根據seatID讀取資料庫憑據資料numberRec存入實例number</td>
</tr>
<td>-回傳numberRec紀錄</td>
</tr>
</table>

<h4>saveNumber()合約</h4>
<table>
<tr>
<td width="150">合約：</td>
<td>saveNumber()</td>
</tr>
<tr>
<td>操作：</td>
<td>saveNumber(seatsID)</td>
</tr>
<tr>
<td>交戶參照：</td>
<td>憑據處理作業</td>
</tr>
<tr>
<td>前置條件：</td>
<td>存在類別Order之實例newOrder</td>
</tr>
<tr>
<td>後置條件：</td>
<td>-回傳newOrder紀錄至實例number</td>
</tr>
</table>

<h4>checkProfit()合約</h4>
<table>
<tr>
<td width="150">合約：</td>
<td>checkProfit()</td>
</tr>
<tr>
<td>操作：</td>
<td>checkProfit()</td>
</tr>
<tr>
<td>交戶參照：</td>
<td>銷售分析作業</td>
</tr>
<tr>
<td>前置條件：</td>
<td>已開啟Order物件</td>
</tr>
<tr>
<td rowspan="2">後置條件：</td>
<td>-給定實例newOrder之屬性orderID最新銷售業績編號</td>
</tr>
<tr>
<td>-回傳OrderID</td>
</tr>
</table>
## 使用案例之系統循序圖 ##
<h3>「訂票基本資料作業」之系統循序圖</h3>
<img src="http://i.imgur.com/xgEXcID.png" title="訂票基本資料作業之系統循序圖"/>

<h3>「訂票基本資料作業」之完整循序圖</h3>
<img src="http://i.imgur.com/1wu6FwS.png" title="訂票基本資料作業之完整循序圖"/>

<h3>「處理訂單記錄作業」之系統循序圖</h3>
<img src="http://i.imgur.com/mAzXzBr.png" title="處理訂單記錄作業之系統循序圖"/>
<h3>「電影基本資料作業」之系統循序圖</h3>
<img src="http://i.imgur.com/QeT9Kyv.png" title="電影基本資料作業之系統循序圖"/>
<h3>「憑據處理作業」之系統循序圖</h3>
<img src="http://i.imgur.com/pRSbaH9.png" title="憑據處理作業之系統循序圖"/>
<h3>「銷售分析作業」之系統循序圖</h3>
<img src="http://i.imgur.com/GGtsAfd.png" title="銷售分析作業之系統循序圖"/>

## E-R Model ##
<img src="http://i.imgur.com/KJCAX9u.png" title="E-R Model"/>
