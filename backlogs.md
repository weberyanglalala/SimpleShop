# 電商專題完整 Backlog

## Epic 1: 首頁開發

### US-001: 首頁 Banner 顯示＋導購按鈕

**Description:**  
作為一個訪客，當我進入首頁時，能看到具有品牌形象的醒目 Banner 區塊，且可以點擊「Shop Now」快速進入商品頁。

**Acceptance Criteria:**

- Banner 須顯示一張高品質圖片，一段主標題與副標題，並有「Shop Now」按鈕
- 點擊「Shop Now」後，使用者將被導向商品列表頁
- Banner 內容可由後台上架與編輯
- Banner 需支援 RWD（響應式設計）

**Estimation:** 5 points

---

### US-002: 類別瀏覽/導覽區

**Description:**  
作為使用者，我能清楚看到居家分類（客廳、臥室、廚房、餐廳、浴室、家庭辦公室），並能點擊各分類快速進入該分類商品頁。

**Acceptance Criteria:**

- 展示 6 個主要空間分類，每個分類有圖片、名稱
- 點擊分類卡片後能切換到對應的分類頁
- 類別內容管理來自後台
- 使用 Flexbox 實現 RWD 排版

**Estimation:** 5 points

---

### US-003: 新品推薦區

**Description:**  
首頁需展示最新上架商品與簡短描述，提升新品曝光與轉換。

**Acceptance Criteria:**

- 最少展示 4 項新到商品，包括圖片、名稱、簡述
- 點擊新品卡片可進入商品詳情頁
- 新品清單來源為後台商品資料，並依照上架時間排序
- 支援 RWD 顯示

**Estimation:** 5 points

---

### US-004: 熱銷推薦區

**Description:**  
首頁展示人氣熱銷商品與簡短描述，吸引用戶點擊與購買。

**Acceptance Criteria:**

- 最少展示 4 項熱銷商品，包括圖片、名稱、簡述
- 點擊熱銷卡片可進入商品詳情頁
- 熱銷清單依據銷售數據由後台計算（例如月銷量 Top 4）
- 支援 RWD 顯示

**Estimation:** 8 points

---

## Epic 2: 共用元件開發

### US-005: Header 導覽列

**Description:**  
提供快速切換各主要區域，包括 Products、Rooms、Inspiration、Offers，右側包含購物車、收藏、會員入口。

**Acceptance Criteria:**

- 導覽列必須於所有頁面可見且點擊後切換相對應頁面
- Cart、Favorite、User Icon 要能正確連結購物車、收藏清單、會員頁
- 購物車圖示顯示當前購物車商品數量
- 支援 Mobile Hamburger Menu

**Estimation:** 8 points

---

### US-006: 搜尋功能

**Description:**  
使用者能夠在頁面右上方搜尋框快速搜尋產品。

**Acceptance Criteria:**

- 搜尋框位於頁面頂部，使用者可輸入關鍵字
- 按 Enter 或點擊搜尋圖示後顯示搜尋結果頁
- 搜尋結果根據關鍵字呈現相關商品

**Estimation:** 8 points

---

### US-007: Footer 區塊

**Description:**  
在頁面底部顯示常用連結與品牌資訊。

**Acceptance Criteria:**

- Footer 包含 About Us、Contact、FAQ、Terms of Service、Privacy Policy 等連結
- 清楚標示網站版權聲明
- 支援 RWD 排版

**Estimation:** 3 points

---

### US-008: 響應式設計（RWD）

**Description:**  
此頁面須在桌機、平板、行動裝置上具有良好視覺與使用體驗。

**Acceptance Criteria:**

- 在不同裝置、解析度下排版不跑版
- 主要操作按鈕、連結皆可於行動裝置點擊
- 使用 Tailwind CSS Flexbox 實現 RWD

**Estimation:** 13 points（橫跨所有頁面）

---

## Epic 3: 商品列表與篩選

### US-009: 商品列表頁顯示

**Description:**  
作為使用者，我能看到商品列表並瀏覽所有可購買的商品。

**Acceptance Criteria:**

