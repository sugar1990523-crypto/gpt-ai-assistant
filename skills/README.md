# 行銷與工作流程 Skills

這套 Skill 從使用者提供的一段持續工作對話萃取，沒有讀取帳號全部歷史對話。文件是通用流程，沒有包含對話原文、內部營運數據、信箱、帳號或資源 ID。

## 候選與優先序

| 優先 | Skill | 用途 |
|---|---|---|
| 高 | [行銷串接驗證](marketing-connection-audit/SKILL.md) | marketing-connection-audit |
| 高 | [GMC 商品與政策檢查](merchant-feed-audit/SKILL.md) | merchant-feed-audit |
| 高 | [SEO 30 天優化追蹤](seo-observation-cycle/SKILL.md) | seo-observation-cycle |
| 中 | [競品價格與關鍵字比較](competitor-comparison/SKILL.md) | competitor-comparison |
| 中 | [試算表重複比對與整合](spreadsheet-reconciliation/SKILL.md) | spreadsheet-reconciliation |
| 中 | [工作進度彙報與隔日安排](work-progress-report/SKILL.md) | work-progress-report |
| 中 | [對話整理與 Skill 萃取](conversation-to-skills/SKILL.md) | conversation-to-skills |
| 中 | [日本市場 SEO 審稿交接](japanese-seo-review/SKILL.md) | japanese-seo-review |

## 使用
在支援本地 Skills 的 agent 中，將需要的資料夾放入該環境的技能搜尋路徑；確認該 agent 的說明後使用。也可要求 agent 讀取指定 SKILL.md，明確指定本次資料與目標。

建議指令：「依 merchant-feed-audit 檢查我指定試算表最新的 GMC 分頁，只讀分析。」或「依 work-progress-report 整理這次對話的進度與明日計畫。」

GitHub 是版本管理來源。這個 PR 不會自動安裝到 ChatGPT 帳號、不會設定排程，也沒有修改既有 OpenAI／LINE 應用的執行程式。每次使用仍需要有效的工具連線與資料權限。

## 擴充全部對話
請另外提供 ChatGPT 對話匯出檔或指定對話；依 conversation-to-skills 先盤點來源再增補。禁止把私有對話或原始報表提交到公開 repo。

## 驗證方式
確認每個資料夾含 SKILL.md、frontmatter 的 name 與資料夾相同、description 清楚、流程與驗收非空。執行測試使用授權資料；目前僅完成文件結構檢查，未做全工具端到端驗收。
