HTML方面：

1. 首先寫一個dropdown的div，裡面包含一個text型態的input和一個list的div。
2. 在list的div裡面，按照題目指示將本來的三個Option各自搭配一個checkbox型態的input，再用form包起來。最後增加一個button。

JavaScript方面：

A. 定義
1. 利用querySelector方法，以class值鎖定list，並定義它為list。
2. 為了鎖定text型態的input，回頭到HTML替他設一個id，值為choices。接著利用getElementById方法鎖定並定義它為input。
3. 為了鎖定button，回頭到HTML替他設一個id，值為ok-button。接著利用getElementById方法鎖定並定義它為okButton。

B. 顯示選單
1. 鎖定list，用addEventListener方法，當使用者點擊，啟動涵式。
2. 這個涵式鎖定list的css程式碼裡面的display值，並改定為"block"，顯示選單。（原來list的css程式碼裡面的display值為"none"）　

C. 點擊按鈕
1. 鎖定okButton，用addEventListener方法，當使用者點擊，啟動涵式。
2. 涵式內定義selectedOptions為一個空的陣列。
3. 涵式內用querySelector方法，以鎖定class值鎖定list，再鎖定list裡面的input，將它們定義為checkboxes。
4. 用forEach方法分別檢查checkbox型態的input，如果checked，把該input的值用push方法加到selectedOptions陣列
5. 重新定義text型態的input的值為selectedOptions陣列，並用join方法，以逗號分開陣列當中的值。
6. 最後，鎖定list的css程式碼裡面的display值，並改定為"none"，不顯示選單。

