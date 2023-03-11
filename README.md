# GmlSpec-CN
Translation for GmlSpec.xml 

## 解决载入时载入报错

找到 OmegaT 安装目录下的 `OmegaT.l4J.ini`，并在该文件结尾添加以下参数：

```ini
-Djdk.xml.xpathExprGrpLimit=0
-Djdk.xml.xpathExprOpLimit=0
-Djdk.xml.xpathTotalOpLimit=0
-XX:-UseGCOverheadLimit
```

