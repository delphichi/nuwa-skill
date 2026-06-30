# 05 重大決策與行動記錄

> 調研時間：2026/06/30
> 範圍：從 1993 創立 NVIDIA 到 2026 GTC Taipei，覆蓋公司級與個人級決策、危機時刻、結構性「沒做」的決策。
> 行為證據比語言更可靠——本檔聚焦「他做了什麼」而非「他說了什麼」。

---

## 公司級重大決策（時間排序）

### 1. 1993/04 創立 NVIDIA — 在 Denny's 餐廳的賭注
**背景**：30 歲的黃仁勳當時是 LSI Logic 的 CoreWare 主管，前 AMD 微處理器設計師。產業共識認為 PC 圖形是「副業」，沒人看好獨立顯卡。
**決策**：與 Chris Malachowsky（Sun Microsystems）、Curtis Priem（IBM/Sun 圖形晶片設計師）在 East San Jose 一間 Denny's 餐廳開了無數次會議，最終於 1993/04/05 成立 NVIDIA。
**邏輯**：他事後解釋——選 Denny's 是「比家裡安靜、咖啡便宜」，這是他打第一份工的地方。公司名 NVIDIA 來自拉丁文 *invidia*（嫉妒）。
**資本**：起始 $40K（≈2025 年 $89K）。
**結果**：30 年後變成市值 $5T 的公司。
**證據**：https://blogs.nvidia.com/blog/nvidia-dennys-trillion/ ; https://en.wikipedia.org/wiki/Nvidia ; Sequoia Crucible Moments: https://sequoiacap.com/podcast/crucible-moments-nvidia/

---

### 2. 1995 NV1 失敗 → Riva 128 救命
**背景**：NV1 押注「quadratic texture mapping」（曲面貼圖）而非業界主流 polygon。結果 Microsoft 推 Direct3D 強制 polygon，NV1 一夜過時。
**決策**：黃仁勳主動承認錯誤，放棄 NV1 與 OpenGL 標準之爭，全公司 ALL-IN 賭 Riva 128。當時只剩一個月工資。
**邏輯**：「30 days from going out of business」這句話此後成為他用了 33 年的內部口頭禪——每次全員會議都用這句開場。
**結果**：Riva 128 大成功，公司活下來。1997 與 TSMC 建立合作關係（Morris Chang 寫信開始）。
**證據**：https://semiwiki.com/uncategorized/699-nvidia-30-days-from-going-out-of-business/ ; https://fortune.com/2025/12/04/nvidia-ceo-admits-he-works-7-days-a-week-including-holidays-in-a-constant-state-of-anxiety-out-of-fear-of-going-bankrupt/

---

### 3. 1999/01/22 IPO + 推出「GPU」一詞
**決策**：上市；同年推出 GeForce 256，自己造一個新類別 "Graphics Processing Unit"。
**邏輯**：「市場類別決定估值——如果只是 graphics card，估值上限就被定死了」。
**結果**：成功為自己定義了新市場。

---

### 4. 2006-2007 押注 CUDA — 公司歷史最大的 zero-billion 賭注
**背景**：當時 GPU 主要做圖形，CUDA 是把 GPU 變成通用計算平台的瘋狂主意。Wall Street 完全看不懂。
**決策**：強制所有 NVIDIA GPU（包含 gaming）都加入 CUDA 支援，硬體成本上升、毛利下降。2006-2017 年 NVIDIA 投入近 $12B R&D 在 CUDA 生態。
**邏輯**：他事後解釋——「如果一件事我們有獨家位置做，就應該做」。這是「Innovator's Dilemma 焦慮」的反向操作——主動破壞自己的商業模式。
**結果**：NVIDIA 估值從 $12B 跌到 $2-3B。市場「沉默」了 10 年。直到 2012 AlexNet。
**證據**：https://www.thecloser.fm/the-nvidia-doctrine/ ; https://every.to/napkin-math/why-is-jensen-huang-120-billion-richer-than-you

---

