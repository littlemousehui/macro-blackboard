---
type: log
---

# 維護紀錄 Log

只能附加，最新在最下面。標題格式：`## [YYYY-MM-DD] 動作 | 標題`，動作為 ingest / query / lint / schema。

## [2026-11-23] schema | 建立知識庫
- 建立 `CLAUDE.md`（學習型、繁中術語附英文、免安裝圖形呈現）
- 建立資料夾骨架、`index`、`log`、`overview`、`glossary`
- 建立 `tools/pptx2md.ps1`（PPTX 轉文字）
- 未安裝 git，版本紀錄依賴 OneDrive 版本歷史

## [2026-11-23] schema | 新增 raw/papers/
- 對話中提供的 PDF 簡報檔一律存入 `raw/papers/`（複製、保留原檔名、不覆蓋同名檔）

## [2026-11-23] ingest | 第3章 成長與累積（ch3.pdf）
- 來源：`raw/papers/ch3.pdf`（33 張）→ [第3章 成長與累積](sources/%E7%AC%AC3%E7%AB%A0%20%E6%88%90%E9%95%B7%E8%88%87%E7%B4%AF%E7%A9%8D.md)
- 新增模型：[Solow 新古典成長模型](models/Solow%20%E6%96%B0%E5%8F%A4%E5%85%B8%E6%88%90%E9%95%B7%E6%A8%A1%E5%9E%8B.md)
- 新增概念：[生產函數](concepts/%E7%94%9F%E7%94%A2%E5%87%BD%E6%95%B8.md)、[成長核算](concepts/%E6%88%90%E9%95%B7%E6%A0%B8%E7%AE%97.md)、[全要素生產力 (TFP)](concepts/%E5%85%A8%E8%A6%81%E7%B4%A0%E7%94%9F%E7%94%A2%E5%8A%9B%20%28TFP%29.md)、[人力資本](concepts/%E4%BA%BA%E5%8A%9B%E8%B3%87%E6%9C%AC.md)、[穩態](concepts/%E7%A9%A9%E6%85%8B.md)、[損益兩平投資](concepts/%E6%90%8D%E7%9B%8A%E5%85%A9%E5%B9%B3%E6%8A%95%E8%B3%87.md)、[邊際報酬遞減](concepts/%E9%82%8A%E9%9A%9B%E5%A0%B1%E9%85%AC%E9%81%9E%E6%B8%9B.md)、[收斂](concepts/%E6%94%B6%E6%96%82.md)、[黃金法則](concepts/%E9%BB%83%E9%87%91%E6%B3%95%E5%89%87.md)
- 新增指標：[人均 GDP](indicators/%E4%BA%BA%E5%9D%87%20GDP.md)；事件：[阿根廷的世紀衰退](events/%E9%98%BF%E6%A0%B9%E5%BB%B7%E7%9A%84%E4%B8%96%E7%B4%80%E8%A1%B0%E9%80%80.md)；人物：[梭羅 (Robert Solow)](people/%E6%A2%AD%E7%BE%85%20%28Robert%20Solow%29.md)
- 新增綜合：[s、n、g 變動效果比較](synthesis/s%E3%80%81n%E3%80%81g%20%E8%AE%8A%E5%8B%95%E6%95%88%E6%9E%9C%E6%AF%94%E8%BC%83.md)
- 更新：[glossary](glossary.md)（30 個術語＋符號）、[overview](overview.md)（學習路徑）、[index](index.md)
- 🔣 折舊率 $d$ / $\delta$ 混用，統一為 $\delta$
- ⚠️ 第 28 張 TFP 寫法（殘差）已加註；第 31 張「貨幣政策調整儲蓄率」待確認
- 待確認：推測教材（Dornbusch-Fischer-Startz）、手寫註記作者

## [2026-11-23] schema | 課堂筆記與 outputs/
- 使用者確認：投影片上的手寫註記是本人的課堂筆記 → wiki 內統一標為「📝 課堂筆記」
- `CLAUDE.md` 新增 `outputs/slides/` 資料夾與 Output 流程（內容只取自 wiki、單檔離線、初學者導向）

