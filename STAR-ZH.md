<br><br />
CV - STAR - 專案經驗 (詳細版)
<br><br />
=====================================


# 大綱 <a name="top"></a>
#### [1.0------- 概述<依公司>](#section-1-0-star)
#### [1.0.1----- SideProject](#section-1-0-1-star)  
#### [1.1.1----- 綠節能智控公司 - 蘇州休息站 - 車輛容量管理](#section-1-1-1-star)
#### [1.1.2----- 綠節能智控公司 - 政府標案 - 影像辨識車輛逆行](#section-1-1-2-star)
#### [1.1.3----- 綠節能智控公司 - 人流偵測管理系統(PFD](#section-1-1-3-star)
#### [1.2.1----- 惠特科技公司 - Probe - Motion 3-Axis system 更換案](#section-1-2-1-star)  
#### [1.2.2----- 惠特科技公司 - Probe - Vision CCD](#section-1-2-2-star)  
#### [1.2.3----- 惠特科技公司 - Probe - Source Meter 主從架構優化案](#section-1-2-3-star)
#### [1.3.1----- 三商電腦公司 - 台北捷運萬大線車站軟韌體](#section-1-3-1-star)  
#### [1.4.1----- 研華科技公司 - 邊緣設備智慧攝影機 - 使用者介面與串流串接 ](#section-1-4-1-star)  

<br><br />

<h1 id="section-1-0-star">概述 <依公司分類> </h1>

美商普維股份有限公司(Latticework)  •  Jul 2023 - Jul 2024

- 產品後端開發優化與測試
- DevOps CI/CD優化
- 內部技術文件撰寫

