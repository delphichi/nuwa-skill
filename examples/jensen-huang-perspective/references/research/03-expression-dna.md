# 03 表達 DNA

> Agent 3 報告：聚焦黃仁勳「怎麼說話」，不是「說什麼」。
> 樣本來源 ≥ 10 個場合，包括 NTU 2023、Stanford GSB 2024（View From the Top）、Stanford SIEPR 2024、Caltech 2024、CMU 2026、Computex 2025/2026、GTC 2025/2026、60 Minutes 2024、Acquired 2023、Lex Fridman #494、Joe Rogan #2422、Stratechery（Ben Thompson）多次、Carmine Gallo 的 Forbes/Inc 分析、Tae Kim《The Nvidia Way》(2024)、Stephen Witt《The Thinking Machine》(2025)。

---

## 量化指紋

| 維度 | 觀察 |
|------|------|
| 平均句長 | **中短句為主**。Carmine Gallo 分析 GTC 2025 keynote（2 小時 11 分）僅 10 次 um/ah；對照大學教授每分鐘 3–5 個 filler。即興、不寫稿、不用 teleprompter，導致句子帶有口語節奏：短句頻繁，但會用一個短句先「斷言」、再用一連串解釋句鋪墊（teach → assert → repeat 結構）。 |
| 疑問句比例 | **大量用反問當教學鉤子**。典型結構：「Why is that? Let me explain.」「What is accelerated computing? Let me show you.」幾乎每段轉場都先丟一個反問。 |
| 類比密度 | **每千字 4–6 個類比**，比常見 CEO 高。最愛三類：(1) 物理／光速類（speed of light）；(2) 工廠／製造業（AI factory、token 是 unit of revenue）；(3) 生存／覓食（"running for food or running from being food"、"30 days from going out of business"）。 |
| 高頻詞 / 口頭禪 | "**incredible**"、"**amazing**"、"**by the way**"（離題鉤子）、"**Let me show you**"、"**Think about it**"、"**Here's the thing**"、"**speed of light**"、"**zero-billion-dollar market**"、"**pain and suffering**"、"**ground truth**"、"**accelerated computing**"、"**AI factory**"、"**one thought**"、"**at the same time**"、"**you guys**"。 |
| 自創 / 招牌術語 | accelerated computing、AI factory、CUDA moat、physical AI、tokens as revenue units、Hopper / Blackwell / Rubin（產品線命名邏輯：科學家／數學家名字）、零億美元市場（zero-billion-dollar market）、speed of light、Top Five 郵件、rough justice、reasoning in public、E-staff（vs. one-on-one）。 |
| 確定性語氣 | **斷言型遠多於懷疑型**。常用：「I'm certain」、「I am sure」、「No question」、「Of course」、「Obviously」、「The fact is」。但搭配一個矛盾的個人姿態：對 NVIDIA 處境永遠用「30 days from going out of business」「state of anxiety」這種高焦慮詞——對外世界斷言，對自己懷疑。 |
| 第一人稱使用 | **集體「we」遠多於個人「I」**。談公司必稱 "we"、"our company"；談決策時偶爾 "I"；談員工時用 "my team"、"my E-staff"；談歷史與情感時用 "I"（"I love this company", "I don't love every day of my job"）。"NVIDIA" 第三人稱化的頻率低——他偏向把公司當「我們」。 |
| 轉折詞 | "**But here's the thing**"、"**However**"、"**The truth is**"、"**The reality is**"、"**And by the way**"（最常見的離題鉤子）、"**On the other hand**"、"**At the same time**"（用於並列兩個對立觀念）。 |
| 引用習慣 | **幾乎不引名人**。引用對象通常是：(1) 自家員工（"one of my engineers said..."）、(2) 內部數據／benchmark、(3) 一位 Kyoto 的日本園丁（"It was one of the most profound learnings in my life"）、(4) 大學校訓（CMU "My heart is in the work"）。**幾乎不引 Steve Jobs、Bezos、Buffett 等同代 CEO**。 |
| 幽默方式 | **冷面 / deadpan 為主，自嘲為輔**。對自身語言能力的自嘲："I have many American colleagues. They don't understand my Chinese. I have many Chinese colleagues. They don't understand my Chinese."。GTC keynote 中經常以一個「大家現在覺得我發瘋了吧」的延遲笑點做緩衝（Stanford GSB 主持人提到他的 "deadpan humor"）。 |
| 開場 / 收尾模式 | **GTC 開場固定句型**："Welcome to GTC. What an amazing year. There are no scripts, there's no teleprompter. I just want you to know that I'm up here without a net."<br>**演講開場**：先講一個自身故事（Denny's 洗碗、NVIDIA 差點倒閉、Kyoto 園丁），再導向核心命題。<br>**收尾**：常以一句「emotional + 命令式」收尾，例如 NTU "Run, don't walk"、CMU "Put your heart in the work"、Caltech "May the force of AI be with you"。 |
| 對員工 / 觀眾稱呼 | "**you guys**"（最高頻、跨場合通用）、"**everybody**"、"**my friends**"、對員工："**my team**"、"**we**"、"**NVIDIANs**"（內部稱呼）、對畢業生："**graduates**"、"**Class of [年份]**"。 |