## [2026-11-23] output | 第3章 成長與累積 HTML 簡報
- 產出 `outputs/slides/第3章 成長與累積.html`（23 頁）
- 取材：[第3章 成長與累積](sources/%E7%AC%AC3%E7%AB%A0%20%E6%88%90%E9%95%B7%E8%88%87%E7%B4%AF%E7%A9%8D.md)、[Solow 新古典成長模型](models/Solow%20%E6%96%B0%E5%8F%A4%E5%85%B8%E6%88%90%E9%95%B7%E6%A8%A1%E5%9E%8B.md)、[成長核算](concepts/%E6%88%90%E9%95%B7%E6%A0%B8%E7%AE%97.md)、[黃金法則](concepts/%E9%BB%83%E9%87%91%E6%B3%95%E5%89%87.md)、[s、n、g 變動效果比較](synthesis/s%E3%80%81n%E3%80%81g%20%E8%AE%8A%E5%8B%95%E6%95%88%E6%9E%9C%E6%AF%94%E8%BC%83.md) 等
- 初學者設計：麵包店比喻（Y/K/N/A）、水桶比喻（流入 sf(k)、流出 (n+δ)k）、先直覺後公式
- 圖表為內嵌 SVG，使用示意參數（非實際數據）；阿根廷圖為目測約值

## [2026-11-23] output | 第3章簡報改為黑板教學風
- 依使用者要求改版：黑板底、粉筆筆觸、木框、粉筆槽導覽、便利貼課堂筆記、封面加塗鴉與「值日生」角落
- `CLAUDE.md` 將黑板風設為簡報預設樣式

## [2026-11-23] output | 第3章簡報字型改為微軟正黑體
- 使用者覺得標楷體老氣 → 改用 Segoe UI＋微軟正黑體；`CLAUDE.md` 樣式說明同步更新
- 窄螢幕時封面右上角「今日主題」改為不浮動，避免與標題重疊

## [2026-11-23] output | 第3章簡報封面改版
- 使用者覺得封面太空 → 改左右兩欄：左邊標題、問題、資訊標籤；右邊三線塗鴉圖（富國／阿根廷／停滯）＋「今天的課程」四單元大綱
- 修正封面高度超出畫面造成的捲軸

## [2026-11-23] output | 簡報流程 graph 試跑：第3章
- 節點 1：`outputs/slides/第3章/outline.md`（22 頁）→ 自動檢查通過（提醒 2 項）→ 關卡一通過
- 節點 2：`slides.md` 逐頁腳本 → 自動檢查硬性全過（提醒：P22 密度最高）
- 節點 3：`index.html` 由黑板模板渲染 → 瀏覽器檢查抓到 3 頁標題與腳本不一致、寬螢幕留白，已修
- 試跑發現：wiki 連結無方向，前置順序需人工判斷（可考慮 frontmatter `prereq:`）
- 狀態：等待關卡二驗收；舊版 `outputs/slides/第3章 成長與累積.html` 未動

## [2026-11-23] schema | 簡報產生 graph 定案
- 關卡二驗收通過 → `CLAUDE.md` 的 Output 改為正式流程：大綱 → 逐頁腳本 → 渲染，各接自動檢查（loop），關卡一（大綱）＋關卡二（驗收）
- 納入試跑學到的修正：渲染從模板＋slides.md 重新產生、瀏覽器檢查加「標題一致」「寬螢幕留白」、模板改指向 `outputs/slides/第3章/index.html`
- 未定：wiki frontmatter 是否加 `prereq:`

## [2026-11-23] output | 刪除舊版第3章簡報
- 依使用者指示將 `outputs/slides/第3章 成長與累積.html`（23 頁舊版）移到資源回收筒；現行版本為 `outputs/slides/第3章/index.html`