### 5. 2012/09 AlexNet → 2013 全公司 "All-in" 深度學習
**背景**：2012 年 ImageNet 比賽，AlexNet 用兩塊 GeForce GTX 580 + CUDA 訓練，碾壓所有傳統演算法。
**關鍵動作**（不是立刻 pivot，而是 2013 早期才轉向）：
- 早期內部倡議者 Bryan Catanzaro 把 cuDNN 原型直接送到 Jensen 桌上（繞過軟體部門的阻力）
- Jensen 清空一個週末研讀 deep learning，回來時白板上寫了一句：**OIALO – Once In A Lifetime Opportunity**
- Bill Dally（Chief Scientist，2009 從 Stanford CS 主任轉投）啟動與 Andrew Ng（Baidu/Stanford）的合作專案
- 2013 內部全公司轉向 ML，Pascal 架構開始重新設計
- 2014/09 cuDNN v1 釋出（productize Catanzaro 的原型）
- 2015/03 GTC 上 Jensen 公開 all-in：發表 Titan X、DIGITS 軟體、DIGITS DevBox、Drive PX
- 2016/04 Pascal P100 出貨，宣布 NVIDIA 為此投入 $3B
**邏輯**（他自己的話）：「當我們看到 AlexNet，我們有 first principles 的清醒去問——是什麼讓它有效？如果一個 universal function approximator 能從例子學習，那幾乎所有軟體最終都會用這種方式寫」（Acquired Podcast）。
**結果**：Pascal 把 training（GP100）與 inference/gaming（GP104）SKU 分流。此後成為 Volta/Ampere/Hopper 的模板。
**證據**：https://www.acquired.fm/episodes/jensen-huang ; https://www.fastcompany.com/90957372/how-bryan-catanzaro-jumpstarted-nvidias-ai-big-bang ; https://images.nvidia.com/content/pdf/tesla/whitepaper/pascal-architecture-whitepaper.pdf

---

### 6. 2016/08/15 親手送 DGX-1 給 OpenAI — 教科書級 founder-to-founder 行銷
**背景**：OpenAI 2015/12 成立非營利。DGX-1（8× Tesla P100，~170 TFLOPS，$129K）是 NVIDIA 第一台「盒裝 AI 超級電腦」。當時 NVIDIA 是 $7B 公司，deep learning 還是 data center 的小部分。
**決策**：Jensen 親自開車送世界第一台量產 DGX-1 到 OpenAI 三藩市辦公室，並在機殼上手寫簽名：
> **"To Elon & the OpenAI Team! To the Future of Computing and Humanity. I present you the World's First DGX-1!"**
**邏輯**：「賭一個小規模 frontier research lab 會產生比 cloud hyperscaler 更強的需求拉力」。同時這是高度可拍照、可重複講故事的關係建立動作。
**結果**：OpenAI 用這台機器與後續 NVIDIA 硬體訓練出 GPT-2、GPT-3、ChatGPT。2025/09 雙方宣布「史上最大 AI 基礎設施部署」——10 GW、數千億美元規模。
**證據**：https://fortune.com/2024/02/22/jensen-huang-elon-musk-openai-first-ai-supercomputer-sam-altman/ ; https://www.tomshardware.com/tech-industry/artificial-intelligence/elon-musk-reminisces-about-the-time-jensen-huang-donated-a-dgx-1-to-openai-shares-photo-gallery

---

### 7. 2016-2017 Tesla / Drive PX 汽車押注
**決策**：CES 2016 推 Drive PX 2（雙 Tegra Parker + 雙 Pascal GPU，24 TOPS）。Tesla 2016/10 將 Autopilot HW2 全押 Drive PX 2。Volvo、Mercedes、Audi、Toyota 跟進。
**邏輯**：「自動駕駛是我們會追求的最大 computing market」——TAM 賭注，不是近期營收。
**結果**：2018-2019 Tesla 自研 HW3 取代 Drive PX 2，Musk 公開批評 GPU 是「emulation mode」。Audi 2020 Level-4 跳票。但 Mercedes 2020 選 Orin、BYD、Lucid、Polestar 跟進。Auto 一直是 NVIDIA 最小 segment（3-5% 營收）但成為 Isaac robotics 與 Drive Thor 的種子。
**證據**：https://en.wikipedia.org/wiki/Nvidia_Drive ; https://electrek.co/2016/10/20/tesla-new-autopilot-hardware-suite-camera-nvidia-tesla-vision/

---

