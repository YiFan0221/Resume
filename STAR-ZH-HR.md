<br><br />
CV - STAR - 專案經驗 (人資版)
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

<h3 id="section-1-4-1-star">研華科技公司 - 產品圖形使用者介面</h3>

研華科技公司 - 產品圖形使用者介面
- S：  
   - 接手外包開發的相機網頁GUI專案，需整合韌體與DeepStream進行即時影像辨識與預覽。  
        - 團隊缺乏清晰的規劃與規格文件，導致初期無法制定驗收標準，後期也無從追溯原設計意圖。  
        - 原設計拒絕設置ErrorHandle與Log機制，韌體或底層錯誤直接暴露於使用者界面，追查與修復困難。  

- T：  
   - 作為專案接手者，分析問題根源並提出解決方案。  
        - 需要優化系統架構與設計，解決初期設計缺陷帶來的挑戰。  
        - 推動專案分工協作，確保穩定進展並按時完成。  

- A：  
   - 主動學習並應用解決方案：  
        - 下班後透過與朋友的Coffee Chat聚會，討論技術挑戰與解決方案，學習相關技術並應用於專案中。  
        - 使用UML、Workflow與Sequence圖表，將模糊需求轉化為具體設計，快速建立團隊共識。  
        - 採用Swagger生成動態API文件與使用WIreFlow制定UI/UX，推動專案文件化並提升跨部門協作效率。  
   - 優化系統基礎架構：  
        - 設計並導入ErrorHandle機制，與韌體層分離，縮短問題追查時間。  
        - 使用Docker與微服務，統一部署環境，減少部署時間並提升穩定性。  
        - 開發代碼生成器產出前後端代碼與文件，減少手動錯誤並提升代碼一致性。  
   - 確保專案穩定進展：  
        - 建立End-to-End (E2E) 自動化測試框架，確保功能穩定性並快速驗證功能變更。  
        - 調整團隊分工策略，明確責任劃分(WBS)，促進專案高效運作。  
- R：
   - 在實施了 ErrorHandle、E2E 測試、動態文件生成等措施後：
        - Bug 追蹤效率顯著提升，平均排查時間縮短 60%。
        - 測試框架確保功能穩定性，迭代過程中無功能遺失。
        - 使用 Docker 和 Swagger，縮短部署與協作時間，API 開發效率提升 300%。
        - 代碼生成器減少手動工作量，整體開發效率提升 750%。
        - 最終在一個月內順利完成專案交付，超過預期目標。