## [2026-11-23] output | 簡報流程圖 PNG
- 將 CLAUDE.md 的簡報 graph（Mermaid）用 Windows 內建 Edge 無頭模式截圖，存成 `outputs/diagrams/簡報產生流程.png`（940×2740，2 倍解析度）

## [2026-11-23] output | 單元首頁
- 新增 `outputs/slides/index.html`：黑板風單元卡片頁，已上架單元為大卡片（第3章），另有 4 張「單元準備中」佔位卡（使用者將再提供四份簡報）
- 第3章簡報導覽列加「🏠 首頁」連結
- `CLAUDE.md` 交付步驟加入「更新首頁 UNITS 陣列」

## [2026-11-23] ingest | 第4章 成長與政策（ch04.pdf）
- 來源：`raw/papers/ch04.pdf`（25 張）→ [第4章 成長與政策](sources/%E7%AC%AC4%E7%AB%A0%20%E6%88%90%E9%95%B7%E8%88%87%E6%94%BF%E7%AD%96.md)
- 新增模型：[內生成長模型 (AK 模型)](models/%E5%85%A7%E7%94%9F%E6%88%90%E9%95%B7%E6%A8%A1%E5%9E%8B%20%28AK%20%E6%A8%A1%E5%9E%8B%29.md)、[兩部門成長模型](models/%E5%85%A9%E9%83%A8%E9%96%80%E6%88%90%E9%95%B7%E6%A8%A1%E5%9E%8B.md)、[內生人口成長的 Solow 模型](models/%E5%85%A7%E7%94%9F%E4%BA%BA%E5%8F%A3%E6%88%90%E9%95%B7%E7%9A%84%20Solow%20%E6%A8%A1%E5%9E%8B.md)
- 新增概念：[外部效應與社會報酬](concepts/%E5%A4%96%E9%83%A8%E6%95%88%E6%87%89%E8%88%87%E7%A4%BE%E6%9C%83%E5%A0%B1%E9%85%AC.md)、[規模報酬](concepts/%E8%A6%8F%E6%A8%A1%E5%A0%B1%E9%85%AC.md)、[貧窮陷阱](concepts/%E8%B2%A7%E7%AA%AE%E9%99%B7%E9%98%B1.md)、[大推力](concepts/%E5%A4%A7%E6%8E%A8%E5%8A%9B.md)；政策：[成長政策](policies/%E6%88%90%E9%95%B7%E6%94%BF%E7%AD%96.md)
- 新增人物：[羅默 (Paul Romer)](people/%E7%BE%85%E9%BB%98%20%28Paul%20Romer%29.md)、[盧卡斯 (Robert Lucas)](people/%E7%9B%A7%E5%8D%A1%E6%96%AF%20%28Robert%20Lucas%29.md)、[巴羅 (Robert Barro)](people/%E5%B7%B4%E7%BE%85%20%28Robert%20Barro%29.md)、[顧志耐 (Simon Kuznets)](people/%E9%A1%A7%E5%BF%97%E8%80%90%20%28Simon%20Kuznets%29.md)；事件：[迦納的長期停滯](events/%E8%BF%A6%E7%B4%8D%E7%9A%84%E9%95%B7%E6%9C%9F%E5%81%9C%E6%BB%AF.md)；綜合：[新古典 vs 內生成長理論](synthesis/%E6%96%B0%E5%8F%A4%E5%85%B8%20vs%20%E5%85%A7%E7%94%9F%E6%88%90%E9%95%B7%E7%90%86%E8%AB%96.md)
- 更新：[阿根廷的世紀衰退](events/%E9%98%BF%E6%A0%B9%E5%BB%B7%E7%9A%84%E4%B8%96%E7%B4%80%E8%A1%B0%E9%80%80.md)、[收斂](concepts/%E6%94%B6%E6%96%82.md)（條件收斂改為有出處）、[Solow 新古典成長模型](models/Solow%20%E6%96%B0%E5%8F%A4%E5%85%B8%E6%88%90%E9%95%B7%E6%A8%A1%E5%9E%8B.md)（限制改為有出處）、[人力資本](concepts/%E4%BA%BA%E5%8A%9B%E8%B3%87%E6%9C%AC.md)、[邊際報酬遞減](concepts/%E9%82%8A%E9%9A%9B%E5%A0%B1%E9%85%AC%E9%81%9E%E6%B8%9B.md)、[全要素生產力 (TFP)](concepts/%E5%85%A8%E8%A6%81%E7%B4%A0%E7%94%9F%E7%94%A2%E5%8A%9B%20%28TFP%29.md)、[s、n、g 變動效果比較](synthesis/s%E3%80%81n%E3%80%81g%20%E8%AE%8A%E5%8B%95%E6%95%88%E6%9E%9C%E6%AF%94%E8%BC%83.md)、[glossary](glossary.md)（23 術語＋a/α/g/n(y) 符號）、[overview](overview.md)、[index](index.md)
- 🔣 d→δ；g 在第4章指 Δy/y；a 與 α 區分
- ⚠️ 第 15 張課堂筆記 s·k/y 應為 s·y/k；第 25 張儲蓄率未標年份
- 🔀 內生成長理論 vs Barro 實證
- 第 11–12 張塗鴉不收錄