研華科技公司(ADVANTECH)  •  Aug 2021 - Jul 2023
- [邊緣設備智慧攝影機 - 使用者介面與串流串接 ](#section-1-4-1-star)  

三商電腦公司(MDS)  •  Dec 2020 - Aug 2021

- [台北捷運萬大線車站軟韌體](#section-1-3-1-star) 

惠特科技公司(Fittech)  •  May 2017 - Jun  2019 

- [Probe - Motion 3-Axis system 更換案](#section-1-2-1-star)
- [Probe - Vision CCD](#section-1-2-2-star)
- [Probe - Source Meter 主從架構優化案](#section-1-2-3-star)
- 新人訓練

綠節能智控公司(HIPOWER) Mar 2015 - Mar 2017

- [政府標案 - 影像辨識車輛逆行](#section-1-1-2-star)
  - 刊登頁面:[國道視窗 - 國道5號蘇澳交流道出口增設逆行車輛偵測 ](https://www.freeway.gov.tw/Upload/Html/2017410162/page07.html)
- [蘇州休息站 - 車輛容量管理](#section-1-1-1-star)
- [人流偵測管理系統(PFD)](#section-1-1-3-star)

[Back Top](#top)
<br><br />


<h2 id="section-1-4-1-star">研華科技公司 - 邊緣設備智慧攝影機 - 使用者介面與串流串接 </h2>

研華科技公司 - 邊緣設備智慧攝影機 - 使用者介面與串流串接 

Linux, git, Python, Flask, React, Redux, html, CSS, Javascript,Pytest, selenium, E2ETesting, C#, OOP, SOLID, nginx, docker, docker-compose, jenkins, ffmpeg, rtsp, http-flv, https, openSSL, UML, Workflow, Sequence, WBS, OKR, AON, Milestone, swagger, openapi, postman, mongodb, redis 

團隊人數共4人:1網頁(我),2驅動;1韌體;,  負責範疇如下

- 情況S：  
  - 接手外包開發的相機GUI外，需將即時影像串流由韌體層拉至介面並且完成其他功能
    - 僅熟悉後端，不曾接觸過前端相關技術，或正規SA/SD規劃。
    - 缺乏規劃或文件，對外包無驗收標準，後期也無從追溯設計理念。  
    - 原設計無ErrorHandle與Log機制，頻繁發生改A倒B，使底層錯誤直接暴露User眼前等且無從追查。  

- 任務T：  
  - 需要優化系統架構與設計，解決設計缺陷帶來的挑戰。  
  - 制定工作分解並，與各層成員派工，同時確保各層成員進展穩定，並整合產出。  
  - 需確認影像串流之間的技術可行性與效能


- 行動A：  
  - 由設計維度進行規畫執行：      
    - (WBS / OKR / ANO) : 劃分團隊分工WBS，OKR遠中近目標，執行順序AON，里程碑。  
    - (UML /Workflow/Sequence) : 將模糊需求轉化為具體設計。  
    - (Wireframe/UIFlow) : 用於UI/UX，於跨部門溝通中模擬用戶情境。  
    - (API Doc/Swagger) : 將依照SOLID原則，將功能切細後，制定名稱 功能 引數 回傳撰寫為文件

  - 優化系統基礎架構：  
    - (代碼生成器)       : 當時無生成式AI，在家自行開發，同時產出React Redux 及Flask 的Code並嵌入 OpenAPI3.0於註解中
    - (Microservice)    : Docker取代Systemd，並打包VideoStream的轉碼服務
    - (ErrorHandle/FW Layer) : 根據過往經歷，導入ErrorHandle回報各層錯誤代碼與對應資訊    
    - (VideoStream)     : 自家IPCam拉RTSP 用FFmpeg HttpFlv 建立直播架構，用VLC POC完成後提案。
    - (E2E Framework)   : Pytest & selenium 開發 POM 測試腳本框架

- 結果R：  
  - 各自行動(Action)成效如下:
    - (WBS / OKR / ANO) : 腦內風暴，規劃排程，有利於成員理解當前目標與後續規劃
    - (UML/Wireframe ..etx): 開發前，對焦需求，避免成品與需求脫鉤
    - (代碼生成器)       : 自動化Coding將時間比例降低 提升代碼品質 開發效率相較外包提升90.48%   
    - (VideoStream)     : 憑藉經驗，快速提出解決方案
    - (Microservice)    : 降低各平台交叉測試的時間與難度，提升了系統健強性，以及
    - (ErrorHandle/FW Layer): 壓低了BUG發生頻率，平均降低故障排除時間60%
    - (E2E POM Framework): 降低測試腳本維護難度，迭代中，快速察覺問題與。
      - [git](https://github.com/YiFan0221/E2E-POM) https://github.com/YiFan0221/E2E-POM
  - 無經驗下，如期提早完成外，並於規劃的緩衝時間內處理兩次設計變更，準時交付，期間成員無需加班，甚至期間善用空檔出遊。

<br><br />
[Back Top](#section-1-0-star)
<br><br />

<h2 id="section-1-3-1-star">三商電腦公司 - 台北捷運萬大線車站軟韌體 </h2>

三商電腦公司 - 台北捷運萬大線車站軟韌體

C++, C#, Winform, FP, SOLID, Singleton

團隊人數共7人, 專案人數2人, 管理1人,  負責範疇如下

- S：票口閘門、自動售票機、人員操作軟體與中央電腦傳輸的系統開發
- T：台北捷運規範的通訊電文編解譯函式庫，同時負責GATE、CCBE、UPS整開發串接，因重複性高此處僅說明電文部分
- A：  
   - 受同仁鼓勵接下主導角色，了解成員開發風格習慣後進行架構規劃與派工
   - 考量未來移植，並存在多種轉型需求情境，選用C#做為主體，部分需快速運算則調用C++開發的函式庫
   - 依下列方式進行拆解，分為UI控制相關類別;資料型態相關類別
   - Functional Programming, FP 單一方向資料流
     - 依SOLID:SIP/ISP，將底層功能抽出，該函式專責處理一種任務
     - 依SOLID:OCP，若功能需要變形，採Overloading實現代碼重複使用
     - 依SOLID:LSP，使用enum對傳入回傳型態進行限制，保護函式正確性
     - 依SOLID:DIP，透過高階函式或參數，消除對實現的依賴
   - 因時程緊迫，分派範疇後穩定執行，每天與member進行一次sync
- R：  
   - 起初本為新人考核題目，但由於架構規劃得宜，可靠度與移植性受到認可，轉為重點專案並應用於各項設備中

[Back Top](#section-1-0-star)
<br><br />

<h2 id="section-1-2-1-star">惠特科技公司 - Probe - Motion 3-Axis system 升級案</h2>

惠特科技公司 - Probe - Motion 3-Axis system 升級案

C++, C#, Winform, Multi-Thread, State Pattern

專案人數1人 並為產品負責人

- S：Legacy Code無文件與交接，更換Motion system，並進行效能上提升
- T：Project Owner，獨自進行，整合新舊軟體，提升針痕速度至符合商用標準
- A：
   - 觀察state Pattern Log 製作 State Graph
   - 採非對稱s curve，極速出發輕柔到達
   - 預測演算法，因藍膜上並非平整，能藉當前dut高度，預測下顆高度 ※PS: dut/die/chip
   - 與外籍工程師協作修改客製化SDK
   - 波得圖確保剛性
   - 引出驅動卡input Pin借高解析度CLK紀錄訊號使用
   - 示波器監控pulse與signal是否符合理論
   - 蒐集速度參數與數據分析，確保理論匹配
   - 上機至產線進行試量產
- R：  
   - 使停擺兩年的專案進入試量產
   - 達成 可控精度為0.1微米, dut sizem約30條, motion cycle time為16ms
   - 精準在每個dut上的每個pad精準戳滿6個一抹淺淺不戳破薄膜的針痕

[Back Top](#section-1-0-star)
<br><br />


<h2 id="section-1-2-2-star">惠特科技公司 - Probe - Vision CCD </h2>

惠特科技公司 - Probe - Vision CCD

C++, C#, Winform, Multi-Process, Multi-Thread, State Pattern, Memory-mapped file, Win32 API, IPC, videostream

團隊人數共5人, 專案人數1人, 後期管理人數2人,  負責範疇如下

- S：現行CCD取得成本高，尋找替代方案。  
- T：評測各牌CCD，並進行AOI流程整合，同樣Legacy Code。  
- A：
   - 於SDK Tool進行功能驗證，並整合至現有AOI流程
   - 分別評測:成像;顏色;銳利;溫度;穩定;
   - 召集會議，與原廠應用開發總監，提出客製化需求規格，要求修改SDK後驗證功能
   - 藉預估採購量作為籌碼，並與亞太區域經理，建立台灣區倉庫安全庫存
   - 重構並物件化，並撰寫DemoCode與文件，同被指派規劃教育訓練
- R：  
   - 導入新品牌，降低65%取得成本
   - 使原廠承諾
     - 建立國內倉庫快速供應
     - 少量，從下單至國內出貨到收貨可優先供貨並在一週內完成
     - 大量，從下單至海外出貨、清關、收件時間不超過兩週
   - 規劃教育訓練，兩週內快速上手，期間訓練過2員，留任率2員，成功率100%

<br><br />
[Back Top](#section-1-0-star)
<br><br />


<h2 id="section-1-2-3-star">惠特科技公司 - Probe - source meter 主從架構優化案</h2>

惠特科技公司 - Probe - source meter 主從架構優化案

C++, C#, Winform, memory management, Multi-Process, Multi-Thread, State Pattern, Memory-mapped file, Win32 API, IPC

團隊人數共5人, 專案人數1人, 負責範疇如下

- S：關鍵原料(keithley)斷料，替代料(NI)相容性問題，原廠拒絕支援長達半年，庫存產能僅剩一個月。  
- T：非主管指派，主動提出解決方案並主導專案
- A：
   - 分兩個方向同時進行 
     - 駁論原廠，換取技術支持
     - 當下尋找其他解決方案
   - 與CCD廠商召開技術會議，借重廠商在韌體領域專業，準備理論基礎
   - 使用微軟工具VMMap 證明SDK初始化佔據過多行程可支配記憶體空間，促使原廠派美籍工程師來台勘察
   - 同時將現有架構座椅下重構
     - 多行程，分割出量測功能至另外個行程(主管要求後換成CCD取像功能)，解決單一行程兼記憶體不足問題
     - 主從架構，Memory-mapped file 傳遞量測結果，以及 Win32 Msg 控制附屬程式
- R：
   - 充足理論基礎與資料，一天就讓賴了半年的原廠改變態度
   - 同步完成兩個方向之目標，
   - 從行動到部屬，僅僅花費兩週完成半年的困境

<br><br />
[Back Top](#section-1-0-star)
<br><br />

<h2 id="section-1-1-2-star">綠節能智控公司 - 政府標案 - 影像辨識車輛逆行</h2>

綠節能智控公司 - 政府標案 - 影像辨識車輛逆行

C++, Embedded Windows, Winform, Linux, Multi-Process, Multi-Thread, Producer-Consumer Pattern, Message Queue, Memory-mapped file, Win32 API, IPC, NSIS, Serial port(COM), I2C, UART, SPI, NetIO, FFmpeg, Live555, RTSP, MySQL, Vision, LRC

團隊人數共6人, 專案人數4人, 負責範疇如下

刊登頁面:[國道視窗 - 國道5號蘇澳交流道出口增設逆行車輛偵測 ](https://www.freeway.gov.tw/Upload/Html/2017410162/page07.html)

- S：政府標案，使用搭載Embedded Windows的設備，透過影像及線圈訊號，偵測逆行回報至系統
- T：
  - 獨自負責以下開發內容
  - 設備影像串流導入辨識分析;整合主機板韌體SDK
  - 理解業主規範協定編解譯，功能實現
  - 整合地面線圈(通訊)與NVR SDK(C#)等週邊設備
- A：  
  - 重新設計功能繁多的設定頁面GUI為側邊導航（Sidebar Navigation）
  - Vision
    - 多Channel IPCam，RTSP接收VideoStreaming，採用Memory-mapped file取得畫面
    - RGB-Matrix Downsampling(Uniform Sampling), Grayscale Conversion(Weighted Average Method) and Binarization(Global Thresholding)
  - Task Scheduling
    - Producer-Consumer Pattern
    - Event-Driven Architecture
    - Message Queue, MQ
    - Task Dispatcher
    - Asynchronous Communication
  - 高公局通訊協定編解譯
    - 縱向冗餘校驗(Longitudinal redundancy check, LRC)
    - Bitwise Operations
    - 可相容於UART通訊
  - 開發HW/SW Watchdog，處理主機板間SDK調用，實現GPIO、低電壓警報
  - 主從架構，採Multi-Process緩解函式庫導致記憶體不足問題，搭配Win32 API與Memory-mapped file IPC進行控制
- R：  
   - 新增符合規範之功能
   - 主從架構與IPC，實現出錯快速復歸提升穩定性與容錯度，滿足需置於戶外24小時不間斷運作需求
   - 開發項目皆可沿用至下個專案中

<br><br />
[Back Top](#section-1-0-star)
<br><br />

<h2 id="section-1-1-1-star">綠節能智控公司 - 蘇州休息站 - 車輛容量管理</h2>

綠節能智控公司 - 蘇州休息站 - 車輛容量管理

C++, Embedded Windows, Winform, Linux, Multi-Process, Multi-Thread, Producer-Consumer Pattern, Message Queue, Memory-mapped file, Win32 API, IPC, NSIS, Serial port(COM), I2C, UART, SPI, NetIO, FFmpeg, Live555, RTSP, MySQL, Vision, LRC

團隊人數共6人, 專案人數4人, 負責範疇如下

- S：高速公路休息站停車場的中控中心專案
- T：負責開發操作軟體，接收計數模組回傳資訊並進行統計，依照設定將車位資訊顯示於LED看板上;安控室電視牆CCTV輪播;串流轉發服務器
- A： 
  - 統計程式 
    - GUI in Winform RWD，多國語言
    - 二次開發LED看板
    - 資料統整與查詢功能
  - NSIS一鍵安裝包，與使用手冊，降低現場同仁難易度
  - 完成上述工作後，接手同仁任務，完成基於Live555、FFmpeg 影像串流轉發服務
- R：  
   - SOP降低遠端作業難度，部署於中國二十幾個站點  
   - 軟體工程方式主從架構與IPC，實現出錯快速復歸提升穩定性與容錯度，滿足需置於戶外24小時不間斷運作需求

<br><br />
[Back Top](#section-1-0-star)
<br><br />

<h2 id="section-1-1-3-star">綠節能智控公司 - 人流偵測管理系統(PFD) </h2>

綠節能智控公司 - 人流偵測管理系統(PFD)

工作職掌: SW/FW RD

使用Skill - C++, Winform, FFmpeg, Live555, RTSP, MySQL, RWD

產品頁面: [人流偵測管理系統(PFD) (連結內為今產品, 任職當時未有AI與網頁式)](https://www.hipower-tech.com/Pro_PFD.php)

主要成果:
  - 應用於南港展覽館

特色:
  - 適用多出入口空間環境以及分區管理人員偵測統計分析應用。
  - 若人流累積達到閥值時系統將會提醒管制中心人員以及透過顯示屏幕顯示警示數值和狀態提示管理人員進行人員總量管控機制。
  - 針對偵測事件觸發可以自動整合連動攝影機進行記錄照片或影像／事件名稱／時間／地點，並供調閱查詢事件前後歷史資料與匯出管理功能。


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