- 商品以網格方式排列（桌面版每行 5 個，手機版 2 個）
- 每個商品顯示：圖片、名稱、價格
- 點擊商品進入單一商品頁
- 顯示搜尋結果標題（如 "Results for 'Living Room Furniture'"）

**Estimation:** 5 points

---

### US-010: 商品篩選功能

**Description:**  
使用者能透過多種條件篩選商品，快速找到符合需求的產品。

**Acceptance Criteria:**

- 提供分類篩選 (Category)
- 提供價格範圍篩選 (Price)
- 提供顏色篩選 (Color)
- 提供材質篩選 (Material)
- 每個篩選器為下拉選單
- 篩選條件可複選
- 篩選後即時更新商品列表

**Estimation:** 13 points

---

### US-011: 商品分頁功能

**Description:**  
當商品數量過多時，使用分頁方式呈現，提升載入速度與使用體驗。

**Acceptance Criteria:**

- 頁碼導航（1, 2, 3, 4, 5）
- 上一頁/下一頁按鈕
- 顯示當前頁碼
- 每頁顯示固定數量商品（如 20 筆）
- 支援跳轉至特定頁碼

**Estimation:** 5 points

---

### US-012: 搜尋結果頁

**Description:**  
使用者輸入關鍵字後，能看到相關的搜尋結果商品列表。

**Acceptance Criteria:**

- 顯示搜尋關鍵字
- 顯示搜尋結果數量
- 提供清除搜尋按鈕
- 若無結果顯示友善提示訊息
- 支援搜尋結果排序（價格、熱門度等）

**Estimation:** 8 points

---

## Epic 4: 單一商品頁

### US-013: 商品詳細資訊展示

**Description:**  
作為使用者，我能查看商品的完整資訊，包含圖片、規格、價格等。

**Acceptance Criteria:**

- 顯示商品主圖（大尺寸）
- 顯示 3-4 張商品縮圖
- 點擊縮圖可切換主圖
- 顯示商品名稱、完整描述
- 顯示商品價格
- 顯示商品規格（顏色、材質、尺寸）

**Estimation:** 8 points

---

### US-014: 麵包屑導航

**Description:**  
使用者能清楚知道當前所在位置，並快速返回上層頁面。

**Acceptance Criteria:**

- 顯示完整導航路徑（如：Home / Living Room / Sofas）
- 每個層級可點擊返回
- 當前頁面不可點擊

**Estimation:** 3 points

---

### US-015: 加入購物車功能

**Description:**  
使用者能選擇商品數量並加入購物車。

**Acceptance Criteria:**

- 提供數量選擇器（增加/減少按鈕）
- 顯示「Add to Cart」按鈕
- 點擊後商品加入購物車
- 顯示加入成功提示訊息
- 更新 Header 購物車數量顯示
- 檢查庫存數量，不可超過庫存

**Estimation:** 8 points

---

### US-016: 庫存狀態顯示

**Description:**  
使用者能清楚看到商品的庫存狀態。

**Acceptance Criteria:**

- 顯示庫存狀態（有貨/缺貨/少量庫存）
- 當庫存不足時，顯示剩餘數量
- 缺貨時禁用「Add to Cart」按鈕

**Estimation:** 5 points

---

### US-017: 顧客評價區

**Description:**  
使用者能查看其他顧客對此商品的評價，協助購買決策。

**Acceptance Criteria:**

- 顯示平均評分（星級 + 數字，如 4.5）
- 顯示總評價數量（如 120 reviews）
- 顯示評分分布圖表（5 星到 1 星的百分比）
- 列出個別評價，包含：評價者姓名、日期、星級、評價內容
- 支援評價分頁或「載入更多」

**Estimation:** 13 points

---

### US-018: 相關商品推薦

**Description:**  
在商品詳情頁底部顯示相關商品，增加交叉銷售機會。

**Acceptance Criteria:**

- 顯示至少 3 個相關商品
- 每個商品顯示圖片、名稱、價格
- 點擊可進入該商品詳情頁
- 相關商品基於分類或標籤推薦

**Estimation:** 5 points

---

## Epic 5: 購物車與結帳

### US-019: 購物車商品列表

**Description:**  
使用者能查看已加入購物車的所有商品。

**Acceptance Criteria:**