## [2026-11-23] output | 第4章簡報（依簡報 graph）
- 節點 1：`outputs/slides/第4章/outline.md`（22 頁）→ 自動檢查全過（提醒：省略推導、需第3章前置）→ 關卡一通過
- 節點 2：`slides.md` → 硬性檢查全過（提醒：P22 密度最高）
- 節點 3：`index.html` 由模板＋腳本重新產生（6 張新圖：AK 直線、收斂路徑×2、兩部門、三均衡、Solow 迷你圖）→ 瀏覽器檢查抓到 P12 標籤重疊、P18 曲線不單調，已修
- 狀態：等待關卡二驗收；驗收後上架首頁
- 關卡二驗收通過 → 首頁 `UNITS` 加入第4章（藍色卡片、「建議先看：第 3 章」），佔位卡剩 3 張；首頁卡片新增 `prereq` 欄位顯示

## [2026-11-23] schema | 瀏覽器檢查新增「曲線形狀」
- 經使用者同意，`CLAUDE.md` 節點 3 瀏覽器檢查加入「曲線形狀符合原簡報描述」（截圖逐張看＋程式驗證單調性、交點數、穩定方向、凹凸）
- 起因：第4章 P18 必要投資線原本有一段往下彎，原檢查清單抓不到

## [2026-11-24] ingest | 第14章 消費與儲蓄（ch14.pdf）
- 來源：`raw/papers/ch14.pdf`（18 張）→ [第14章 消費與儲蓄](sources/%E7%AC%AC14%E7%AB%A0%20%E6%B6%88%E8%B2%BB%E8%88%87%E5%84%B2%E8%93%84.md)
- 新增模型：[凱因斯消費函數](models/%E5%87%B1%E5%9B%A0%E6%96%AF%E6%B6%88%E8%B2%BB%E5%87%BD%E6%95%B8.md)、[生命週期理論](models/%E7%94%9F%E5%91%BD%E9%80%B1%E6%9C%9F%E7%90%86%E8%AB%96.md)、[恆常所得理論](models/%E6%81%86%E5%B8%B8%E6%89%80%E5%BE%97%E7%90%86%E8%AB%96.md)、[隨機漫步消費模型 (Hall)](models/%E9%9A%A8%E6%A9%9F%E6%BC%AB%E6%AD%A5%E6%B6%88%E8%B2%BB%E6%A8%A1%E5%9E%8B%20%28Hall%29.md)
- 新增概念：[邊際消費傾向 (MPC)](concepts/%E9%82%8A%E9%9A%9B%E6%B6%88%E8%B2%BB%E5%82%BE%E5%90%91%20%28MPC%29.md)、[恆常所得與暫時所得](concepts/%E6%81%86%E5%B8%B8%E6%89%80%E5%BE%97%E8%88%87%E6%9A%AB%E6%99%82%E6%89%80%E5%BE%97.md)、[消費平滑化](concepts/%E6%B6%88%E8%B2%BB%E5%B9%B3%E6%BB%91%E5%8C%96.md)、[流動性限制與短視](concepts/%E6%B5%81%E5%8B%95%E6%80%A7%E9%99%90%E5%88%B6%E8%88%87%E7%9F%AD%E8%A6%96.md)、[預防性儲蓄與緩衝儲備](concepts/%E9%A0%90%E9%98%B2%E6%80%A7%E5%84%B2%E8%93%84%E8%88%87%E7%B7%A9%E8%A1%9D%E5%84%B2%E5%82%99.md)
- 新增指標：[民間消費](indicators/%E6%B0%91%E9%96%93%E6%B6%88%E8%B2%BB.md)；政策：[消費券](policies/%E6%B6%88%E8%B2%BB%E5%88%B8.md)；人物：[傅利曼 (Milton Friedman)](people/%E5%82%85%E5%88%A9%E6%9B%BC%20%28Milton%20Friedman%29.md)、[霍爾 (Robert Hall)](people/%E9%9C%8D%E7%88%BE%20%28Robert%20Hall%29.md)；綜合：[消費理論比較](synthesis/%E6%B6%88%E8%B2%BB%E7%90%86%E8%AB%96%E6%AF%94%E8%BC%83.md)
- 更新：[Solow 新古典成長模型](models/Solow%20%E6%96%B0%E5%8F%A4%E5%85%B8%E6%88%90%E9%95%B7%E6%A8%A1%E5%9E%8B.md)（儲蓄假設連到本章）、[第3章 成長與累積](sources/%E7%AC%AC3%E7%AB%A0%20%E6%88%90%E9%95%B7%E8%88%87%E7%B4%AF%E7%A9%8D.md)／[第4章 成長與政策](sources/%E7%AC%AC4%E7%AB%A0%20%E6%88%90%E9%95%B7%E8%88%87%E6%94%BF%E7%AD%96.md)（教材推測加 McGraw-Hill 2014 證據）、[glossary](glossary.md)（23 術語＋8 符號）、[overview](overview.md)（新增第 5 單元）、[index](index.md)
- 🔣 小寫 c：第3章人均消費 vs 本章 MPC；WL、NL 非乘積
- ⚠️ 財富的 MPC 實為 1 ÷ 剩餘年數（加註）
- 補充：台灣 2009 消費券每人 3,600 元（非簡報內容）

