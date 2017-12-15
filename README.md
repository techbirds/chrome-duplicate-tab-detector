# chrome-duplicate-tab-detector

> chrome-duplicate-tab-detector is an extension for Google Chrome which alters the behaviour of opening a new tab to help reduce duplicate tabs (tabs displaying the same URL).
> When opening a new tab, and a duplicate tab exists in the same window, it closes the new tab and selects the duplicate tab. If there's no duplicate, the new tab is opened as usual.

Notes and limitations:
 * Only applies to new tabs--navigation within a single tab is not affected.
 * Tabs in other windows are ignored.
 * Does not handle redirects--the requested URL must match the duplicated page URL exactly to be considered a duplicate.
 * Does not detect new tabs which are opened via javascript (e.g. via bookmarklets)
 * Does not auto-update
 * 新增reload


 ## 安装

 1. 克隆工程到本地
 
 ```
 git clone https://github.com/techbirds/chrome-duplicate-tab-detector.git
 ```

 2. 加载插件

 chrome -> 窗口 -> 扩展程序 -> 加载已解压的扩展程序 -> 选择克隆所在的文件加载即可
 
 ## 示例
 
 ![path](http://g.recordit.co/NwhnpTnVZd.gif)

## 感谢

* [@mbhutton](https://github.com/mbhutton/chrome-duplicate-tab-detector)