### 8. 2019/03 收購 Mellanox（$6.9B）— 看似貴的賭注
**決策**：擊敗 Intel、Microsoft，以 $6.9B 收 Mellanox（InfiniBand、Ethernet 高速網路）。
**邏輯**：「未來 data center 是一台電腦——network 就是 computer」。Mellanox 提供 NVLink 之外的跨機架通訊能力。
**結果**：Hopper 與 Blackwell 時代，InfiniBand 是 AI 集群的標配。事後看是大撿便宜。

---

### 9. 2020/09 → 2022/02 收購 ARM 嘗試失敗
**背景**：2020/09 宣布以 $40B（$12B 現金 + $21.5B NVDA 股票 + $1.5B ARM 員工股權）收 ARM。
**決策**：Jensen 個人花 17 個月遊說全球監管機構。
**結果**：FTC 2021/12 起訴，2022/02 終止。NVIDIA 損失 $1.25B 訂金，但獲得 20 年 ARM 架構授權。
**事後反應（典型 Jensen）**：完全不公開抱怨。對 SoftBank 給出極優雅的官方聲明：「ARM 有光明的未來，我們會繼續以驕傲的 licensee 身分支持他們。」然後立刻轉向——其實早在 2021/04 就已宣布自研 Grace CPU（hedge）。
**證據**：https://nvidianews.nvidia.com/news/nvidia-and-softbank-group-announce-termination-of-nvidias-acquisition-of-arm-limited

---

### 10. 2020 COVID 期間 — 不裁員、加薪、廚房 keynote
**決策**：
- 2020/03 中內部信承諾「零裁員」+ 加速年度加薪
- 2020/05/14 GTC 從 Los Altos 自家廚房開 keynote，從烤箱裡拿出 50 磅重的 HGX A100 baseboard
- A100 / Ampere 如期出貨（7nm TSMC，54B 電晶體，~20× V100）
- DGX A100 $199K 首批送 COVID 研究機構（Argonne）
**邏輯**：「我們有足夠的雨備金做反週期投資」
**結果**：Datacenter 營收 FY2021 達 $6.7B（+124% YoY）。NVDA 2020 年漲 122.26%。
**證據**：https://blogs.nvidia.com/blog/gtc-keynote-virtual-kitchen/ ; https://nvidianews.nvidia.com/news/nvidia-announces-financial-results-for-fourth-quarter-and-fiscal-2021

---

### 11. 2022/03 Hopper H100 + Transformer Engine — 提前 3-4 年下注
**決策**：在 2019-2020 已決定 H100 加入專屬 Transformer Engine + FP8 dynamic precision——當時 transformer 還主要在 NLP 研究領域，LLM 商業化還沒影子。
**邏輯**（事後 Acquired Podcast）：「Hopper 的 T 就是 GPT 的 T——這是世界第一台為 transformer 設計的電腦。」Mar 2023 他對記者說「我們十年前就看到了」。
**結果**：H100 成為半導體史上最賺錢的單顆晶片。LLM training 9× / inference 30× 對 A100。

---

### 12. 2022 加密幣崩盤 — 重演 2018 套路
**背景**：Ethereum 轉 PoS（2022/09），GPU mining 死亡。Q2 FY23 營收差 $1.4B 預測。
**決策**：不裁員（同期 Meta/Google/Microsoft 裁數萬人）。降價、放慢出貨清庫存、減記、繼續高強度 R&D 投資（Hopper 已鎖定）。
**邏輯**：「ChatGPT 時刻」隨即到來——保住的工程團隊立刻就能交付爆量需求。
**證據**：https://fortune.com/2024/09/05/nvidia-ceo-jensen-huang-torture-employees-to-greatness-culture/

---

### 13. 2022/11 ChatGPT 後 — pivot 敘事而非產品
**決策**：產品線（H100）已經完美，pivot 的是「敘事」。從 Berkeley Haas 2023/02 開始稱 ChatGPT 為「the iPhone moment of AI」，然後 GTC 2023/03、2023/05 財報會上 guide $11B vs Street 預測 $7B——一通電話讓股價翻倍。
**結果**：Data center 營收從 Q4 FY23 ~$3.6B/季 暴衝到 Q4 FY24 >$18B/季。

---

### 14. 2023 AI Factory 重新框架
**決策**：把公司從「晶片廠」重新定義為「AI factory」供應商——推 DGX H100 / HGX / DGX SuperPOD / DGX Cloud bundle。
**結果**：每「單位」ASP 從 $10K（GPU）→ $30K（H100）→ $3M+（NVL72 Blackwell rack）。

