# Angular-boilerplate 說明


當前專案的結構是最基本的模板，可依專案需求自行進行調整，以下內容請依照每個專案內容去調整，並詳細說明以下內容：<br>
1. [專案說明](#一專案說明)
2. [專案環境和套件](#二專案環境和套件)
3. [專案啟動](#三專案啟動)
4. [專案資料夾結構](#四專案資料夾結構)


## 一、專案說明
這是一個基於` Angular 16` 框架的模板專案，是以模組(module)架構而非standalone。<br>

<br>
以下將指導你如何安裝必要的套件、理解本專案的基本架構以及如何啟動和執行專案。

## 二、專案環境和套件

### 環境設置
|檔案|版本|
|----|----|
|[Node.js](https://nodejs.org/zh-tw/download)|^16.14.0 或 ^18.10.0|
| [git](https://git-scm.com/downloads) | 不限 |
| [Angular cli](https://angular.io/cli) | 16版 |

### 套件
目前暫時無安裝其他第三方套件
## 三、專案啟動

1. 安裝vscode推薦的工作應用<br>
首先點擊左側功能列的`Extensions`， 在最上方的查詢列輸入`@recommended`，就會出現推薦的應用程式，請安裝推薦的所有應用程式。

1. 輸入以下指令，進行套件安裝
```bash
npm install 
```
3. 待安裝完套件後輸入以下指令來啟動專案
```bash
ng serve 
```

## 四、專案資料夾結構
```
🔸 表示當前專案沒有該檔案，在此列出是為了顯示結構，可以依照需求自行新增。

- 📂 angular-boilerplate
  - 📂 .vscode (vscode設定)
  - 📂 e2e
  - 📂 node_modules (引用套件)
  - 📂 src
      - 📂 app
          - 📂 core（共用工具模組)
               - 📂 enums (列舉宣告)
                   - 📄 common.enum.ts
               - 📂 guards (路由守衛)
               - 📂 utils （輔助工具）
                   - 📄 common-utils.ts
               - 📂 consts (常數宣告)
                   - 📄 common.consts.ts
               - 📂 models (通用資料模型)
                   - 📄 a.model.ts 🔸
                   - 📄 b.model.ts 🔸
               - 📂 services (通用服務: 如Storage)
               - 📂 validators (驗證器) 🔸

               - 📂 interceptors
          - 📂 features（各功能模組）
               - 📂 feature-a 🔸
                    - 📄 feature-a.component.html
                    - 📄 feature-a.component.scss
                    - 📄 feature-a.component.ts
                    - 📄 feature-a.component.spec.ts
                    - 📂 models(該功能會使用到的資料模型）
          - 📂 shared (共用元件)
               - 📂 components（共用元件，例:dialog、toast）
               - 📂 pipes 
               - 📂 directives 
               - 📂 layout (畫面框架元件，例：header、navbar等)
          - 📄 app.component.html
          - 📄 app.component.scss
          - 📄 app.component.ts
          - 📄 app.module.ts 
          - 📄 app.routing-module.ts
     - 📂 assets(靜態資源)
         - 📂 images (圖片)
         - 📂 data (API假資料) 🔸
         - 📂 scripts (外部js) 🔸
         - 📂 icons 🔸
     - 📂 styles(樣式檔案）
          - 📄 _custom.scss 🔸（外部套件樣式）
          - 📄 styles.scss 
     - 📂 environments(環境變數)
          - 📄 environment.ts
          - 📄 environment.prod.ts
     - 📄 index.html
     - 📄 main.ts
     - 📄 polyfills.ts
  - 📄 .eslintrc.json
  - 📄 .gitignore
  - 📄 angular.json
  - 📄 package.json
  - 📄 tsconfig.json
  - 📄 README.md
