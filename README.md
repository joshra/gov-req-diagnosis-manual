# 政府需求診斷手冊（靜態網站）

這個 repo 內的 `政府需求診斷手冊/` 是 Markdown 手冊原文；已用 **MkDocs** 直接轉成可部署的靜態網站，並可用 **GitHub Pages** 上架。

## 本機預覽

1. 安裝 Python（建議 3.11+）
2. 在 repo 根目錄執行：

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve
```

瀏覽器打開終端機顯示的本機網址即可（預設 `http://127.0.0.1:8000/`）。

## 部署到 GitHub Pages（自動）

這個專案已包含 GitHub Actions 工作流：`.github/workflows/deploy-mkdocs.yml`

上架步驟：
- **建立 GitHub Repo**：把這個資料夾 push 上去
- **到 GitHub Repo Settings → Pages**
  - **Source** 選擇：`Deploy from a branch`
  - **Branch** 選擇：`gh-pages` / `(root)`
- 之後每次 push 到 `main`（或 `master`）都會自動更新網站

## 手冊內容位置

- 來源 Markdown：`政府需求診斷手冊/`
- MkDocs 設定：`mkdocs.yml`

