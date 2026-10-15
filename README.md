# 這次到底該發給誰？餐飲業的精準發訊決策 · 學員站

LINE 官方帳號 餐飲產業經營者小聚；講師 Angle 何佳勳（小圭）／圭話行銷。2026/10/22（四）13:30-16:30 升級會議中心松江館。單頁 HTML、GitHub Pages。

- **index.html**：組別（1 到 6 組）報到、8 分頁、7 題現場互動（6 題個人題投完顯示正解）、20 個標籤可點選收藏、三個計算機（LINE 訊息成本／目標回推發送人數／全發 vs 精準發對照）、六情境實作題、**8 欄位發訊決策卡**（可填可複製可一鍵送出）、團體題、全場投票、發訊前 5 分鐘檢核表、16 支 ecom 工具。
- **admin.html**：後台（noindex）決策卡牆（結構化顯示每組每一版）／計分（8 種加分預設）／互動題統計／投票／學員／其他交件，全部可匯出 CSV。
- **board.html**：投影用。計分榜模式 ＋ **決策卡輪播模式**（發表時一組一組投影，鍵盤左右切換、1 到 6 直接跳、A 自動播放、F 全螢幕）。

後端：共用 Supabase `lw_line_students`（course=`restaurant-line-decision`）＋ `lw_workshop_submissions`（task=card／team／extra，決策卡以 JSON 存在 content）＋ `lw_workshop_scores` ＋ `lw-workshop` bucket。