<br><br />
[Back Top](#section-1-0-star)
<br><br />

<h3 id="section-1-3-1-star">三商電腦公司 - 台北捷運萬大線車站協議函式庫  </h3>

三商電腦公司 - 台北捷運萬大線車站協議函式庫
- S：台北捷運電文協定的編解譯演算法。 
- T：開發與台北捷運主系統溝通使用的通訊協定。  
- A：  
   - 與夥伴討論，了解夥伴專長後接下主導位置
   - 分割執行範疇並制定時程，依時程檢驗結果。
   - 制定編碼風格並採用SOLID原則，提升維護容易度  
- R：  
   - 成果優於預期，高可靠度與可移植性使的廣泛應用於各設備中

<br><br />
[Back Top](#section-1-0-star)
<br><br />

<h3 id="section-1-2-1-star">惠特科技公司 - Probe - Motion 3-Axis system 更換案</h3>

惠特科技公司 - Probe - Motion 3-Axis system 更換案
- S：更換舊有架構軸控系統，確保微米等級針痕品質不受影響，需重新啟動。  
- T：獨立執行專案，控制並調校硬體設備，確保針痕品質，並提升速度與控制精度。  
- A：  
   - 除了軟體開發以及實驗外，學習並跨部門協調尋求資源解決問題(如學習博得圖證明剛性不足要求機構修改)  
   - 與荷蘭籍原廠工程師協作客製SDK
- R：  
   - 成功驅動停擺兩年的專案進入試量產，顯著提升設備精度與速度，縮短30%的作業時間，控制精度達0.1微米。

<br><br />
[Back Top](#section-1-0-star)
<br><br />


<h3 id="section-1-2-2-star">惠特科技公司 - Probe - Vision CCD</h3>

惠特科技公司 - Probe - Vision CCD
- S：現行CCD成本過高，須尋找便宜替代方案。  
- T：審視各家CCD成像品質、穩定性及開發難易度。  
- A：  
   - 將CCD與圖像buffer代碼統一規格化，降低整合難度，規劃新人訓練  
   - 與代理經銷商預估採購數量藉此提升配合度  
   - 藉與原廠制定經銷端安全庫存與出貨時長，降低公司庫存成本壓力   
- R：  
   - 導入新品牌，降低成本至少65%，並將下訂到收貨時間縮短至2週  
   - 新人於兩週內快速上手新代碼

<br><br />
[Back Top](#section-1-0-star)
<br><br />


<h3 id="section-1-2-3-star">惠特科技公司 - Probe - Source Meter 主從架構優化案</h3>

惠特科技公司 - Probe - Source Meter 主從架構優化案
- S：原料斷料替代料整合困難，無原廠支援，產線將中斷。  
- T：主動提案證明原廠BUG與提出解決方案。 
- A：  
   - 提議開案架構優化，將子功能切出並透過多行程架構降低主行程資源負荷
   - 借重其他廠商資源，取得相關技術知識，並舉證要求原廠處理  
- R：  
   - 證明原廠問題成功獲取原廠派遣工程師支援
   - 同步完成解決方案POC，提前解決生產危機

<br><br />
[Back Top](#section-1-0-star)
<br><br />

<h3 id="section-1-1-2-star">綠節能智控公司 - 車輛影像辨識逆行偵測專案</h3>

綠節能智控公司 - 車輛影像辨識逆行偵測專案
- S：需要整合影像辨識技術與地面線圈來檢測高速公路交流道的車輛逆行行為，並存在舊廠商配合度的磨合問題。  
- T：開發影像偵測設備，實現軟硬體功能(手提測試機、watchdog、GPIO、電壓與網路狀態偵測等功能)，結合線圈機交叉比對後的資訊，遵循甲方協定回傳高公局。  
- A：  
   - 開發影像辨識軟體、通訊協定、socket、主從架構規劃、硬體SDK整合
   - 多次前往協作廠，透過親切謙虛態度解決技術問題  
- R：  
   - 化解政治帶來的影響，由消極轉變為信任與支持，完成專案。  
   - 提升系統健強度及相容性，致使所有開發項目皆能疊代至下個專案使用  

<br><br />
[Back Top](#section-1-0-star)
<br><br />

<h3 id="section-1-1-1-star">綠節能智控公司 - 蘇州高速公路 - 休息站停車場車輛計數</h3>

綠節能智控公司 - 蘇州高速公路 - 休息站停車場車輛計數
- S：蘇州高速公路休息站停車場，由於高交通流量，導致車輛進入休息站後才得知有無空位。  
- T：與團隊共同制定解決方案，開發車輛計數程式，二次開發LED看板，整合PTZ Cam，以及安控室的CCTV電視牆。  
- A：  
  - 使用多行程主從架構，制定系統間協定，提升系統間穩定性(類今MicroServices)  
  - 使用自適應式介面，提升相容性(類今RWD)  
  - 撰寫使用手冊並開發一鍵安裝包，提升現場人員容易度
  - 完成份內工作支援同仁開發影像串流轉發服務(基於Live555)   
- R：  
   - 提升系統健強度及相容性，致使所有開發項目皆能疊代至下個專案使用  
   - SOP降低遠端部署難度，成功部署於二十幾個站點  

<br><br />
[Back Top](#section-1-0-star)
<br><br />


<h3 id="section-1-0-1-star">SideProject</h3>

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