- 以表格形式顯示商品
- 欄位包含：商品縮圖、名稱、數量、單價、小計
- 每個商品可調整數量
- 提供刪除商品按鈕
- 即時計算並更新小計

**Estimation:** 8 points

---

### US-020: 購物車數量調整

**Description:**  
使用者能在購物車中調整商品數量。

**Acceptance Criteria:**

- 提供數量增加/減少按鈕
- 即時更新商品小計
- 即時更新訂單總額
- 檢查庫存限制
- 數量不可小於 1

**Estimation:** 5 points

---

### US-021: 訂單摘要計算

**Description:**  
購物車頁面顯示完整的訂單摘要，包含小計、運費、稅金、總計。

**Acceptance Criteria:**

- 顯示 Subtotal（小計）
- 顯示 Shipping（運費，標註「下一步計算」）
- 顯示 Total（總計）
- 金額即時更新

**Estimation:** 5 points

---

### US-022: 繼續購物與結帳按鈕

**Description:**  
使用者能選擇繼續購物或前往結帳。

**Acceptance Criteria:**

- 提供「Continue Shopping」按鈕，點擊返回商品列表
- 提供「Proceed to Checkout」按鈕，點擊進入結帳流程
- 購物車為空時，禁用結帳按鈕並顯示提示

**Estimation:** 3 points

---

### US-023: 結帳流程（訂單建立）

**Description:**  
使用者能完成結帳並建立訂單。

**Acceptance Criteria:**

- 驗證使用者登入狀態（未登入則導向登入頁）
- 收集收貨地址資訊
- 選擇運送方式
- 選擇付款方式
- 確認訂單資訊
- 建立訂單記錄
- 顯示訂單確認頁

**Estimation:** 13 points

---

### US-024: 金流整合 - ECPay

**Description:**  
整合 ECPay 金流服務，使用者能使用多種付款方式完成交易。

**Acceptance Criteria:**

- 整合 ECPay API
- 支援信用卡付款
- 處理付款成功/失敗回傳
- 更新訂單付款狀態

**Estimation:** 13 points

---

## Epic 6: 會員系統

### US-025: 會員登入頁

**Description:**  
使用者能透過帳號密碼登入系統。

**Acceptance Criteria:**

- 提供 Email/帳號輸入框
- 提供密碼輸入框
- 提供「Remember me」勾選框
- 提供「Login」按鈕
- 提供「Forgot password?」連結
- 提供「Create an account」註冊連結
- 驗證登入資訊
- 登入成功後導向原頁面或首頁

**Estimation:** 8 points

---

### US-026: 會員註冊功能

**Description:**  
新使用者能建立帳號成為會員。

**Acceptance Criteria:**

- 提供註冊表單（姓名、Email、密碼、確認密碼、電話）
- 驗證 Email 格式
- 驗證密碼強度
- 檢查 Email 是否已被註冊
- 註冊成功後自動登入
- 發送歡迎信件

**Estimation:** 8 points

---

### US-027: 忘記密碼功能

**Description:**  
使用者能透過 Email 重設密碼。

**Acceptance Criteria:**

- 提供 Email 輸入框
- 驗證 Email 是否存在
- 發送重設密碼連結至信箱
- 提供重設密碼頁面
- 驗證重設連結有效性與時效
- 更新新密碼

**Estimation:** 8 points

---

### US-028: 第三方登入 - Google

**Description:**  
使用者能使用 Google 帳號快速登入。

**Acceptance Criteria:**

- 整合 Google OAuth 2.0
- 顯示「Sign in with Google」按鈕
- 處理 Google 登入回傳資訊
- 建立或關聯會員帳號
- 登入成功後導向原頁面或首頁

**Estimation:** 13 points

---

### US-029: 第三方登入 - LINE

**Description:**  
使用者能使用 LINE 帳號快速登入。

**Acceptance Criteria:**

- 整合 LINE Login API
- 顯示「Sign in with LINE」按鈕
- 處理 LINE 登入回傳資訊
- 建立或關聯會員帳號
- 登入成功後導向原頁面或首頁

**Estimation:** 13 points

---

### US-030: 會員個人資訊管理

