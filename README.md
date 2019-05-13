## 選擇器語法：
 - 兄弟節點
   - ```+``` 運算子（前後可以有多個空格）
     <br>```A + B``` 表示 A 為前兄弟節點，B 為 A 的後兄弟節點，且是直接緊鄰 A
   
   - ```~``` 運算子（前後可以有多個空格）
     <br>```A - B``` 表示 A 為前兄弟節點，B 為 A 的後兄弟節點，可以直接或間接緊鄰 A

 - 子節點
   - ```*``` 運算子（前後可以有多個空格）
     <br>```A *``` 表示 A 為父節點，* 表示父節點 A 底下的所有(緊鄰/直接)子節點
     
   - ```>``` 運算子（前後可以有多個空格）
     <br>```A > B``` 表示 A 為父節點，B 為 A 的子節點，且是直接緊鄰 A
     <br>```<A><span><B>...</B></spna></A>``` 此結構並不會被選取，因為 A 與 B 是間接關係
   
 - 條件(condition) (加上冒號當作過濾條件)
   - list (依據清單劃分)
     - order (依據順序)
       - ```:first-child``` (尋找第一個元素) 
         <br>(等效於```:nth-child(1)```)
       - ```:nth-child``` (尋找第 n 個元素) (nth 表示可計數)
       - ```:only-child``` (尋找個數只有它自己一個的元素)
       - ```:last-child``` (尋找最後一個元素)
     - type (依據清單類型劃分，像是資料庫的 having by type)
       - ```:first-of-type``` (尋找各類型的第一個元素) 
         <br>(等效於```:first```)
         <br>(等效於```:nth-of-type(1)```)
       - ```:nth-of-type``` (尋找各類型的第 n 個元素) (nth 表示可計數)
       - ```:only-of-type``` (尋找各類型元素中，個數只有它自己一個的元素)
       - ```:last-of-type``` (尋找各類型的最後一個元素)
   - ```:nth-xxx``` (可計數 API 以 nth- 起始) (nth 表示可計數)
   - ```:empty``` (尋找沒有子元素的元素)
   - ```:not(selector)``` (反向選擇器)
   - ```:hover``` (當滑鼠在上面的時候觸發)
     ```css
     <style>
         .myClass:hover {
             color: red;
             background: yellow;
	        }
     </style>
     ```
   - ```:before```
   - ```:after```
   
 - 偽元素：不是真正的網頁元素，但其行為與表現卻和真正的網頁元素一樣
   - ```::before``` ([介紹](https://www.oxxostudio.tw/articles/201706/pseudo-element-1.html))
   - ```::after``` ([介紹](https://www.oxxostudio.tw/articles/201706/pseudo-element-1.html))
   - ```::first-line```
   - ```::first-letter```
   - ```::selection```
   
 - 屬性(attribute)
   - ```tag[attr]```
   - ```[attr]```
   - ```[attr="xxx"]```
     - 根據搜尋來劃分：
       - ```[attr^="xxx"]```
       - ```[attr*="xxx"]```
       - ```[attr$="xxx"]```
   - 為何需要此設計?
     - 可以將套用範圍，控制在局部區域
     - 範例：https://vue-loader-v14.vuejs.org/zh-cn/features/scoped-css.html
       ```css
       <style>
           .example[data-v-f3f3eg9] {
               color: red;
           }
       </style>
       ```
       ```html
       <div class="example" data-v-f3f3eg9>hi</div>
       ```

## 基礎學習資源
 - [CSS闖關遊戲](http://flukeout.github.io/)
   - Answers: [CSS Diner.md](CSS%20Diner.md)

 - [[mozilla] CSS](https://developer.mozilla.org/zh-CN/docs/Learn/CSS/Introduction_to_CSS/Simple_selectors)
