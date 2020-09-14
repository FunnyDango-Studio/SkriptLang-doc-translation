翻譯自https://github.com/SkriptLang/Skript/tree/master/docs
# Skript文件範例

Skript的特色都已經直接註解在Java程式碼中了。但仍需

1. HTML、CSS和Javascript來建立網站
2. 明瞭教學，而並非只是「你能夠確認該語法」
3. 若有需要，請解析範例

當在產生最終結果時，每個HTML檔都需要依循著template.html
所提供的head元素及導覽列等等……。

## 範例語法

語法皆有其標準${pattern_here}。比如說，${skript.version}是用來取代
目前Skript版本。請詳見以下內容以獲取更多資訊……。

您也可以利用${include <filename>}來引入檔案。僅需確
保所引入的檔案內未含使在被呼叫時不被允許的標籤。

## 語法參考
```
skript.* - Skript的資訊
version - Skript的版本
include <filename> - 載入所獲檔案並將其置於此
generate <expressions/effects/events/types/functions> <loop template file> - 已產生的語法參考
content - In template.html, marks the point where other file is placed 在template.html中，標註已放有其他檔案的點
```