**Description:**  
會員能查看與編輯個人基本資料。

**Acceptance Criteria:**

- 顯示當前個人資訊（First name, Last name, Email, Phone number）
- 提供編輯表單
- 提供「Update」按鈕
- 驗證輸入資料格式
- 更新成功顯示提示訊息

**Estimation:** 5 points

---

### US-031: 會員密碼變更

**Description:**  
會員能變更登入密碼。

**Acceptance Criteria:**

- 提供「Change password」按鈕
- 點擊後展開密碼變更表單
- 輸入當前密碼
- 輸入新密碼
- 確認新密碼
- 驗證當前密碼正確性
- 驗證新密碼強度
- 更新密碼並顯示成功訊息

**Estimation:** 5 points

---

### US-032: 會員側邊欄導航

**Description:**  
提供會員功能的快速導航選單。

**Acceptance Criteria:**

- 顯示側邊欄選單，包含：
  - Account details（帳戶詳情）
  - Addresses（地址管理）
  - Saved items（收藏商品）
  - Orders（訂單記錄）
  - Settings（設定）
- 當前頁面選項需高亮顯示
- 點擊切換對應功能頁

**Estimation:** 5 points

---

### US-033: 地址管理功能

**Description:**  
會員能新增、編輯、刪除收貨地址。

**Acceptance Criteria:**

- 顯示已儲存的地址列表
- 提供「Add New Address」按鈕
- 提供地址表單（收件人、電話、郵遞區號、地址）
- 可設定預設地址
- 可編輯現有地址
- 可刪除地址（至少保留一個）

**Estimation:** 8 points

---

### US-035: 收藏商品功能

**Description:**  
會員能收藏喜歡的商品，方便日後查看。

**Acceptance Criteria:**

- 商品頁提供「加入收藏」按鈕（愛心圖示）
- 已收藏商品顯示實心愛心
- 點擊可取消收藏
- 會員中心顯示收藏商品列表
- 可從收藏清單直接加入購物車
- 可從收藏清單移除商品

**Estimation:** 8 points

---

## Epic 7: 訂單管理

### US-036: 訂單列表頁

**Description:**  
會員能查看所有歷史訂單記錄。

**Acceptance Criteria:**

- 以表格形式顯示訂單
- 欄位包含：Order Number、Date、Status、Total Amount、Actions
- 訂單狀態以不同顏色標籤顯示（Shipped, Delivered, Processing, Cancelled）
- 每筆訂單提供「View Details」連結
- 依日期降冪排序（最新在前）

**Estimation:** 8 points

---

### US-037: 訂單搜尋功能

**Description:**  
會員能透過關鍵字搜尋訂單。

**Acceptance Criteria:**

- 提供搜尋框（Search orders）
- 可搜尋訂單編號
- 可搜尋商品名稱
- 即時顯示搜尋結果
- 無結果時顯示友善提示

**Estimation:** 5 points

---

### US-038: 訂單詳情頁

**Description:**  
會員能查看單一訂單的完整資訊。

**Acceptance Criteria:**

- 顯示訂單編號、日期、狀態
- 顯示收貨地址
- 顯示付款方式
- 顯示訂單商品清單（圖片、名稱、數量、單價、小計）
- 顯示訂單金額明細（小計、運費、稅金、總計）

**Estimation:** 8 points

---

### US-039: 訂單狀態追蹤

**Description:**  
會員能查看訂單的處理進度。

**Acceptance Criteria:**

- 顯示訂單狀態時間軸
- 狀態包含：訂單已建立、已付款、處理中、已出貨、已送達
- 每個狀態顯示更新時間

**Estimation:** 8 points

---

## Epic 8: 後台管理系統

### US-042: 管理員登入

**Description:**  
管理員能透過後台登入頁面進入管理系統。

**Acceptance Criteria:**

- 提供獨立的後台登入頁
- 驗證管理員權限
- 登入後進入後台儀表板
- 記錄登入日誌

**Estimation:** 5 points

---

### US-043: 商品管理 - 新增商品

**Description:**  
管理員能新增商品至系統。

**Acceptance Criteria:**

