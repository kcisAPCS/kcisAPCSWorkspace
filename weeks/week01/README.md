# Week 01：C++ 基本輸入與輸出

本週練習編譯與執行、文字輸出、換行與空格，再使用 `std::cin` 讀取整數。圖案題可直接寫輸出敘述，本週不需要使用迴圈。

## 上課流程

1. 在 VS Code 開啟自己的教材 repo，執行 [hello.cpp](notes/hello.cpp) 確認能編譯。
2. 依下方說明觀察文字、換行與空格，再練習讀取整數。
3. 選擇基礎或進階題目，修改後重新編譯、執行並核對輸出。

## 今天的內容

### 文字與換行

閱讀 [output-order.cpp](notes/output-order.cpp)，先預測四行輸出，再執行核對。交換第二個與第三個輸出敘述，觀察順序的變化。

`std::cout << "Hello\n";` 會輸出文字並換行。`\n` 是換行字元；引號內的半形空格也會原樣輸出。再修改 [hello.cpp](notes/hello.cpp) 的文字，儲存、編譯並執行。

### 空格與圖案

`std::cout << "  *\n";` 會先輸出兩個空格，再輸出星號。空格數量會影響圖案的位置；不要用 Tab 代替題目指定的空格。

第一週可以直接為每行圖案寫一個輸出敘述，不必使用迴圈。

### 讀取整數

開啟 [input.cpp](notes/input.cpp)，編譯執行後輸入 `12 34` 並按 Enter。

- `int first = 0;` 宣告整數變數並給予初始值。
- `std::cin >> first >> second;` 依序讀取兩個整數。空格與換行都可以分隔它們。
- `std::cout << "First: " << first << '\n';` 依序輸出標籤、變數的值與換行。

程式等待輸入時沒有立刻顯示結果是正常的。Judge 會提供輸入，不要額外印出「請輸入」等提示文字。

## 題目

基礎題放在 `problems/basic/`，進階題放在 `problems/advanced/`。06 製作文字選單是進階自由練習，沒有標準輸出。

| 題目 | 難度 | 練習重點 |
| --- | --- | --- |
| [01 修正字串輸出](problems/basic/01-fixStringOutput/README.md) | 基礎 | 編譯錯誤與字串 |
| [02 輸出課程資訊](problems/basic/02-printCourseInfo/README.md) | 基礎 | 文字與換行 |
| [03 輸出星號三角形](problems/basic/03-printStarTriangle/README.md) | 基礎 | 星號圖案 |
| [04 讀取並輸出整數](problems/basic/04-readAndPrintInteger/README.md) | 基礎 | 讀取整數與格式化輸出 |
| [05 靠右對齊三角形](problems/advanced/05-rightAlignedTriangle/README.md) | 進階 | 行首空格與對齊 |
| [06 製作文字選單](problems/advanced/06-createTextMenu/README.md) | 進階 | 自訂文字排版 |
| [07 空心矩形](problems/advanced/07-hollowRectangle/README.md) | 進階 | 行內空格 |

依進度選題，不要求全部完成。每題先讀 README.md，再修改 main.cpp。自由練習沒有標準輸出，不使用 Judge；其他題目可在網站依週次與題名選取。

## 編譯與測試

在 VS Code 開啟要執行的 .cpp，儲存後使用課堂設定的編譯功能，再從終端機執行產生的程式。修改後要重新編譯；程式需要輸入時，依題目範例輸入資料。

有標準輸出的題目可到 Judge 網站選擇週次與題名，選取最新的 main.cpp 檢測。自由練習只在本機確認效果。

## 下課前

儲存程式，在 VS Code 的 Source Control 確認修改、建立 Commit，再 Push 到自己的 GitHub repo。教室電腦會還原，關機前請確認遠端已更新；Push 失敗時先請老師協助或另存備份。