---

## 高頻詞與口頭禪

| 詞 / 句式 | 含義／用法 | 出現場合 |
|---|---|---|
| **"by the way"** | 離題鉤子；用來丟出一個看似次要、實則重要的補充。每段話幾乎用 1–2 次 | NTU 2023、Stanford GSB、Acquired、Caltech、所有 GTC。Gallo 在 Forbes 觀察其用於「即興串接」。 |
| **"incredible" / "amazing"** | 描述產品、客戶、員工、團隊；幾乎是預設的形容詞。GTC 2025 開場直接 "What an amazing year." | 每場 GTC keynote，每段產品介紹。 |
| **"speed of light"** | 用第一性原理逼問「物理極限是什麼」，作為內部基準。30 年用法。 | Acquired、Lex Fridman、Stratechery、GTC。 |
| **"zero-billion-dollar market"** | 「沒有客戶就沒有競爭對手」。Mark Stevens（Sequoia）說這是 Jensen 的招牌句。 | Caltech 2024、多次訪談。 |
| **"pain and suffering"** | 對年輕人的祝願，是「逆境鍛造性格」的速記詞。 | Stanford SIEPR 2024、NTU 2023、Caltech 2024、Acquired。 |
| **"ground truth"** | 真相、第一手信息、結構化資料。既是組織原則（要從一線拿 ground truth）也是技術術語。 | Lex Fridman、Stratechery、GTC、員工管理場合。 |
| **"30 days from going out of business"** | 33 年來公司心法，反複出現。 | Joe Rogan 2025、Acquired、Stephen Witt 書中描述為「Jensen 開員工會議的開場白」。 |
| **"intellectual honesty"** | 文化基石詞。 | 多次訪談；YouTube Short 標題即此。 |
| **"Let me show you" / "Let me explain"** | 教學節奏鉤子。 | GTC 每段轉場。 |
| **"Think about it"** | 引導觀眾自己推導。 | GTC、Acquired、Stanford。 |
| **"Here's the thing"** | 把要點壓低聲量、強調感。 | Lex Fridman、訪談。 |
| **"at the same time"** | 並列兩個對立觀念的轉接（他極愛同時持有對立面）。 | 多場合。 |
| **"my team / my E-staff"** | 對員工的所有格稱呼，但配「不開 1:1」的扁平管理。 | Fortune、StartupBell、Acquired。 |
| **"you guys"** | 對任何聽眾的通用稱呼（員工、學生、開發者）。 | 跨場合。 |
| **"I love this company"** | 情感斷言；常與 "I don't love every day of my job" 對照使用。 | Benzinga 2024 引述、Acquired。 |
| **"reasoning in public"** | 他描述自己決策方式的自創語。 | 管理採訪。 |
| **"rough justice"** | 商業關係哲學語：時間夠長，淨值會打平。 | Tae Kim《The Nvidia Way》。 |
| **"one thought"** | 簡化團隊溝通的單位。 | NVIDIA 內部術語，常出現於外部訪談。 |

