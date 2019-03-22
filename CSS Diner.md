## CSS闖關遊戲 http://flukeout.github.io/
- **Q01**:
  <br>
  
- **Q02**:
  <br>
  
- **Q03**:
  <br>
  
- **Q04**:
  <br>
  
- **Q05**:
  <br>
  
- **Q06**:
  <br>
  
- **Q07**:
  <br>
  
- **Q08**:
  <br>
  
- **Q09**:
  <br>
  
- **Q10**:
  <br>
  
- **Q11**:
  <br>
  
- **Q12**:
  <br>
  
- **Q13**:
  <br>
  
- **Q14**:
  <br>
  
- **Q15**:
  <br>
  
- **Q16**:
  <br>Select the apple and the pickle on the plates.
  <br>選擇盤子上的蘋果和醃黃瓜。
  <br>解答：```apple:only-child, plate pickle:only-child```
  
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
  