- 提供商品新增表單
- 輸入商品基本資訊（名稱、描述、價格、SKU）
- 選擇商品分類
- 上傳商品圖片（多張）
- 設定商品規格（顏色、尺寸、材質）
- 設定庫存數量
- 儲存後商品上架

**Estimation:** 13 points

---

### US-044: 商品管理 - 編輯商品

**Description:**  
管理員能修改現有商品資訊。

**Acceptance Criteria:**

- 顯示商品列表
- 可搜尋商品
- 點擊商品進入編輯頁
- 可修改所有商品欄位
- 可新增/刪除商品圖片
- 儲存後更新商品資訊

**Estimation:** 8 points

---

### US-045: 商品管理 - 刪除商品

**Description:**  
管理員能刪除不再銷售的商品。

**Acceptance Criteria:**

- 提供刪除按鈕
- 需要確認彈窗
- 軟刪除（保留資料但不顯示）
- 刪除後無法被搜尋或購買
- 記錄刪除日誌

**Estimation:** 5 points

---

### US-046: 圖片上傳 - Cloudinary 整合

**Description:**  
整合 Cloudinary 服務進行圖片儲存與管理。

**Acceptance Criteria:**

- 整合 Cloudinary API
- 上傳圖片至 Cloudinary
- 取得圖片 URL 並儲存至資料庫
- 支援圖片壓縮與縮放
- 支援多圖上傳
- 刪除商品時同步刪除 Cloudinary 圖片

**Estimation:** 13 points

---

### US-047: 分類管理

**Description:**  
管理員能管理商品分類。

**Acceptance Criteria:**

- 顯示分類列表
- 可新增分類（名稱、描述、圖片）
- 可編輯分類
- 可刪除分類（確認沒有商品使用）
- 支援分類排序

**Estimation:** 8 points

---

### US-048: 訂單管理 - 訂單列表

**Description:**  
管理員能查看所有訂單。

**Acceptance Criteria:**

- 顯示所有訂單列表
- 可依狀態篩選
- 可依日期範圍篩選
- 可搜尋訂單編號或會員
- 顯示訂單摘要資訊

**Estimation:** 8 points

---

### US-049: 訂單管理 - 更新訂單狀態

**Description:**  
管理員能手動更新訂單狀態。

**Acceptance Criteria:**

- 可變更訂單狀態（Processing → Shipped → Delivered）
- 更新物流資訊（物流單號）
- 發送狀態更新通知信給會員
- 記錄狀態變更歷程

**Estimation:** 8 points

---

### US-050: 會員管理

**Description:**  
管理員能查看與管理會員資料。

**Acceptance Criteria:**

- 顯示會員列表
- 可搜尋會員（姓名、Email、電話）
- 查看會員詳細資料
- 查看會員訂單歷史
- 可停用會員帳號
- 可重設會員密碼

**Estimation:** 8 points

---

### US-051: 庫存管理

**Description:**  
管理員能管理商品庫存數量。

**Acceptance Criteria:**

- 顯示所有商品庫存狀況
- 可手動調整庫存數量
- 設定低庫存警示閾值
- 顯示低庫存商品提醒

**Estimation:** 8 points

---

### US-052: 銷售報表

**Description:**  
管理員能查看銷售數據與報表。

**Acceptance Criteria:**

- 顯示日/週/月銷售額統計
- 顯示熱銷商品排行
- 顯示訂單數量統計
- 顯示會員成長趨勢
- 可匯出報表（CSV/Excel）
- 以圖表視覺化呈現

**Estimation:** 13 points

---

## Epic 9: 技術架構與優化

### US-053: MVC 路由設計

**Description:**  
設計並實作所有頁面的路由規則。

**Acceptance Criteria:**

- 定義所有 Controller 與 Action
- 設定路由規則（RouteConfig）
- 實作 RESTful 路由慣例
- 設定靜態檔案路徑

**Estimation:** 5 points

---

### US-054: ViewModel 設計

**Description:**  
為所有頁面設計對應的 ViewModel。

**Acceptance Criteria:**

- 設計首頁 ViewModel
- 設計商品列表 ViewModel
- 設計商品詳情 ViewModel
- 設計購物車 ViewModel
- 設計訂單 ViewModel
- 設計會員 ViewModel
- 使用 AutoMapper 進行物件映射