## [2026-11-24] output | 第14章簡報（依簡報 graph）
- 節點 1：`outputs/slides/第14章/outline.md`（20 頁）→ 自動檢查全過（提醒：省略 Hall 推導、補充內容較多）→ 關卡一通過
- 節點 2：`slides.md` → 硬性檢查全過（提醒：P12 密度最高）
- 節點 3：`index.html` 由模板＋腳本重新產生（新圖：所得 vs 消費、45 度線、凱因斯直線、生命週期）→ 瀏覽器檢查（首次套用「曲線形狀」檢查，全過）抓到 P05 標籤重疊、P11 圖文不一致，已修
- 狀態：等待關卡二驗收
- 關卡二驗收通過 → 首頁 `UNITS` 加入第14章（粉紅色卡片，無前置），佔位卡剩 2 張

## [2026-11-24] ingest | 第13章 國際連結（ch13.pdf）
- 來源：`raw/papers/ch13.pdf`（43 張，含 IS-LM 附錄）→ [第13章 國際連結](sources/%E7%AC%AC13%E7%AB%A0%20%E5%9C%8B%E9%9A%9B%E9%80%A3%E7%B5%90.md)
- 新增模型：[Mundell-Fleming 模型](models/Mundell-Fleming%20%E6%A8%A1%E5%9E%8B.md)、[IS-LM 模型](models/IS-LM%20%E6%A8%A1%E5%9E%8B.md)
- 新增概念：[名目匯率與實質匯率](concepts/%E5%90%8D%E7%9B%AE%E5%8C%AF%E7%8E%87%E8%88%87%E5%AF%A6%E8%B3%AA%E5%8C%AF%E7%8E%87.md)、[購買力平價 (PPP)](concepts/%E8%B3%BC%E8%B2%B7%E5%8A%9B%E5%B9%B3%E5%83%B9%20%28PPP%29.md)、[資本移動性](concepts/%E8%B3%87%E6%9C%AC%E7%A7%BB%E5%8B%95%E6%80%A7.md)、[淨出口](concepts/%E6%B7%A8%E5%87%BA%E5%8F%A3.md)、[邊際進口傾向](concepts/%E9%82%8A%E9%9A%9B%E9%80%B2%E5%8F%A3%E5%82%BE%E5%90%91.md)、[外匯干預與外匯存底](concepts/%E5%A4%96%E5%8C%AF%E5%B9%B2%E9%A0%90%E8%88%87%E5%A4%96%E5%8C%AF%E5%AD%98%E5%BA%95.md)
- 新增指標：[國際收支](indicators/%E5%9C%8B%E9%9A%9B%E6%94%B6%E6%94%AF.md)；政策：[匯率制度](policies/%E5%8C%AF%E7%8E%87%E5%88%B6%E5%BA%A6.md)；事件：[2022 新興市場風險](events/2022%20%E6%96%B0%E8%88%88%E5%B8%82%E5%A0%B4%E9%A2%A8%E9%9A%AA.md)；人物：[孟岱爾 (Robert Mundell)](people/%E5%AD%9F%E5%B2%B1%E7%88%BE%20%28Robert%20Mundell%29.md)、[弗萊明 (Marcus Fleming)](people/%E5%BC%97%E8%90%8A%E6%98%8E%20%28Marcus%20Fleming%29.md)；綜合：[開放經濟下的政策效果](synthesis/%E9%96%8B%E6%94%BE%E7%B6%93%E6%BF%9F%E4%B8%8B%E7%9A%84%E6%94%BF%E7%AD%96%E6%95%88%E6%9E%9C.md)
- 更新：[阿根廷的世紀衰退](events/%E9%98%BF%E6%A0%B9%E5%BB%B7%E7%9A%84%E4%B8%96%E7%B4%80%E8%A1%B0%E9%80%80.md)（2021 脆弱度第一）、[人均 GDP](indicators/%E4%BA%BA%E5%9D%87%20GDP.md)（連到 PPP）、[邊際消費傾向 (MPC)](concepts/%E9%82%8A%E9%9A%9B%E6%B6%88%E8%B2%BB%E5%82%BE%E5%90%91%20%28MPC%29.md)（對照邊際進口傾向）、[glossary](glossary.md)（28 術語＋11 符號）、[overview](overview.md)、[index](index.md)
- ⚠️ 第 22 張 R 誤稱 real interest rate；第 35 張 inflows 應為 outflows
- 🔣 進口統一用 Q（附錄的 M 與貨幣衝突）

