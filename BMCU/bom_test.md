---
title: Untitled Page
description: 
published: true
date: 2025-03-21T16:26:13.389Z
tags: 
editor: markdown
dateCreated: 2025-03-21T16:15:22.212Z
---

# 动态物料清单示例

选择版本：
<select id="version" onchange="updateBOM()">
  <option value="None">click here</option>
  <option value="130">130版本</option>
  <option value="370">370版本</option>
</select>

选择类型：
<select id="type" onchange="updateBOM()">
  <option value="None">click here</option>
  <option value="steel">钢珠版</option>
  <option value="optic">光电版</option>
</select>

---

## 物料清单（BOM）

<div id="bom">
  请在上方选择版本和类型
</div>
