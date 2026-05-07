# Power BI Dynamic Image Library
**Documentation Date:** 2026-03-01  
**Version:** 1.0  

## 🚀 Overview
This repository hosts SVG assets used as dynamic icons in Power BI reports. By referencing these raw URLs, icons can be updated globally without re-publishing `.pbix` files.

## 🛠️ How to use in Power BI
To display these images in a table or gallery, use the **Raw** GitHub URL format.

### URL Structure
`https://raw.githubusercontent.com/BritishTJK/images/main/[FileName].svg`

### Example DAX Measure
```dax
SVG Icon = 
VAR _Base = "[https://raw.githubusercontent.com/BritishTJK/images/main/](https://raw.githubusercontent.com/BritishTJK/images/main/)"
VAR _FileName = "Bronze.svg" 
RETURN
_Base & _FileName