**Estimation:** 13 points

---

### US-055: 資料庫 Schema 設計

**Description:**  
設計電商系統的資料庫結構。

**Acceptance Criteria:**

- 設計 Entity Relationship Diagram
- 定義所有資料表與欄位
- 設定主鍵與外鍵關聯
- 設定索引以優化查詢
- 使用 Code First 建立 Migration
- 產生 Mermaid ER Diagram

**Estimation:** 13 points

---

### US-056: Repository Pattern 實作

**Description:**  
實作 Repository Pattern 抽象資料存取層。

**Acceptance Criteria:**

- 建立 Generic Repository Interface
- 實作 Generic Repository
- 為主要 Entity 建立專屬 Repository
- 實作 Unit of Work Pattern
- 統一資料庫交易管理

**Estimation:** 13 points

---

### US-057: Service Layer 實作

**Description:**  
實作 Service Layer 封裝商業邏輯。

**Acceptance Criteria:**

- 建立 Service Interface
- 實作各功能的 Service（Product, Order, Member, Cart）
- 分離商業邏輯與資料存取
- 使用 Dependency Injection

**Estimation:** 13 points

---

### US-058: RESTful API 設計

**Description:**  
設計並實作符合 RESTful 原則的 Web API。

**Acceptance Criteria:**

- 定義 API 路由規範（/api/products, /api/orders）
- 實作 CRUD API Endpoints
- 使用正確的 HTTP Methods（GET, POST, PUT, DELETE）
- 統一 API Response 格式
- 實作 API 版本控制
- 撰寫 API 文件（Swagger）

**Estimation:** 13 points

---

### US-059: 資料驗證 (Validation)

**Description:**  
實作完整的資料驗證機制。

**Acceptance Criteria:**

- 使用 Data Annotations 進行模型驗證
- 實作自定義驗證規則
- 前端驗證（JavaScript）
- 後端驗證（Controller & Service）
- 統一錯誤訊息格式
- 驗證失敗回傳友善錯誤訊息

**Estimation:** 8 points

---

### US-060: 搜尋與篩選優化

**Description:**  
優化商品搜尋與篩選功能的效能。

**Acceptance Criteria:**

- 實作搜尋參數物件
- 使用 LINQ 動態組合查詢條件
- 實作多條件篩選（AND/OR）
- 支援模糊搜尋（LIKE）
- 建立資料庫索引加速查詢

**Estimation:** 8 points

---

### US-061: 分頁機制實作

**Description:**  
實作通用的分頁機制。

**Acceptance Criteria:**

- 建立 PagedResult 類別
- 實作分頁查詢方法
- 支援自訂每頁筆數
- 回傳總筆數、總頁數、當前頁碼
- 前端實作分頁 UI 元件

**Estimation:** 5 points

---

### US-062: Redis Cache 整合

**Description:**  
整合 Redis 進行快取管理，提升效能。

**Acceptance Criteria:**

- 安裝與設定 Redis
- 整合 StackExchange.Redis
- 快取熱門商品資料
- 快取商品分類資料
- 設定快取過期時間
- 實作快取失效機制

**Estimation:** 13 points

---

### US-063: 錯誤處理與日誌記錄

**Description:**  
實作統一的錯誤處理與日誌記錄機制。

**Acceptance Criteria:**

- 實作全域錯誤處理 (Global Exception Handler)
- 整合日誌框架（如 NLog, Serilog）
- 記錄錯誤日誌
- 記錄重要操作日誌（登入、下單、付款）
- 顯示友善錯誤頁面
- 開發環境顯示詳細錯誤資訊

**Estimation:** 8 points

---

### US-064: 單元測試

**Description:**  
撰寫單元測試確保程式品質。

**Acceptance Criteria:**

- 使用 xUnit 或 NUnit
- 測試 Service Layer 商業邏輯
- 測試 Repository 資料存取
- 使用 Moq 進行 Mock
- 測試覆蓋率達 70% 以上

**Estimation:** 13 points

---

### US-065: 效能優化

**Description:**  
優化系統效能，提升使用者體驗。