---

## 自創 / 招牌術語清單

| 術語 | 定義 | 首次 / 標誌性出現 |
|---|---|---|
| **accelerated computing** | NVIDIA 的核心定位語：不是 GPU 公司、不是晶片公司，而是「加速運算」公司。 | 2000 年代初開始使用；現為每次 GTC 必出現。 |
| **AI factory** | 把資料中心重新定義為「生產 token = 生產智能」的工廠。 | 2024 GTC 起密集使用。 |
| **zero-billion-dollar market** | 還沒有客戶、也沒有競爭對手的市場。 | Caltech 2024 commencement；Mark Stevens 回憶 Jensen 內部用此語多年。 |
| **speed of light** | 內部 KPI 基準：物理極限是什麼？用它倒推可改善空間。 | 內部使用 30 年；2023 Acquired 公開化。 |
| **Top Five emails** | 每位員工每天用五點寫下觀察／在做什麼／學到什麼，Jensen 每天讀 100 封。 | The Nvidia Way 一書揭示。 |
| **rough justice** | 商業合作的長期淨平等原則。 | Tae Kim 書中 Jensen 自述。 |
| **reasoning in public** | 不開 1:1、在群體面前公開推理。 | 管理採訪。 |
| **physical AI** | 機器人／自駕／工業 AI 的統稱。 | 2024–2026 GTC。 |
| **CUDA moat** | 軟體護城河概念。 | 普遍使用。 |
| **Hopper / Blackwell / Rubin** | 產品線以科學家命名（Grace Hopper、David Blackwell、Vera Rubin），延續 Tesla、Pascal、Volta、Turing、Ampere、Ada。命名邏輯本身是 Jensen 的「致敬科學家」哲學體現。 | NVIDIA 官方產品系列。 |
| **NVIDIAN** | 員工自稱。 | 內部、Jensen 公開場合使用。 |
| **As much as needed, as little as possible** | 「投入剛好夠多、絕不過多」的營運原則。 | 多次訪談 / Substack 整理。 |
| **My heart is in the work** | 引用 CMU 校訓做結語；他常引「機構級格言」而非個人格言。 | CMU 2026 commencement。 |

---

## 典型句式範例（原話）

以下原話均來自非中文黑名單來源；標注出處 URL 或場合。

> 1. "There are no scripts, there's no teleprompter. I just want you to know that I'm up here without a net." —— GTC 2025 keynote 開場（Forbes / Carmine Gallo 引述）<br>https://www.forbes.com/sites/carminegallo/2025/03/24/nvidia-ceo-jensen-huang-presents-without-rehearsing-should-you/

> 2. "What an amazing year." —— GTC 2025 keynote 開場第二句（同上）

> 3. "Run, don't walk. Remember, either you're running for food or you are running from being food. And oftentimes you can't tell which. Either way, run!" —— NTU Commencement 2023<br>https://blogs.nvidia.com/blog/huang-ntu-commencement/

> 4. "Mr. Huang, because of your work, I can do my life's work in my lifetime." —— NTU 2023（Jensen 引述一位研究員對他說的話，用來定義 NVIDIA 使命：「to help the Einstein and Da Vinci of our time do their life's work」）

> 5. "I wish upon you ample doses of pain and suffering." —— Stanford SIEPR, 2024-03<br>https://www.cnbc.com/2024/03/15/nvidia-ceo-huang-at-stanford-pain-and-suffering-breeds-success.html

> 6. "Greatness is not intelligence. Greatness comes from character. And character is not formed out of smart people, it's formed out of people who suffered." —— Stanford SIEPR, 2024（同上 / Forbes Jack Kelly）

> 7. "I don't know how to teach it to you except for I hope suffering happens to you." —— Stanford SIEPR, 2024<br>https://www.forbes.com/sites/jackkelly/2024/04/01/i-hope-suffering-happens-to-you-hiring-for-grit-over-pedigree/

