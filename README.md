## 選擇器語法：
 - 條件(condition) (加上冒號當作過濾條件)
   - list (依據清單劃分)
     - type (依據清單類型劃分)
       - ```:first-of-type``` (尋找各類型的第一個元素)
       - ```:nth-of-type``` (尋找各類型的第 n 個元素) (nth 表示可計數)
       - ```:only-of-type``` (尋找各類型元素中，只有它自己一個)
       - ```:last-of-type``` (尋找各類型的最後一個元素)
   - ```:empty``` (尋找沒有子元素的元素)
   - ```:not(selector)``` (反向選擇器)
   
 - 屬性(attribute)
   - ```tag[attr]```
   - ```[attr]```
   - ```[attr="xxx"]```
     - 根據搜尋來劃分：
     - ```[attr^="xxx"]```
     - ```[attr*="xxx"]```
     - ```[attr$="xxx"]```


## 基礎學習資源
 - [CSS闖關遊戲](http://flukeout.github.io/)
   - Answers: [CSS Diner.md](CSS%20Diner.md)

 - [[mozilla] CSS](https://developer.mozilla.org/zh-CN/docs/Learn/CSS/Introduction_to_CSS/Simple_selectors)