## [2026-11-24] output | 第13章簡報（依簡報 graph）
- 節點 1：`outputs/slides/第13章/outline.md`（24 頁）→ 自動檢查（補上弗萊明）→ 關卡一通過
- 節點 2：`slides.md` → 硬性檢查全過（提醒：本章整體偏密，7 頁超過 300 字）
- 節點 3：`index.html` 由模板＋腳本重新產生（10 張新圖）→ 瀏覽器檢查一次全過（曲線形狀、圖文一致、溢出、重疊、手機）
- 狀態：等待關卡二驗收
- 關卡二驗收通過 → 首頁 `UNITS` 加入第13章（綠色卡片、「建議先看：第 14 章」，依章次排在第14章前），佔位卡剩 1 張

## [2026-11-24] ingest | 第15章 投資支出（ch15.pdf）
- 來源：`raw/papers/ch15.pdf`（21 張）→ [第15章 投資支出](sources/%E7%AC%AC15%E7%AB%A0%20%E6%8A%95%E8%B3%87%E6%94%AF%E5%87%BA.md)
- 新增模型：[最適資本存量](models/%E6%9C%80%E9%81%A9%E8%B3%87%E6%9C%AC%E5%AD%98%E9%87%8F.md)、[彈性加速模型](models/%E5%BD%88%E6%80%A7%E5%8A%A0%E9%80%9F%E6%A8%A1%E5%9E%8B.md)
- 新增概念：[資本的租賃成本](concepts/%E8%B3%87%E6%9C%AC%E7%9A%84%E7%A7%9F%E8%B3%83%E6%88%90%E6%9C%AC.md)、[實質利率與預期通膨](concepts/%E5%AF%A6%E8%B3%AA%E5%88%A9%E7%8E%87%E8%88%87%E9%A0%90%E6%9C%9F%E9%80%9A%E8%86%A8.md)、[流量與存量](concepts/%E6%B5%81%E9%87%8F%E8%88%87%E5%AD%98%E9%87%8F.md)、[存貨投資](concepts/%E5%AD%98%E8%B2%A8%E6%8A%95%E8%B3%87.md)
- 新增指標：[投資的組成](indicators/%E6%8A%95%E8%B3%87%E7%9A%84%E7%B5%84%E6%88%90.md)；事件：[疫後投資熱潮 (2021–2022)](events/%E7%96%AB%E5%BE%8C%E6%8A%95%E8%B3%87%E7%86%B1%E6%BD%AE%20%282021%E2%80%932022%29.md)、[大衰退中的存貨 (2008–2009)](events/%E5%A4%A7%E8%A1%B0%E9%80%80%E4%B8%AD%E7%9A%84%E5%AD%98%E8%B2%A8%20%282008%E2%80%932009%29.md)；綜合：[投資的決定因素](synthesis/%E6%8A%95%E8%B3%87%E7%9A%84%E6%B1%BA%E5%AE%9A%E5%9B%A0%E7%B4%A0.md)
- 更新：[IS-LM 模型](models/IS-LM%20%E6%A8%A1%E5%9E%8B.md)（I(i) 的個體基礎）、[邊際報酬遞減](concepts/%E9%82%8A%E9%9A%9B%E5%A0%B1%E9%85%AC%E9%81%9E%E6%B8%9B.md)、[Solow 新古典成長模型](models/Solow%20%E6%96%B0%E5%8F%A4%E5%85%B8%E6%88%90%E9%95%B7%E6%A8%A1%E5%9E%8B.md)、[第3章 成長與累積](sources/%E7%AC%AC3%E7%AB%A0%20%E6%88%90%E9%95%B7%E8%88%87%E7%B4%AF%E7%A9%8D.md)／[第4章 成長與政策](sources/%E7%AC%AC4%E7%AB%A0%20%E6%88%90%E9%95%B7%E8%88%87%E6%94%BF%E7%AD%96.md)（教材證據）、[glossary](glossary.md)（21 術語＋6 符號）、[overview](overview.md)、[index](index.md)
- 頁名「最適資本存量 (K*)」因 Windows 檔名不能含 * 改為「最適資本存量」，K* 放在別名
- ⚠️ 第 2 張日期疑為 2022-02-05；第 21 張座標軸標籤對調
- 🔣 d→δ；r（實質利率）vs R（實質匯率）