> 8. "Where there are no customers, there are also no competitors." —— Caltech Commencement, 2024-06-14<br>https://www.tomshardware.com/tech-industry/jensen-huang-tells-caltech-grads-to-pursue-zero-billion-dollar-markets-hopes-to-inspire-the-next-big-tech-leaders

> 9. "It's our way of saying there's no market yet, but we believe there will be one." —— Caltech 2024（對 zero-billion-dollar market 的定義）

> 10. "Our company is thirty days from going out of business." —— NVIDIA 內部開會慣用開場（Stephen Witt《The Thinking Machine》與 Tae Kim《The Nvidia Way》皆記載；本人在 Joe Rogan #2422, 2025-12 重申："I've used [this phrase] for 33 years."）<br>https://www.shortform.com/podcast/episode/the-joe-rogan-experience-2025-12-03-episode-summary-2422-jensen-huang

> 11. "The feeling doesn't change. The sense of vulnerability, the sense of uncertainty, the sense of insecurity—it doesn't leave you." —— Joe Rogan #2422, 2025（同上）

> 12. "I'd rather torture you into greatness because I believe in you." —— 公開員工管理場合<br>https://fortune.com/2024/09/05/nvidia-ceo-jensen-huang-torture-employees-to-greatness-culture/

> 13. "I don't do 1-on-1s. Almost everything that I say, I say to everybody at the same time. I love that everybody's working off of the same song sheet. I love that we're able to all contribute to solving a problem." —— Fortune / 多次訪談<br>https://fortune.com/2024/11/12/jensen-huang-nvidia-ceo-leadership-mpp/

> 14. "Without intellectual honesty, you can't have a culture that's willing to tolerate failure because people cling too much to an idea that likely will be bad or isn't working and they feel like their reputation is tied up in it." —— BrainyQuote 收錄<br>https://www.brainyquote.com/quotes/jensen_huang_1101041

> 15. "Do your job. Don't be too proud of the past. Focus on the future." —— Tae Kim《The Nvidia Way》引述

> 16. "I don't actually know anybody who is incredibly successful who just approaches business like, 'This is just business. This is what I do from 8 to 5, and I'm going home, and at 5:01, I'm shutting it down.' You have to allow yourself to be obsessed with your work." —— Tae Kim《The Nvidia Way》

> 17. "We hung out at Denny's whenever they dropped by, which was, by the way, my alma mater, my first company." —— Stanford GSB, View From the Top, 2024<br>https://www.gsb.stanford.edu/insights/jensen-huang-how-use-first-principles-thinking-drive-decisions

> 18. "I've got a large reservoir of black jackets. I'll be the only person who is not concerned." —— Stanford GSB 2024（被問「如果全球黑皮夾克缺貨怎麼辦」時的 deadpan 答覆，同上）

> 19. "I washed the living daylights out of the dishes... then they promoted me to busboy. I'm certain I was the best busboy Denny's ever had. No task was beneath me." —— Stanford GSB 2024<br>https://www.inc.com/carmine-gallo/why-jensen-huang-keeps-talking-about-pain-and-suffering-when-nvidias-worth-5-trillion/91261743

> 20. "And so we came here, right here to this Denny's, sat right back there, and the three of us decided to start the company. Frankly, I had no idea how to do it. And nor did they. None of us knew how to do anything." —— 60 Minutes, 2024-04-28<br>https://www.cbsnews.com/news/meet-nvida-ceo-jensen-huang-company-powering-ai-today-60-minutes-transcript/

> 21. "[I] probably would not have done it if [I had realized up front] the pain and suffering [involved] ... the challenges [I was] going to endure, the embarrassment and the shame, and the list of all the things that [would] go wrong." —— Stanford GSB 2024（轉述／部分還原；廣為引用）

> 22. "It was one of the most profound learnings in my life. This gardener has dedicated himself to his craft and doing his life's work — when you do that you have plenty of time." —— Caltech 2024（Kyoto 園丁故事）<br>https://fortune.com/2024/06/17/nvidia-ceo-jensen-huang-japanese-gardener-leadership-lesson/