---

### 15. 2022-2025 中國出口管制 — 「合規但極限化」
**決策**：每次出口管制收緊，立刻設計專為 China market 設計的「擦邊球」版本——A800、H800、H20，每代都剛好低於最新門檻。
**2025/04 H20 事件**：BIS 禁止 H20 出口中國，NVIDIA 提列 $5.5B 減損。Jensen 1) 飛 Mar-a-Lago 出席 $1M/人晚宴 2) 宣布 $500B 在美建 AI server 廠 3) 個人遊說 3 個月。2025/07 川普政府逆轉，准許出口 H20，但 US 政府抽 15% 營收。
**邏輯**：表面「完全合規」；行為上是「最大化出口的同時對華府施壓」。
**結果**：中國市場部分保住，但長期受限。
**證據**：https://www.npr.org/2025/08/11/nx-s1-5498689/trump-nvidia-h20-chip-sales-china ; https://time.com/7309264/nvidia-trump-china-chips-deal-h20-blackwell-national-security-concerns/

---

### 16. 2024 Blackwell 良率延遲 — 公開承擔責任
**背景**：2024/03 GTC 發表 Blackwell，2024/08 The Information 揭發 CoWoS-L 封裝設計缺陷導致良率低，延遲 3 個月。
**決策**：先短暫迴避，隨後在 10 月記者會上完全公開認錯：
> "We encountered a design flaw in Blackwell. While it was functional, this flaw led to low yield rates, and it was **entirely Nvidia's responsibility… 100% Nvidia's fault**."
明確護 TSMC：「TSMC 幫我們解決良率問題」。稱 NVIDIA-TSMC 關係緊張的傳聞是「fake news」。
**結果**：Q4 CY24 順利出貨「數十億美元」Blackwell。
**證據**：https://www.techradar.com/pro/100-percent-nvidias-fault-jensen-huang-admits-blackwell-ai-chips-had-a-concerning-design-flaw

---

### 17. 2023-2026 投資生態 — 用資產負債表鎖客
**規模**：累積 $53B 跨 ~170 個 AI 投資案。從 2022 年 12 個 → 2024 年 54 個 → 2025 年 67 個。被稱為「AI 界的 Federal Reserve」。
**代表性投資**：
- CoreWeave（2023/04 投 + 後 $2B 追投）
- Lambda（$480M Series D，$2.5B 估值）
- Mistral（2024/06 $640M B 輪 + 2025/09 €1.7B）
- Figure AI（2024/02 B 輪 + 2024 C 輪，$39B 估值）
- Wayve（2024/05 $1.05B）
- OpenAI（2025/09 $100B infrastructure 協議）
- Run:ai（$700M 收購 → 開源化軟體解除反壟斷顧慮）
- Groq（2025/12 $20B 資產收購 → 2026 推出 Groq 3 LPU）
**邏輯**：「每 $1 投資 AI startup 最終回流為 $2-4 的 GPU 訂單」。

---

### 18. 2024-2026 Physical AI / Robotics 押注
**決策**：
- 2025/01 CES 推出 Cosmos world-foundation models（20M 小時真實世界資料訓練）
- 2025/03 GTC 推出 Isaac GR00T N1（首個開源 humanoid robot foundation model）
- 投資 Figure AI、Wayve 等公司
**邏輯**（重複用 iPhone 模板）：「The ChatGPT moment for robotics is coming」——他在 2023 用「iPhone moment」框架 AI，2026 再用同樣框架 robotics。
**結果**：1.2M+ 機器人開發者註冊 Isaac SDK。

---

### 19. 2024-2026 Sovereign AI 個人外交
**決策**：親自飛各國首都做主權 AI 交易。2025/11 沙烏地 200K-GPU 協議。2025/01 法國、德國、印度、日本、新加坡。2024/06 倫敦 Tech Week 稱 UK 是「世界上最大的 AI 生態，但沒有自己的基礎設施」——一句精心設計的「捧殺」銷售話術。
**邏輯**：sovereign AI 交易需要 head-of-state 等級的認可——只有 Jensen 能成交。
**結果**：sovereign AI 2025 年帶來 ~$20B 營收（2024 的 2 倍），跨 20+ 個國家。

---

