## CSS闖關遊戲 http://flukeout.github.io/
- **Q01**:
  <br>Select the plates.
  <br>選取盤子。
  <br>解答：```plate```
  
- **Q02**:
  <br>Select the bento boxes.
  <br>選擇便當盒。
  <br>解答：```bento```
  
- **Q03**:
  <br>Select the fancy plate
  <br>選取花俏的盤子。
  <br>解答：```plate#fancy```
  
- **Q04**:
  <br>Select the apple on the plate.
  <br>選擇盤子上的蘋果。
  <br>解答：```plate apple``` (因為階層關係，中間要空一格)
  
- **Q05**:
  <br>Select the pickle on the fancy plate.
  <br>選擇花俏盤子上的醃黃瓜。
  <br>解答：```plate#fancy pickle```
  
- **Q06**:
  <br>Select the small apples.
  <br>選擇小蘋果。
  <br>解答：```apple.small```
  
- **Q07**:
  <br>Select the small oranges.
  <br>選擇小橘子。
  <br>解答：```orange.small```
  
- **Q08**:
  <br>Select the small oranges in the bentos.
  <br>選擇便當裡的小橘子
  <br>解答：```bento orange.small```
  
- **Q09**:
  <br>Select all the plates and bentos.
  <br>選擇所有的盤子和便當。
  <br>解答：```plate, bento```
  
- **Q10**:
  <br>Select all the things!
  <br>選擇所有的東西。
  <br>解答：```*```
  
- **Q11**:
  <br>Select everything on a plate.
  <br>選擇盤子上的所有東西。
  <br>解答：```plate *``` (因為階層關係，中間要空一格，亦即盤子下的所有子元素)
  
- **Q12**:
  <br>Select every apple that's next to a plate
  <br>選擇盤子旁邊的每個蘋果。
  <br>解答：```plate+apple``` (選擇緊接在盤子之後的每個蘋果)
  
- **Q13**:
  <br>Select the pickles beside the bento.
  <br>選擇便當旁邊的泡菜
  <br>解答：```bento~pickle``` (選擇在便當之後的所有相鄰泡菜)
  
- **Q14**:
  <br>Select the apple directly on a plate.
  <br>選擇緊接在盤子上的蘋果。
  <br>解答：```plate > apple```(直接)
  <br>困惑答案：```plate apple```(間接) 會造成這種 [plate]:[bento]:[apple] 擺設也會被選取，我們要的是蘋果緊接著盤子
  
- **Q15**:
  <br>Select the top orange.
  <br>選擇頂端的橘子。
  <br>解答：```orange:first-child```
  <br>其他解答：```orange:nth-child(1)```
  <br>其他解答：```orange:first-of-type```
  <br>其他解答：```orange:first```
  <br>其他解答：```orange:nth-of-type(1)```
  
- **Q16**:
  <br>Select the apple and the pickle on the plates.
  <br>選擇盤子上的蘋果和醃黃瓜。
  <br>解答：```apple:only-child, plate pickle:only-child```
  <br>其他解答：```plate apple, plate pickle```
  
- **Q17**:
  <br>Select the small apple and the pickle.
  <br>選擇小蘋果和醃黃瓜。
  <br>解答：```apple:last-child, pickle:last-child```
  <br>其他解答：```apple, pickle```
  
- **Q18**:
  <br>Select the 3rd plate.
  <br>選擇第3個盤子。
  <br>解答：```:nth-child(3)```
  <br>其他解答：```:nth-last-child(2)```
  <br>其他解答：```:nth-of-type(3)```
  <br>其他解答：```:nth-last-of-type(2)```
    
- **Q19**:
  <br>Select the 1st bento.
  <br>選擇第一個便當。
  <br>解答：```bento:nth-last-child(3)```
  <br>其他解答：```bento:nth-child(2)```
  <br>其他解答：```bento:first```
  <br>其他解答：```bento:first-of-type```
  <br>其他解答：```bento:nth-of-type(1)```
  
- **Q20**:
  <br>Select first apple.
  <br>選擇第一個蘋果。
  <br>解答：```apple:first-of-type```
  <br>其他解答：```apple:first```
  <br>其他解答：```apple:nth-of-type(1)```
  <br>其他解答：```apple:nth-child(2)```
  
- **Q21**:
  <br>Select all even plates.
  <br>選擇所有偶數盤子。
  <br>解答：```:nth-of-type(even)```
  <br>其他解答：```:nth-of-type(2n)```
  <br>其他解答：```plate:nth-of-type(even)```
  <br>其他解答：```plate:nth-of-type(2n)```
  
- **Q22**:
  <br>Select every 2nd plate, starting from the 3rd.
  <br>從第 3 個開始，每兩個為一組，選擇每組的第 1 個。
  <br>解答：```plate:nth-of-type(2n+3)```
  
- **Q23**:
  <br>Select the last apple and orange.
  <br>選擇最後一個蘋果與橘子。
  <br>解答：```apple:only-of-type```
  <br>其他解答：```apple:only-child```
  
- **Q24**:
  <br>Select the last apple and orange.
  <br>選擇最後的蘋果與橘子。
  <br>解答：```apple:last-of-type, orange:last-of-type```
  <br>困惑答案：```apple:last-child, orange:last-child``` orange:last-child 會是空的，last-child 是指同一層最後的元素(apple)，而 orange 與 apple 交集是空集合
  
- **Q25**: 
  <br>Select the empty bentos.
  <br>選擇空的便當。
  <br>解答：```apple:not(.small)```
  
- **Q26**: （又稱為：反向選擇器）
  <br>Select the big apples.
  <br>選擇大蘋果。
  <br>解答：```apple:not(.small)```
  
- **Q27**:
  <br>Select the items for someone.
  <br>為某人選擇物品。
  <br>解答：```[for]```
  
- **Q28**:
  <br>Select the plates for someone.
  <br>為某人選擇盤子。
  <br>解答：```plate[for]```
  
- **Q29**:
  <br>Select Vitaly's meal.
  <br>選擇 Vitaly 膳食。
  <br>解答：```[for="Vitaly"]```
  
- **Q30**:
  <br>Select the items for names that start with 'Sa'.
  <br>選擇名子以 'Sa' 起始的物品。
  <br>解答：```[for^="Sa"]```
  <br>說明：類似 Reg-Exp 的用法```^Sa```，用 ```^=``` 來表示
  
- **Q31**:
  <br>Select the items for names that end with 'ato'.
  <br>選擇名子以 'ato' 結尾的物品。
  <br>解答：```[for$="ato"]```
  <br>說明：類似 Reg-Exp 的用法```ato$```，用 ```$=``` 來表示
  
- **Q32**:
  <br>Select the meals for names that contain 'obb'.
  <br>選擇名子包含 'obb' 的膳食。
  <br>解答：```[for*="obb"]```
  <br>說明：類似 Reg-Exp 的用法```.*obb.*```，用 ```*=``` 來表示
  
