# 执行动作命令

## 使用方式

```javascript
import Editor from "@hufe921/canvas-editor"

const instance = new Editor(container, <IElement[]>data, options)
instance.command.commandName()
```

## executeMode
功能：切换编辑器模式（编辑、清洁、只读）

用法：
```javascript
instance.command.executeMode(EditorMode)
```

## executeCut
功能：剪切

用法：
```javascript
instance.command.executeCut()
```

## executeCopy
功能：复制

用法：
```javascript
instance.command.executeCopy()
```

## executePaste
功能：粘贴

用法：
```javascript
instance.command.executePaste()
```

## executeSelectAll
功能：全选

用法：
```javascript
instance.command.executeSelectAll()
```

## executeBackspace
功能：向前删除

用法：
```javascript
instance.command.executeBackspace()
```

## executeSetRange
功能：设置选区

用法：
```javascript
instance.command.executeSetRange(startIndex, endIndex)
```

## executeUndo
功能：撤销

用法：
```javascript
instance.command.executeUndo()
```

## executeRedo
功能：重做

用法：
```javascript
instance.command.executeRedo()
```

## executePainter
功能：格式刷-复制样式

用法：
```javascript
instance.command.executePainter()
```

## executeApplyPainterStyle
功能：格式刷-应用样式

用法：
```javascript
instance.command.executeApplyPainterStyle()
```

## executeFormat
功能：清除样式

用法：
```javascript
instance.command.executeFormat()
```

## executeFont
功能：设置字体

用法：
```javascript
instance.command.executeFont(font)
```

## executeSizeAdd
功能：增大字号

用法：
```javascript
instance.command.executeSizeAdd()
```

## executeSizeMinus
功能：减小字号

用法：
```javascript
instance.command.executeSizeMinus()
```

## executeBold
功能：字体加粗

用法：
```javascript
instance.command.executeBold()
```

## executeItalic
功能：字体斜体

用法：
```javascript
instance.command.executeItalic()
```

## executeUnderline
功能：下划线

用法：
```javascript
instance.command.executeUnderline()
```

## executeStrikeout
功能：删除线

用法：
```javascript
instance.command.executeStrikeout()
```

## executeSuperscript
功能：上标

用法：
```javascript
instance.command.executeSuperscript()
```

## executeSubscript
功能：上下标

用法：
```javascript
instance.command.executeSubscript()
```

## executeColor
功能：字体颜色

用法：
```javascript
instance.command.executeColor()
```

## executeHighlight
功能：高亮

用法：
```javascript
instance.command.executeHighlight()
```

## executeLeft
功能：行居左

用法：
```javascript
instance.command.executeLeft()
```

## executeCenter
功能：行居中

用法：
```javascript
instance.command.executeCenter()
```

## executeRight
功能：行居右

用法：
```javascript
instance.command.executeRight()
```

## executeAlignment
功能：行两端对齐

用法：
```javascript
instance.command.executeAlignment()
```

## executeRowMargin
功能：行间距

用法：
```javascript
instance.command.executeRowMargin(number)
```

## executeInsertTable
功能：插入表格

用法：
```javascript
instance.command.executeInsertTable(row, col)
```

## executeInsertTableTopRow
功能：向上插入一行

用法：
```javascript
instance.command.executeInsertTableTopRow()
```

## executeInsertTableBottomRow
功能：向下插入一行

用法：
```javascript
instance.command.executeInsertTableBottomRow()
```

## executeInsertTableLeftCol
功能：向左插入一列

用法：
```javascript
instance.command.executeInsertTableLeftCol()
```

## executeInsertTableRightCol
功能：向右插入一列

用法：
```javascript
instance.command.executeInsertTableRightCol()
```

## executeDeleteTableRow
功能：删除当前行

用法：
```javascript
instance.command.executeDeleteTableRow()
```

## executeDeleteTableCol
功能：删除当前列

用法：
```javascript
instance.command.executeDeleteTableCol()
```

## executeDeleteTable
功能：删除表格

用法：
```javascript
instance.command.executeDeleteTable()
```

## executeMergeTableCell
功能：合并表格

用法：
```javascript
instance.command.executeMergeTableCell()
```

## executeCancelMergeTableCell
功能：取消合并表格

用法：
```javascript
instance.command.executeCancelMergeTableCell()
```

## executeImage
功能：插入图片

用法：
```javascript
instance.command.executeImage({
  width: number;
  height: number;
  value: string;
})
```

## executeHyperlink
功能：插入链接

用法：
```javascript
instance.command.executeHyperlink({
  type: ElementType.HYPERLINK,
  value: '',
  url,
  valueList: IElement[]
})
```

## executeDeleteHyperlink
功能：删除链接

用法：
```javascript
instance.command.executeDeleteHyperlink()
```

## executeCancelHyperlink
功能：取消链接

用法：
```javascript
instance.command.executeCancelHyperlink()
```

## executeEditHyperlink
功能：编辑链接

用法：
```javascript
instance.command.executeEditHyperlink(newUrl)
```

## executeSeparator
功能：插入分割线

用法：
```javascript
instance.command.executeSeparator(dashArray)
```

## executePageBreak
功能：分页符

用法：
```javascript
instance.command.executePageBreak()
```

## executeAddWatermark
功能：添加水印

用法：
```javascript
instance.command.executeAddWatermark({
  data: string;
  color?: string;
  opacity?: number;
  size?: number;
  font?: string;
})
```

## executeDeleteWatermark
功能：添加水印

用法：
```javascript
instance.command.executeDeleteWatermark()
```

## executeSearch
功能：搜索

用法：
```javascript
instance.command.executeSearch(keyword)
```

## executeSearchNavigatePre
功能：搜索导航-上一个

用法：
```javascript
instance.command.executeSearchNavigatePre()
```

## executeSearchNavigateNext
功能：搜索导航-下一个

用法：
```javascript
instance.command.executeSearchNavigateNext()
```

## executeReplace
功能：搜索替换

用法：
```javascript
instance.command.executeReplace(newWord)
```

## executePrint
功能：打印

用法：
```javascript
instance.command.executePrint()
```

## executeReplaceImageElement
功能：替换图片

用法：
```javascript
instance.command.executeReplaceImageElement(newUrl)
```

## executeSaveAsImageElement
功能：另存为图片

用法：
```javascript
instance.command.executeSaveAsImageElement()
```

## executeChangeImageDisplay
功能：改变图片行显示方式

用法：
```javascript
instance.command.executeSaveAsImageElement(element, display)
```

## executePageMode
功能：页面模式

用法：
```javascript
instance.command.executePageMode(pageMode)
```

## executePageScaleRecovery
功能：恢复页面原始缩放比例

用法：
```javascript
instance.command.executePageMode()
```

## executePageScaleMinus
功能：页面缩小

用法：
```javascript
instance.command.executePageScaleMinus()
```

## executePageScaleAdd
功能：页面放大

用法：
```javascript
instance.command.executePageScaleAdd()
```

## executePaperSize
功能：设置纸张大小

用法：
```javascript
instance.command.executePaperSize(width, height)
```

## executeSetPaperMargin
功能：设置纸张页边距

用法：
```javascript
instance.command.executeSetPaperMargin([top: number, right: number, bottom: number, left: number])
```

## executeInsertElementList
功能：插入元素

用法：
```javascript
instance.command.executeInsertElementList(IElement[])
```

## executeRemoveControl
功能：删除控件

用法：
```javascript
instance.command.executeRemoveControl()
```

## executeSetLocale
功能：设置本地语言

用法：
```javascript
instance.command.executeSetLocale(locale)
```