### 20. 2025/03 → 2026/03 GTC 路線圖 — Blackwell Ultra / Vera Rubin
**決策**：
- 2025 GTC：宣布 Blackwell Ultra + Vera Rubin 路線圖（年度升級節奏，而非業界傳統 2 年）
- 2026/03 GTC：宣布 $1T Blackwell + Vera Rubin 訂單到 2027（從 2024 預期的 $500B 翻倍）
- Vera Rubin：1.3M 零件、效能/瓦特是 Grace Blackwell 的 10×
- 收購 Groq → 2026 推 Groq 3 LPU
**邏輯**：年度節奏迫使 hyperscaler 不斷升級才能保持競爭力——形成「升級稅」。
**證據**：https://www.cnbc.com/2026/03/16/nvidia-gtc-2026-ceo-jensen-huang-keynote-blackwell-vera-rubin.html ; https://siliconangle.com/2026/06/01/five-thoughts-nvidia-ceo-jensen-huangs-gtc-taipei-2026-keynote/

---

## 個人決策

### 1. 1973 — 9 歲被送到美國肯塔基州 Oneida 男子學校
**背景**：父母為了讓孩子有更好教育，送他與哥哥到美國親戚家——但實際上親戚家附近只有 Oneida 男子學校（一所收容問題青少年的教會學校）。
**經歷**：被分配清廁所、做雜役。每個室友手臂都有刀疤。
**他事後解釋**：「這段經歷塑造了我對 hard work、對受苦的態度——這是我為什麼能告訴 Stanford 學生『I wish you ample doses of pain and suffering』」（NTU、Stanford GSB 多次提及）。

### 2. 大學選 Oregon State 而非藤校
**邏輯**：Oregon State 接受他這個剛搬到美國的孩子。他在那裡認識了未來妻子 Lori Mills。

### 3. 1993 — 30 歲離開 LSI Logic 創業
**背景**：在 LSI Logic 已是高階主管，財務穩定，妻小都在。
**邏輯**：「30 歲是創業的 sweet spot——還有體力，已經有經驗」。

### 4. 至今仍親自主持周會、寫全員 email
**行為**：33 年來不間斷。每週五早上 6 點全員會議。他不寫紙本 strategy plan，但寫無數 email。
**邏輯**：「資訊應該平面化分發。私下會議是剝奪其他人的學習機會。」

---

## 結構性「沒做」的決策（反向證據）

### 1. 永遠不自建 fab — 一直 fabless
- 1997 親自寫信給 Morris Chang 建立 TSMC 合作。
- 即使峰值現金時也從未自建/收購 fab。
- 公開反覆說：「沒有 TSMC 就沒有 NVIDIA」。
**邏輯**：將供應鏈關係視為**核心資產而非可榨取的對象**——這與多數美式 CEO 的「上游往下打」哲學完全相反。

### 2. 永遠不做消費硬體
- Tegra 嘗試手機晶片，2014 退出
- 沒做過 phone、PC、console（只當 Sony/Microsoft 的供應商）
- 守住「silicon + CUDA 軟體護城河」

### 3. 經濟下行絕不砍 R&D
- 2018 加密崩盤、2022 加密再崩、2020 COVID——R&D 持續成長
- R&D 占營收一直在 20-30%（大型半導體公司高端）

### 4. 不寫長期戰略計畫
> "We don't have a long-term plan. Our definition of a long-term plan is: what are we doing today?"
- 沒有年度策略會議的繁文縟節
- 沒有 Plan B：「Plan B 會稀釋 Plan A」

### 5. 不裁員（即使最痛苦時）
- 2022 加密崩盤、2018 加密崩盤、2008 金融危機——都沒大裁
- 哲學：「I'd rather torture you into greatness because I believe in you」
- FY2025 整體流失率僅 2.5%，1/5 員工司齡 ≥10 年

### 6. 個人薪酬從不取 $1
- Base salary 自 2015 起 10 年凍結在 $996,514
- 不像 Jobs/Zuckerberg/Musk 那樣象徵性 $1
- 財富 100% 來自 ~3.5% 創辦人持股——天然 owner alignment

---

## 重複出現的決策模式（這是寶藏，直接餵 Phase 2）

### 模式 A：**逆共識 zero-billion 下注**
- 1993 創業：當時沒人看好獨立顯卡
- 2006-2007 CUDA：市場「沉默」10 年
- 2019 Mellanox：當時看似貴
- 2020 Arm 嘗試：監管風險高
- 2019-2020 Hopper Transformer Engine：當時 LLM 還沒爆
- 2025 Cosmos / GR00T：robotics 商業化還沒到
**特徵**：在沒人理解的時候賭，承受 N 年沒回報。

