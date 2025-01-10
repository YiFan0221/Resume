<br><br />
專案經驗 
<br><br />
=====================================


# 大綱 <a name="top"></a>
#### [1.0------- 概述<依公司>](#section-1-0-star)
#### [1.0.1----- SideProject](#section-1-0-1-star)  
#### [1.1.1----- 綠節能智控公司 - 蘇州休息站 - 車輛容量管理](#section-1-1-1-star)
#### [1.1.2----- 綠節能智控公司 - 政府標案 - 影像辨識車輛逆行](#section-1-1-2-star)
#### [1.2.1----- 惠特科技公司 - Probe - Motion 3-Axis system 更換案](#section-1-2-1-star)  
#### [1.2.2----- 惠特科技公司 - Probe - Vision CCD](#section-1-2-2-star)  
#### [1.2.3----- 惠特科技公司 - Probe - Source Meter 主從架構優化案](#section-1-2-3-star)
#### [1.3.1----- 三商電腦公司 - 台北捷運萬大線車站軟韌體](#section-1-3-1-star)  
#### [1.4.1----- 研華科技公司 - 產品圖形使用者介面](#section-1-4-1-star)  

<br><br />
<br><br />

<h1 id="section-1-0-star">概述 <依公司分類> </h1>

美商普維股份有限公司(Latticework)  •  Jul 2023 - Jul 2024

- 產品後端開發優化與測試
- DevOps CI/CD優化
- 內部技術文件撰寫

研華科技公司(ADVANTECH)  •  Aug 2021 - Jul 2023

