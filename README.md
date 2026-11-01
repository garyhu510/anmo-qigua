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

## 請安墨居士解卦
在「安墨解卦」區塊點選 Claude、Gemini 或 ChatGPT，再按「複製並前往 ○○ 解卦」。
App 會連同安墨居士指令一起複製，並打開該 AI，在新對話貼上送出即可，用的是自己原本的帳號或訂閱。
若在該 AI 建好了安墨的專案（Claude）、Gem（Gemini）或 GPT（ChatGPT），可在「解卦設定」填入網址，之後只複製起卦結果並直接打開它。
「複製安墨居士指令」按鈕可複製角色指令，貼到 Gem、GPT 或專案的指示欄位。