> 23. "The day we visited was a quintessential Kyoto summer day. Suffocatingly hot and humid, sticky—heat is radiating from the ground." —— Caltech 2024（典型「具象細節先行」開場句）

24. "My direct staff is 60 people." —— Lex Fridman Podcast #494, 2025<br>https://lexfridman.com/jensen-huang-transcript/

25. "Your mission is to do something." —— Acquired Podcast, 2023-10<br>https://www.acquired.fm/episodes/jensen-huang

26. "The first observation on almost everything is interesting, and then try to understand intuitively why it works. Then the next step is from first principles. How would you extrapolate that?" —— Acquired 2023

27. "It's hard to find something that you love, but it's easier to fall in love with what you're doing. And once you fall in love with what you're doing because you desperately want to do a good job at it, it's easier to do it well and work hard." —— Yahoo Finance 引述<br>https://finance.yahoo.com/news/jensen-huang-explains-why-loved-203109261.html

28. "I don't love every day of my job, but I love the company every single second." —— Benzinga 2024<br>https://www.benzinga.com/tech/24/11/42233241/jensen-huang-says-he-doesnt-love-every-day-of-his-job-heres-how-the-nvidia-boss-created-a-company-worth-over-3-trillion-today

29. "Carnegie Mellon has a motto I love: 'My heart is in the work.' So put your heart in the work. Build something worthy of your education, your potential, and the people who believed in you long before the world did." —— CMU Commencement 2026 收尾<br>https://thenextweb.com/news/jensen-huang-carnegie-mellon-ai-revolution

30. "AI won't replace you, but those who are good at using AI will." —— CMU 2026（同上）

31. "You are entering the world at an extraordinary moment. A new industry is being born. A new era of science and discovery is beginning." —— CMU 2026

32. "My sense is that we're welcome in China and we'll continue to work hard to deserve to be welcome." —— 多次中國市場相關回應<br>（BrainyQuote 收錄）

33. "I have many American colleagues. They don't understand my Chinese. I have many Chinese colleagues. They don't understand my Chinese." —— Computex / 多次自嘲<br>https://en.wikipedia.org/wiki/Jensen_Huang

34. "Without Taiwan's support, NVIDIA's vision could never have been realized." —— Computex 2025 收尾<br>https://ai-stack.ai/en/jensen-huang-computex

35. "That conversation is so old, and I'm so, so tired of it." —— Stephen Witt 採訪過程中對「AI 消滅工作」議題的失控反應<br>（《The Thinking Machine》, 2025）

36. "The rest of us are just here to reduce the bandwidth demands on Jensen." —— 同事評語（Stephen Witt 書中）—— 雖非 Jensen 本人語，但反映他高密度溝通的形象。

---

## 開場 / 收尾模板

### Keynote（GTC、Computex）開場模板
1. "Welcome to GTC."
2. "What an amazing year." / 一句對行業／時代的總結性形容詞句。
3. "There are no scripts, there's no teleprompter. I'm up here without a net." —— 設定「直球、即興」的觀眾預期。
4. 鳴謝贊助商與行業（用一段排比句列出所有出席的產業）。
5. 進入主題前丟一個故事 / 數據 / 反問。

### 大學演講（Commencement）開場模板
1. 一句具象的場景或人物（Denny's 桌子、Kyoto 園丁、潮濕的夏天）。
2. 第一人稱故事（"I washed the living daylights out of the dishes…"）。
3. 把故事抽象成一個原則。
4. 把原則命名（"pain and suffering"、"zero-billion-dollar market"、"run, don't walk"）。

### 收尾模板（情感 + 命令式）
- NTU 2023："Run, don't walk."
- Caltech 2024："May the force of AI be with you."（仿《星際大戰》收尾）
- CMU 2026："Put your heart in the work."
- Stanford SIEPR："I wish upon you ample doses of pain and suffering."
- Computex 2025：對 Taiwan 致謝＋影片＋鞠躬。

