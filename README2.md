# 个性化配置

## 默认英文输入模式

+ 全局配置：将ascii_mode的值改为1
+ 每个应用单独设置：在 squirrel 或 weasel 里参考注释，在 app_options 下面设定

## 候选词横向排列

在weasel.custom.yaml中添加一行：
`
patch:
    "style/horizontal": true
`

wease.custom.yaml配置：

``` yaml
patch:

    "style/horizontal": true # 横向排列：true；false
    "preset_color_schemes/+":
        __include: "weasel_style:/preset_color_schemes"
    "style/+":
        __include: "weasel_style:/style"    
```