**Acceptance Criteria:**

- 優化資料庫查詢（避免 N+1 問題）
- 使用 AsNoTracking 於唯讀查詢
- 實作 Lazy Loading 或 Eager Loading
- 壓縮靜態資源（CSS, JS）
- 啟用瀏覽器快取
- 使用 CDN 載入圖片

**Estimation:** 13 points

---

### US-066: 安全性強化

**Description:**  
強化系統安全性，防範常見攻擊。

**Acceptance Criteria:**

- 防範 SQL Injection（使用參數化查詢）
- 防範 XSS 攻擊（輸出編碼）
- 防範 CSRF 攻擊（AntiForgeryToken）
- 密碼加密儲存（bcrypt, PBKDF2）
- 實作 HTTPS
- 設定 Content Security Policy

**Estimation:** 8 points

---

## Sprint 規劃建議

### Sprint 1 (Week 1-2): 專案初始化與切版

- US-053: MVC 路由設計
- US-008: 響應式設計（RWD）
- 完成所有頁面靜態切版

### Sprint 2 (Week 3-4): 資料架構與核心功能

- US-055: 資料庫 Schema 設計
- US-054: ViewModel 設計
- US-056: Repository Pattern 實作
- US-057: Service Layer 實作

### Sprint 3 (Week 5-6): 首頁與商品列表

- US-001: 首頁 Banner 顯示＋導購按鈕
- US-002: 類別瀏覽/導覽區
- US-003: 新品推薦區
- US-004: 熱銷推薦區
- US-005: Header 導覽列
- US-007: Footer 區塊
- US-009: 商品列表頁顯示
- US-010: 商品篩選功能
- US-011: 商品分頁功能

### Sprint 4 (Week 7-8): 商品詳情與購物車

- US-013: 商品詳細資訊展示
- US-014: 麵包屑導航
- US-015: 加入購物車功能
- US-016: 庫存狀態顯示
- US-017: 顧客評價區
- US-018: 相關商品推薦
- US-019: 購物車商品列表
- US-020: 購物車數量調整
- US-021: 訂單摘要計算
- US-022: 繼續購物與結帳按鈕

### Sprint 5 (Week 9-10): 會員系統

- US-025: 會員登入頁
- US-026: 會員註冊功能
- US-027: 忘記密碼功能
- US-030: 會員個人資訊管理
- US-031: 會員密碼變更
- US-032: 會員側邊欄導航
- US-033: 地址管理功能
- US-035: 收藏商品功能

### Sprint 6 (Week 11-12): 訂單與結帳

- US-023: 結帳流程（訂單建立）
- US-036: 訂單列表頁
- US-037: 訂單搜尋功能
- US-038: 訂單詳情頁
- US-039: 訂單狀態追蹤
- US-040: 取消訂單功能

### Sprint 7 (Week 13-14): 第三方整合

- US-024: 金流整合 - ECPay
- US-028: 第三方登入 - Google
- US-029: 第三方登入 - LINE
- US-046: 圖片上傳 - Cloudinary 整合

### Sprint 8 (Week 15-16): 後台管理系統

- US-042: 管理員登入
- US-043: 商品管理 - 新增商品
- US-044: 商品管理 - 編輯商品
- US-045: 商品管理 - 刪除商品
- US-047: 分類管理
- US-048: 訂單管理 - 訂單列表
- US-049: 訂單管理 - 更新訂單狀態
- US-050: 會員管理
- US-051: 庫存管理

### Sprint 9 (Week 17-18): API 與優化

- US-058: RESTful API 設計
- US-059: 資料驗證 (Validation)
- US-060: 搜尋與篩選優化
- US-061: 分頁機制實作
- US-062: Redis Cache 整合
- US-063: 錯誤處理與日誌記錄

### Sprint 10 (Week 19-20): 測試與上線準備

- US-064: 單元測試
- US-065: 效能優化
- US-066: 安全性強化
- US-041: 退貨申請功能
- US-052: 銷售報表
- 整合測試與 Bug 修復
- 部署與上線

---

## 總計

- **Total User Stories: 66**
- **Total Story Points: 530**
- **Estimated Duration: 20 weeks (5 months)**