## [2026-11-24] output | 第15章簡報（依簡報 graph）
- 節點 1：`outputs/slides/第15章/outline.md`（19 頁）→ 自動檢查全過 → 關卡一通過
- 節點 2：`slides.md` → 自動檢查抓到錯字（恆復→恢復）已修，硬性全過
- 節點 3：`index.html` 由模板＋腳本重新產生（7 張新圖＋雙長條）→ 瀏覽器檢查抓到 2 處標籤重疊、P02 手機橫向捲動、房貸 vs 住宅示意線不夠反向（只畫 1973–2006 並註明例外），均已修
- 狀態：等待關卡二驗收
- 關卡二驗收通過 → 首頁 `UNITS` 加入第15章（橘色卡片、「建議先看：第 13 章」），最後一張佔位卡移除，**5 個單元全部上架**

## [2026-11-24] lint | 第一次健康檢查（5 份來源後）
- 結構：75 頁、0 失效連結、0 孤兒頁、index 與檔案同步、frontmatter 齊全；`schools/` 為空
- 待處理（等使用者同意）：overview 仍是「暫定」通用架構且編號重複；總需求／財政政策／貨幣政策／央行／景氣循環被多頁提到但沒有自己的頁；3 個頁面只有 1 個連入；glossary 沒有人物區
- 確認無誤：d／δ、進口 Q、台灣用語（人物頁別名裡的大陸譯名為刻意保留以便搜尋）、學派分歧 🔀 標記一致
- 更正：先前回報「15 個模型、7 個綜合頁」有誤，實際為 12 個模型、5 個綜合頁