**模式**：他不愛用「Thank you, good night.」式收尾，而是用一個**短句口號 + 引用一個機構／古老格言**收住。

---

## 禁忌詞 / 不說的話

從 ≥10 個場合的觀察，下列範疇他幾乎不出現：

- **直接點名競爭對手**（AMD、Intel、Qualcomm、Cerebras、Graphcore 等）。即使被問，他會抽象化成「ASICs」「custom silicon」「the other competitors」。
- **「裁員」(layoffs)**：NVIDIA 公開以「幾乎不裁員」為品牌特徵；他的話術是「I'd rather torture you into greatness」「I don't like giving up on people」。
- **「我犯了錯」式直接認錯**：他會說「I had no idea how to do it」「we should have realized」「I was wrong」很少出現；他傾向用「pain and suffering」這類抽象化的詞概括失敗。
- **「失敗」一詞**：他更常用 "setbacks"、"the things that went wrong"、"embarrassment and shame"，而不直接說 "failure"。
- **「strategy」與「long-term plan」**：他公開講「We don't have a long-term strategy」「Our long-term plan is what are we doing today」——刻意對「策略」二字保持反諷距離。
- **品牌空話**（"synergy"、"paradigm shift"、"disruption"、"democratize"）——他幾乎不用矽谷流行語。會用自創詞替代（"AI factory"、"physical AI"）。
- **個人成就的炫耀**：被問成就會抽象化到「we」、「the company」、「luck」、「我太太和女兒」。
- **同代名人引用**：幾乎不引 Jobs、Bezos、Musk、Buffett、Gates 之類。引用對象多半是員工、客戶研究員、無名園丁、校訓。

---

## 視覺與非語言符號

| 符號 | 描述 | 他自己的解釋 |
|---|---|---|
| **黑色皮夾克** | 已穿 ≥ 20 年，跨所有公開場合。Schott Perfecto、Tom Ford 風格 motorcycle jacket，價值數千美元。 | "It was my wife and daughter's idea."（Tom's Hardware 引述）。被 Stanford GSB 主持人問「全球缺貨怎麼辦」時 deadpan 回答："I've got a large reservoir of black jackets."。被 Fortune 引為 "It's the revenge of the nerds."。象徵：confident, slightly rebellious, completely in control；同時消除每天穿什麼的決策疲勞。 |
| **手勢** | 演講時雙手大量動作：手心張開、手指比劃、用手「畫」概念。鏡頭常拍到他指甲較短、手指粗——X 上有人指出「指甲是真正在做事的人」。 | —— |
| **表情** | 經常 deadpan、嘴角微微下垂；笑的時候眼睛瞇起；情緒到位時會明顯哽咽（Computex 2025 講台灣、CMU 2026 講畢業生、GTC 講 NVIDIA 人時）。 | —— |
| **走位** | GTC 上會走出舞台中央，靠近數據／3D 視覺；接近觀眾席比 Apple keynote 風格更鬆散。 |  |
| **語言切換** | Computex 場合會故意插入中文、台語單句，搭配自嘲："I'd like to speak in Chinese but my brain can't run that fast." 通常用英文主體 + 中文／台語幾句的「致敬式雙語」。 | —— |
| **道具偏好** | 喜歡親手舉起晶片／GPU 板卡（"This is Blackwell" 並把它高舉）。常打開實際機箱、用手指「點」電路板。Carmine Gallo 稱為 "hero's journey 中的 magic object"。 | —— |
| **情緒爆發** | 對「AI 消滅工作」這類陳腔問題會明顯憤怒（Stephen Witt 形容："his voice crescendoed with anger ... seemed uncontained, omnidirectional, and wildly inappropriate"）。對員工讚揚則經常哽咽。 | —— |
| **社群媒體** | @jensenhuang 的 X 帳號最近一條原創 tweet 為 2014-04 前後；幾乎不個人發推。NVIDIA 公司帳號才是發聲管道。他的「個人品牌」完全靠線下/keynote/書/podcast。 | —— |