### 模式 B：**不裁員 + 反週期投資**
- 2018 加密崩盤：繼續招 AI 工程師
- 2020 COVID：零裁員 + 加速加薪 + R&D 加碼
- 2022 加密再崩：保留 Hopper 團隊
**邏輯**：保留人才比節省成本重要——下個 wave 來時就贏。

### 模式 C：**親自做高 signal 的關係建立**
- 1997 親自寫信給 Morris Chang
- 2016 親手送 DGX-1 給 OpenAI、簽名留念
- 2025 親飛沙烏地、印度、日本見元首
- 每場 GTC 主 keynote 都是他親自 5+ 小時
**邏輯**：高層級關係只能 CEO 自己做。

### 模式 D：**公開承擔失敗，立刻 pivot**
- 1995 NV1 失敗：立刻認錯轉 Riva 128
- 2022 ARM 嘗試失敗：優雅退出 + 早已準備 Grace CPU hedge
- 2024 Blackwell 良率：完全公開「100% 是 NVIDIA 的錯」+ 護 TSMC
**邏輯**：認錯越快、團隊越敢承擔風險；護住關鍵盟友。

### 模式 E：**重複使用「iPhone moment」敘事模板**
- 2023 AI = iPhone moment
- 2026 Robotics = ChatGPT moment for robotics
**邏輯**：找一個已被市場理解的類比，把新東西放進熟悉的盒子。

### 模式 F：**用資產負債表鎖客 + 開源化解反壟斷**
- 投資 $53B 進 170 個 AI startup → 都成為 GPU 訂單
- 收 Run:ai 後立刻開源化軟體
- CUDA 不開源但 cuDNN 部分開源、PyTorch 整合
**邏輯**：硬體護城河 + 軟體擴散 = 雙重鎖定但避開反壟斷。

### 模式 G：**第一性原理重構問題**
- AlexNet 後問：「universal function approximator 為何有效？」→ 推導出 deep learning 是新軟體寫作模型
- AI factory 框架：把 data center 從「儲存倉」重新定義為「智慧製造工廠」
**邏輯**：不接受行業現有定義，回到物理/數學/客戶需求的根本。

---

## 失敗 / 認錯案例

| 失敗 | 年份 | 他的處理方式 |
|------|------|-------------|
| NV1 quadratic texture | 1995 | 立刻認錯，轉 Riva 128 |
| Bumpgate（焊接故障） | 2008 | 對 OEM 設賠償基金 |
| Mobile / Tegra phone | 2014 | 安靜退出 |
| ARM 收購失敗 | 2022 | 優雅退出 + 早已 hedge |
| Tesla 流失到自研晶片 | 2018-2019 | 不公開抱怨，繼續推 Drive 路線圖 |
| Blackwell 良率延遲 | 2024 | 100% 公開認錯 |

---

## 言行（不）一致觀察

| 他說 | 他做 | 評論 |
|------|------|------|
| 「mission is the boss」 | 60 直屬下屬集中決策 | 部分一致——使命引導大方向，但細節高度親自掌控 |
| 「strategy is execution，不寫長期計畫」 | Hopper / Blackwell / Rubin 路線圖鎖 3 年 | 矛盾——產品路線圖是長期計畫的另一種形式 |
| 「我們完全合規」（出口管制） | 連續設計擦邊球 China-specific 晶片 | 嚴格說是合規但顯然在試探極限 |
| 「公開回饋是學習機會」 | 公開斥責導致經理離職案例 | 部分員工視為文化問題 |

---

## Agent 5 摘要

行為證據覆蓋 1993-2026 共 33 年，含 20 個公司級重大決策、4 個個人決策、6 個結構性「沒做」、7 個重複決策模式、6 個失敗認錯案例。**最重要的發現**：黃仁勳的決策模式高度一致——逆共識下注 + 不砍 R&D + 公開承擔失敗 + 第一性原理。**最大反差**：他常說「mission is the boss」但實際上是極端中央集權（60 直屬）；說「沒有長期計畫」但有 3 年產品路線圖。這些張力是 Phase 2 提煉「內在矛盾」的素材。
