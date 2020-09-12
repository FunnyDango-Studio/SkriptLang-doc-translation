翻譯自https://github.com/SkriptLang/Skript/tree/master/docs
# Skript文件模板

Skripts功能直接記錄在其Java代碼中。 但是我們仍然需要

1. HTML CSS和（可能的）Javascript代碼從這些創建網站
2. 清楚的教學，而不僅僅是“您可以檢查語法模式”
3. 舉例說明，如果需要

生成最終結果時，每個HTML文件都被template.html包圍，
它提供head元素，導航欄等。

## 模板圖案

模式的語法為 ${pattern_here}. 例如, ${skript.version} 被替換為
當前的Skript版本。 請參閱下面的更多信息...

您還可以通過使用其他文件 ${include <filename>}. 請做
確保這些包含的文件沒有位置不允許的標籤
哪裡包括稱為.

## 模式參考
```
skript.* - Skript訊息
version - Skript 版本
include <filename> - 讀取指定文件並將其放在此處
generate <expressions/effects/events/types/functions> <loop template file> - 產生參考
content - 在template.html中，標記放置其他文件的位置
```