- [產品網頁圖形使用者介面的開發與整合](#section-1-4-1-star)  
- [後端程式開發與系統架構的優化](#section-1-4-1-star) 

三商電腦公司(MDS)  •  Dec 2020 - Aug 2021

- [台北捷運萬大線車站軟韌體](#section-1-3-1-star) 

惠特科技公司(Fittech)  •  May 2017 - Jun  2019 

- [Probe - Motion 3-Axis system 更換案](#section-1-2-1-star)
- [Probe - Vision CCD](#section-1-2-2-star)
- [Probe - Source Meter 主從架構優化案](#section-1-2-3-star)
- 新人訓練

綠節能智控公司(HIPOWER) Mar 2015 - Mar 2017

- [政府標案 - 影像辨識車輛逆行](#section-1-1-2-star)
- [蘇州休息站 - 車輛容量管理](#section-1-1-1-star)
- 多項硬體與軟體結合系統開發

<br><br />
[Back Top](#top)
<br><br />


<h2 id="section-1-4-1-star">研華科技公司 - 產品圖形使用者介面</h2>

研華科技公司 - 攝影機影像串流以及使用者介面

Linux, git, Python, Flask, React, Redux, html, CSS, Javascript,Pytest, selenium, E2ETesting, C#, OOP, SOLID, nginx, docker, docker-compose, jenkins, ffmpeg, rtsp, http-flv, https, openSSL, UML, Workflow, Sequence, WBS, OKR, AON, Milestone, swagger, openapi, postman, mongodb, redis 

團隊人數共4人:2驅動;1韌體;1網頁,  負責範疇如下

- 情況S：  
  - 接手外包開發的相機GUI外，需將即時影像串流由韌體層拉至介面並且完成其他功能
    - 僅熟悉後端，不曾接觸過前端相關技術，或正規SA/SD規劃。
    - 缺乏清晰規劃或文件，對外包無驗收標準，後期也無從追溯設計理念。  
    - 原設計無ErrorHandle與Log機制，改A導B、使底層錯誤直接暴露User眼前等頻繁發生且無從追查。  

- 任務T：  
  - 需要優化系統架構與設計，解決設計缺陷帶來的挑戰。  
  - 制定工作分解並，與各層成員派工，同時確保各層成員進展穩定，並整合產出。  
  - 需確認影像串流之間的技術可行性與效能


- 行動A：  
  - 多元管道學習解決方案，由設計維度進行規畫執行：      
    - (Coffee Chat)     : 平時透過與業界友人約吃飯，請教技術與解決方案，得知相關技術後自學。  
    - (WBS / OKR / ANO) : 劃分團隊分工WBS，OKR遠中近目標，執行順序AON，里程碑。  
    - (UML /Workflow/Sequence) : 將模糊需求轉化為具體設計。  
    - (Wireframe/UIFlow) : 用於UI/UX，於跨部門溝通中模擬用戶情境。  
    - (API Doc/Swagger) : 將依照SOLID原則，將功能切細後，制定名稱 功能 引數 回傳撰寫為文件

  - 優化系統基礎架構：  
    - (代碼生成器)       : 當時無生成式AI，在家自行開發，同時產出React Redux 串接API 以及Flask API接口Code與對應的OpenAPI3.0/Swagger
    - (Docker)          : 使用Docker取代原本的Systemd，並打包VideoStream的轉碼服務
    - (ErrorHandle/FW Layer) : 根據過往經歷，導入ErrorHandle回報各層錯誤代碼與對應資訊    
    - (VideoStream)     : 自家IPCam拉RTSP 用FFmpeg HttpFlv 建立直播架構，用VLC POC完成後提案。
    - (E2E)             : 使用Pytest & selenium 製作能以網頁為物件的自動化測試腳本框架

- 結果R：  
  - 各自行動(Action)成效如下:
    - (Coffee Chat)     : 避免使用過時不敷使用的技術，且大幅取得須掌握標的。
    - (WBS / OKR / ANO) : 腦內風暴，規劃，排程，也有利於成員理解當前目標與後續規劃，能自主對當前工作進行調整與建議。
    - (UML/Wireframe .. etx): 於正式進入開發前，由設計維度對焦需求並達成共識，直接避免成品與需求脫鉤的風險。
    - (代碼生成器)       : 自動化Coding將開發時間比例降為 規劃7:驗證2:撰寫1 避免手動撰寫造成的錯誤 開發效率相較外包提升至少750%     
    - (VideoStream)     : 憑藉過去對影像串流的經驗，快速隊需求提出(RTSP/RTP/HttpFLV)解決方案，團隊最後選擇使用HttpFlV 
    - (Docker/compose)  : 容器化的環境一致性，壓低了BUG發生頻率，同時降低直播架構於各平台交叉測試的時間與難度，提升了微服務間的健強性
    - (ErrorHandle/FW Layer): 錯誤碼成功降低過往100%猜測錯誤來源的時間，搭配Docker使用後從發現問題到重現，與過往節省至少60%時間
    - (E2E)             : 幫助內部SQA人員，版本更迭中快速發現功能遺失並快速反應。 
  - 無經驗下，期間善用空檔出遊，如期提早完成外，並於規劃的緩衝時間內處理兩次設計變更，準時交付，期間成員無需加班。

<br><br />
[Back Top](#section-1-0-star)
<br><br />

<h2 id="section-1-3-1-star">三商電腦公司 - 台北捷運萬大線車站軟韌體 </h2>

三商電腦公司 - 台北捷運萬大線車站軟韌體

C++, C#, Winform, FP, SOLID, Singleton

團隊人數共7人, 專案人數2人, 管理1人,  負責範疇如下

- S：站內閘門、自動售票機、人員操作軟體與中央電腦傳輸的系統開發
- T：開發台北捷運規範的通訊電文編解譯函式庫，同時負責GATE、CCBE、UPS整開發串接，因重複性高此處僅說明電文部分
- A：  
   - 受同為新進同仁鼓勵接下主導角色，了解開發風格習慣後進行架構規劃
   - 考輛未來開發環境為，並存在多種轉型需求情境，選用C#做為主體，部分需快速運算則調用C++開發的函式庫
   - 依下列方式進行拆解，分為UI控制相關類別;資料型態相關類別
   - Functional Programming, FP 單一方向資料流
     - 依SOLID:SIP/ISP，將底層功能抽出，該函式專責處理一種任務
     - 依SOLID:OCP，若功能需要變形，採Overloading實現代碼重複使用
     - 依SOLID:LSP，使用enum對傳入回傳型態進行限制，保護函式正確性
     - 依SOLID:DIP，透過高階函式或參數，消除對實現的依賴
   - 因時程緊迫，分派範疇後穩定執行，每天與member進行一次sync
- R：  
   - 起初本為新人考核題目，但由於架構規劃得宜，可靠度與移植性受到認可，轉為重點專案並應用於各項設備中

<br><br />
[Back Top](#section-1-0-star)
<br><br />

<h2 id="section-1-2-1-star">惠特科技公司 - Probe - Motion 3-Axis system 升級案</h2>

惠特科技公司 - Probe - Motion 3-Axis system 升級案

C++, C#, Winform, Multi-Thread, State Pattern

團隊人數共5人, 專案人數1人,  負責範疇如下

- S：Legacy Code無文件與交接，更換old Motion system，並進行效能上提升
- T：Project Owner，獨自進行，新舊軟體整合，針痕速度提升至符合商用
- A：
   - 觀察state Pattern Log 製作 State Graph
   - 採用非對稱加速，極速出發輕柔到達
   - 因藍膜上的每個dut並非平整，能藉當前dut高度，預測下顆高度 
   PS: dut/die/chip
   - 對廠商提出客製化需求與外籍工程師協作修改SDK
   - 使用博得圖與確保設備剛性足夠且不會引發自然共振並請機構修正
   - 跨部請EE協助引出驅動卡input Pin借高解析度CLK紀錄訊號使用
   - 使用示波器監控pulse與signal是否符合理論
   - 蒐集速度參數與測試數據進行分析調整，確保物理特性與運作匹配
   - 上機至產線進行試量產
- R：  
   - 重啟前人停擺兩年的專案進入試量產
   - 達成 可控精度為0.1微米, dut sizem約30條, motion cycle time為16ms
   - 每片藍膜可上下料後調整針位數次，在每個dut上的每個pad精準戳滿6個一抹淺淺不戳破薄膜的針痕


<br><br />
[Back Top](#section-1-0-star)
<br><br />


<h2 id="section-1-2-2-star">惠特科技公司 - Probe - Vision CCD </h2>

惠特科技公司 - Probe - Vision CCD

C++, C#, Winform, Multi-Process, Multi-Thread, State Pattern, Memory-mapped file, Win32 API, IPC, videostream

團隊人數共5人, 專案人數1人, 後期管理人數2人,  負責範疇如下

- S：現行CCD取得成本高，尋找替代方案。  
- T：評測各牌CCD，並進行AOI流程整合，同樣Legacy Code。  
- A：
   - 將新廠牌於SDK Tool進行功能驗證，並整合至現有AOI流程進行POC
   - 使用各家SDK Tool與上機環境長時間運作，分別評測:成像;顏色;銳利;溫度;穩定
   - 對代理商召集會議，提出客製化需求規格，要求修改SDK後驗證功能
   - 暗示採購量提升代理商配合效率
   - 與Hikon台灣區總監見面，協商建立台灣區倉庫安全庫存
   - 類別物件化Vision程式碼，並撰寫與主架構雷同的DemoCode與文件
   - 同時間安排教育訓練，使新人Handle CCD代碼
- R：  
   - 導入新品牌，降低65%取得成本
   - 使原廠承諾
     - 國內建立倉庫準備快速供應至少一產線單生產週期使用的量
     - 少量下單從下單，國內出貨到收貨可優先供貨並在一週內完成
     - 大量下單從下單，海外出貨、清關、收件時間不超過兩週
   - 兩個新人皆於兩週內快速上手新代碼，且一個還帶一個，訓練成功率100%

<br><br />
[Back Top](#section-1-0-star)
<br><br />


<h2 id="section-1-2-3-star">惠特科技公司 - Probe - source meter 主從架構優化案</h2>

惠特科技公司 - Probe - source meter 主從架構優化案

C++, C#, Winform, Multi-Process, Multi-Thread, State Pattern, Memory-mapped file, Win32 API, IPC

團隊人數共5人, 專案人數1人, 負責範疇如下

- S：keithley關鍵原料斷料，替代料NI相容性問題，原廠拒絕支援長達半年，庫存產能僅剩一個月。  
- T：非主管指派，主動提出解決方案並主導專案
- A：
   - 分兩個方向同時進行 
     - 證實原廠BUG換取技術支持
     - 考量等待原廠改版將勢必影響生產，需立即尋找其他方案
   - 與CCD廠商召開技術會議，借重廠商在韌體領域專業，準備理論基礎
   - 使用微軟工具VMMap 證明SDK初始化佔據過多行程可支配記憶體空間，促使原廠派美籍工程師來台勘察
   - 同時參考過去經驗與技術提案
     - 多行程，分割出量測功能至另外個行程(主管要求後換成CCD取像功能)，舒緩當前版本SDK造成記憶體不足問題
     - 主從架構，Memory-mapped file 傳遞量測結果，以及 Win32 Msg 控制附屬程式
- R：
   - 充足理論基礎與資料，一天就讓原廠改變態度
   - 現場與美籍工程師證實理論正確，並同步完成解決方案舒緩產線壓力
   - 從採取行動到安裝程式至產線，前後僅僅花費兩週完成
   - 讓過去經驗發揮作用，主從架構使Legacy Code編譯時間降低，健強度提升

<br><br />
[Back Top](#section-1-0-star)
<br><br />

<h2 id="section-1-1-2-star">綠節能智控公司 - 政府標案 - 影像辨識車輛逆行</h2>

綠節能智控公司 - 政府標案 - 影像辨識車輛逆行

C++, Embedded Windows, Winform, Linux, Multi-Process, Multi-Thread, Producer-Consumer Pattern, Message Queue, Memory-mapped file, Win32 API, IPC, NSIS, Serial port(COM), I2C, UART, SPI, NetIO, FFmpeg, Live555, RTSP, MySQL, Vision, LRC

團隊人數共6人, 專案人數4人, 負責範疇如下

- S：政府標案，使用搭載Embedded Windows的設備，透過影片辨識及地面線圈訊號，偵測車輛逆行事件，並回報至高公局系統
- T：
  - 獨自負責以下開發內容
  - 設備影像串流導入辨識分析;整合主機板韌體SDK
  - 理解並開發高公局溝通協定編解譯，規範功能
  - 整合地面線圈(通訊)與NVR SDK(C#)等設備
- A：  
  - 重新設計功能繁多的設定頁面GUI為側邊導航（Sidebar Navigation）
  - Vision
    - 多Channel IPCam，RTSP接收VideoStreaming，採用Memory-mapped file取得畫面
    - RGB-Matrix Downsampling(Uniform Sampling), Grayscale Conversion(Weighted Average Method) and Binarization(Global Thresholding)
  - Task 收發(從無到有重頭構思，當時不知道有這些技術..)
    - Producer-Consumer Pattern
    - Event-Driven Architecture
    - Message Queue, MQ
    - Task Dispatcher/Scheduling
    - Asynchronous Communication
  - 高公局通訊協定編解譯
    - 縱向冗餘校驗(Longitudinal redundancy check, LRC)
    - Bitwise Operations
    - 可相容於UART通訊
  - 開發軟硬體Watchdog，處理主機板間SDK調用，實現GPIO、低電壓警報、HW Watchdog
  - 提出主從架構，採Multi-Process緩解函式庫導致記憶體不足問題，搭配Win32 API與Memory-mapped file，IPC進行控制，負責Vision與主板兼任體功能調用
  - 與上包取得開發規範並每週匯報進度並至現場驗收對測
- R：  
   - 新增符合規範之功能
   - 主從架構與IPC，實現出錯快速復歸提升穩定性與容錯度，滿足需置於戶外24小時不間斷運作需求
   - 開發項目皆可沿用至下個專案中

<br><br />
[Back Top](#section-1-0-star)
<br><br />

<h2 id="section-1-1-1-star">綠節能智控公司 - 蘇州休息站</h2>

綠節能智控公司 - 蘇州休息站

C++, Embedded Windows, Winform, Linux, Multi-Process, Multi-Thread, Producer-Consumer Pattern, Message Queue, Memory-mapped file, Win32 API, IPC, NSIS, Serial port(COM), I2C, UART, SPI, NetIO, FFmpeg, Live555, RTSP, MySQL, Vision, LRC

團隊人數共6人, 專案人數4人, 負責範疇如下

- S：高速公路休息站停車場的中控中心專案
- T：我負責開發供人員操作軟體，接收計數模組回傳資訊並進行統計，依照設定將當前/剩餘車位顯示於LED看板上;以及負責安控室的CCTV輪播電視牆;以及開發串流轉發服務
- A： 
  - 統計程式 
    - GUI in Winform RWD，多國語言
    - 二次開發LED看板，並測通
    - 將統計資料統整並存入MySQL與查詢功能，並依照前案我所開發協定與主系統回報
  - CCTV電視牆
    - 將前案Multi-Process開發影像串流程式，Memory-mapped file，Win32 API IPC，應用於此案
    - 開發MOXA品牌PTZ軸控攝影機
  - NSIS一鍵安裝包，與使用手冊，降低現場同仁難易度
  - 完成上述工作後，接手同仁任務，完成基於Live555、FFmpeg 影像串流轉發服務
- R：  
   - SOP降低遠端部署難度，成功部署於中國二十幾個站點  
   - 軟體工程方式主從架構與IPC，實現出錯快速復歸提升穩定性與容錯度，滿足需置於戶外24小時不間斷運作需求

<br><br />
[Back Top](#section-1-0-star)
<br><br />


<h2 id="section-1-0-1-star">SideProject</h2>

```
---

SideProject

疫情期間使用linebot串接後端爬蟲公同事查詢股價使用

後續加入容器化、CICD、ChatGPT等功能

應用技術:python / linebot / OpenAI / docker / Nginx / Jenkins / (AWS目前關閉中)/爬蟲/devops建置/分散式設計

實現:最新PTT連結 / linebot / 當前股價查詢功能 / ChatGPT(不定時開放功能)



**TeaOrFish**:

Linebot ID : @320swnwx

[Main Service]

git: https://github.com/YiFan0221/TeaOrFish

[Sub Service]

git: https://github.com/YiFan0221/YiFanServer

swagger: http://yfnoip.ddns.net:5500/apidocs/

[Jenkins]

URL: http://yfnoip.ddns.net:8080/

access : guest / guest


**Web UI testing**:

使用selenium並結合pytest可對於網頁進行自動化測試

[git](https://github.com/YiFan0221/E2E-POM)
```

<br><br />
[Back Top](#section-1-0-star)
<br><br />