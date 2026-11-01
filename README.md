# 安墨起卦 PWA

可離線使用的梅花易數起卦 App。

## 檔案
- index.html：主程式
- manifest.webmanifest：App 名稱、圖示、全螢幕設定
- sw.js：離線快取
- icons/：App 圖示

## 上架 GitHub Pages
1. 到 github.com 註冊並登入。
2. 右上角「+」→ New repository，名稱填 anmo-qigua，選 Public，按 Create。
3. 在新倉庫頁面點「uploading an existing file」，把本資料夾所有檔案（含 icons 資料夾）拖進去，按 Commit changes。
4. 進 Settings → Pages，Source 選 Deploy from a branch，Branch 選 main、資料夾 /(root)，按 Save。
5. 約一兩分鐘後，網址為 https://你的帳號.github.io/anmo-qigua/

## 安裝到手機
- Android（Chrome）：開啟網址 → ⋮ →「安裝應用程式」或「加到主畫面」
- iPhone（Safari）：開啟網址 → 分享 →「加入主畫面」
安裝後先在有網路時開一次，之後即可離線使用。

## 更新程式
修改 index.html 後，把 sw.js 第二行的版本號加一（例如 anmo-v2 改成 anmo-v3），一起上傳覆蓋。

## AI 解卦設定
1. 打開 App 下方的「AI 解卦設定」，選 Claude、Gemini 或 ChatGPT。
2. 貼上該家的 API 金鑰，按「儲存設定」。
   - Claude：console.anthropic.com → API Keys（需儲值）
   - Gemini：aistudio.google.com/apikey（有免費額度）
   - ChatGPT：platform.openai.com/api-keys（需儲值）
3. 起卦後按「請安墨居士解卦」。
金鑰只存在自己的手機，每個人用自己的金鑰與帳單。

## 沒有金鑰也能解卦
起卦後按「複製並前往 Claude 解卦」，會複製起卦結果並打開 Claude。進入「安墨易卦」專案貼上送出即可，用的是 Claude 會員額度。
可在「AI 解卦設定」填入專案網址，按鈕就會直接打開專案。