## [2026-11-24] lint | 依健康檢查修正（使用者同意全部修正）
- [overview](overview.md) 改寫：依實際 5 章重畫課程地圖（長期成長／總需求兩條主線）、單元表含建議先看、移除通用暫定架構與重複編號
- 新增跨章整合頁（內容只取自既有 wiki）：[總需求](concepts/%E7%B8%BD%E9%9C%80%E6%B1%82.md)、[貨幣政策](policies/%E8%B2%A8%E5%B9%A3%E6%94%BF%E7%AD%96.md)（含央行）、[財政政策](policies/%E8%B2%A1%E6%94%BF%E6%94%BF%E7%AD%96.md)、[景氣循環](concepts/%E6%99%AF%E6%B0%A3%E5%BE%AA%E7%92%B0.md)
- 補連結：[疫後投資熱潮 (2021–2022)](events/%E7%96%AB%E5%BE%8C%E6%8A%95%E8%B3%87%E7%86%B1%E6%BD%AE%20%282021%E2%80%932022%29.md)、[大衰退中的存貨 (2008–2009)](events/%E5%A4%A7%E8%A1%B0%E9%80%80%E4%B8%AD%E7%9A%84%E5%AD%98%E8%B2%A8%20%282008%E2%80%932009%29.md)（自[投資的決定因素](synthesis/%E6%8A%95%E8%B3%87%E7%9A%84%E6%B1%BA%E5%AE%9A%E5%9B%A0%E7%B4%A0.md)、[最適資本存量](models/%E6%9C%80%E9%81%A9%E8%B3%87%E6%9C%AC%E5%AD%98%E9%87%8F.md)、[景氣循環](concepts/%E6%99%AF%E6%B0%A3%E5%BE%AA%E7%92%B0.md)）；[顧志耐 (Simon Kuznets)](people/%E9%A1%A7%E5%BF%97%E8%80%90%20%28Simon%20Kuznets%29.md)（自[收斂](concepts/%E6%94%B6%E6%96%82.md)）
- [glossary](glossary.md) 新增「跨章主題」與「人物」對照表

## [2026-11-24] output | 流程圖 PNG 更新
- `CLAUDE.md` 的 Mermaid 流程圖同步現行流程：瀏覽器檢查節點加「含曲線形狀」、交付節點加「上架首頁」
- 重新輸出 `outputs/diagrams/簡報產生流程.png`（960×2900，2 倍解析度），覆蓋舊版（舊版可從 OneDrive 版本歷程還原）

## [2026-11-24] output | GitHub Pages 上傳資料夾
- 依使用者提供的〈把作品放上 GitHub Pages：給新手的上傳指引〉，建立 `publish/macro-blackboard/`
- 指引要求檔名用英文小寫，故章節資料夾改名：第3章→ch03、第4章→ch04、第13章→ch13、第14章→ch14、第15章→ch15；首頁連結同步改寫；各簡報的「🏠 首頁」連結（../index.html）不需改
- 只放網站需要的 6 個 HTML，不放 outline.md、slides.md；無外部資源、單檔皆 < 60 KB
- 原本 `outputs/slides/` 不動；之後改了簡報要重新複製一次到 publish/