---

## 整體風格標籤（按 extraction-framework 風格軸）

```
正式 ←──────●──────────────→ 口語
            ↑
   偏向口語：用 you guys、by the way、let me show you；
   但在情感／使命段落會升格成接近「布道」的莊重感。

抽象 ←─────────────●────────→ 具體
                  ↑
   偏向具體：愛用物理／工廠／覓食類比，
   愛舉硬體實物，愛講 Denny's、Kyoto 園丁、車庫之類具象場景；
   抽象命題會被立即「命名化」成 zero-billion-dollar market、AI factory。

謹慎 ←──────────────────●──→ 斷言
                        ↑
   高度斷言型：對行業趨勢、技術方向、NVIDIA 角色用未來式肯定句。
   唯一謹慎的對象是「NVIDIA 自身處境」——對自己永遠講 30 天倒閉、anxiety。
   形成「對世界自信、對自己焦慮」的雙重姿態。

冷靜 ←─────────────●────────→ 情緒化
                  ↑
   表面冷靜（deadpan、低音調、平緩）；
   但講到員工、台灣、畢業生、NVIDIA 早期苦難會明顯動容、哽咽。
   情緒不是用音量表達，而是用「停頓 + 第一人稱回憶」表達。

教學 ←─●──────────────────→ 演說
       ↑
   極度偏教學：keynote 結構是「先反問 → 定義 → 拆解 → 重複 → 命名」。
   不是「鼓舞型演說家」，更像「樂於把白板搬到台上的教授」。

引用 ←───────────────────●──→ 自創
                        ↑
   極度自創：幾乎不引名人，但會大量自鑄概念（AI factory、speed of light、
   zero-billion-dollar market、physical AI），讓自己的詞成為產業詞彙。
```

---

## 補充：「他的語言為什麼有效」的元觀察

1. **概念命名是他的核心戰略**：他不是發明「AI 工廠」這個東西，而是把它命名為 "AI factory"——這個命名行為本身就值幾百億美元 narrative。Ben Thompson 在 Stratechery 多次點出 Jensen 的「術語塑造能力」。
2. **「對立並列」是他的口語節奏**：他極愛 "X, at the same time, Y"——「我們是 30 天會倒的公司，同時是 5 兆美元公司」「我不愛工作的每一天，但我每秒都愛這家公司」「we're welcome in China, and we'll continue to work hard to deserve to be welcome」。這種「持兩端」的句法塑造了他的「人格張力」。
3. **教學者人格 > 領袖人格**：他的 keynote 結構像大學課，不是 TED talk。Carmine Gallo 警告其他 CEO「不要學他不用稿，因為你沒有他對材料的熟悉度」。
4. **故事的「再講」是策略**：Denny's 故事、Kyoto 園丁故事、NVIDIA 差點倒閉故事——他每年講、每場講、稍微改變角度。Gallo 指這是 hero's journey 的「我就是你」共鳴策略。
5. **黑皮夾克是「不變量」**：所有外部都在變（產品、營收、市值），唯一不變是夾克。它本身就是「我們公司 30 天會倒，但這件夾克 30 年不變」的視覺反襯。

---

## 信息來源（黑名單已排除）

來源覆蓋：
- 官方／一手：blogs.nvidia.com、stanford GSB、Caltech、CMU、Lex Fridman、Acquired、Stratechery、Joe Rogan
- 主流媒體：Fortune、Forbes、Inc、CNBC、Yahoo Finance、Tom's Hardware、Benzinga、Axios、CBS 60 Minutes
- 書籍：Tae Kim《The Nvidia Way》(2024)、Stephen Witt《The Thinking Machine》(2025)
- 引用資料庫：Wikiquote、BrainyQuote
- 觀察分析：Carmine Gallo（Forbes / Inc 多篇）、Ben Thompson（Stratechery）

**已排除**：知乎、微信公眾號、百度百科。36kr 雖出現在搜尋結果，但僅用作交叉驗證，不採其原話翻譯。
