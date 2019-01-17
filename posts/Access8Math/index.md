---
layout:  post
id:  769
title:  "[NVDA addon] 数学阅读程序 Access8Math V2.0 新增自订朗读功能与可自行加入新语言"
slug:  "Access8Math"
categories:  "插件下载"
tags:  ""
permalink:  "/archives/:slug.html"
author:  "tsengwoody"
date:  2018-01-21 20:56:00
---



<body>
<h1>Access8Math 各相關網址</h1>
<a href="https://addons.nvda-project.org/addons/access8math.zh_CN.html">Access8Math 附加元件官方社群網站頁面</a>
<a href="https://github.com/tsengwoody/Access8Math">Access8Math GitHub 主頁</a>
<a href="https://github.com/tsengwoody/Access8Math/releases">Access8Math GitHub 發佈頁</a>
<a href="https://github.com/tsengwoody/Access8Math/releases/download/v2.0/Access8Math-2.0.nvda-addon">Access8Math v2.0 下載點</a>
<h1>Access8Math v2.0 更新日志</h1>
<ul>
<li>加入多国语系新增与客制化设定功能，新增三个窗口「unicode 字典」、「数学规则」、「加入新语言」</li>
<li>unicode 字典可客制设定各项符号文字的报读方式。</li>
<li>数学规则可客制设定各数学类型的报读方式并可于修改完成前透过范例的按钮先行查阅修改的效果。</li>
<li>加入新语言可加入原先于内建未提供的语言，加入后于一般设定内会多出刚新增的语系并可再透过「unicode 字典」与「数学规则」定义读法达到多国语言客制化设定</li>
<li>优化在互动模式下，可使用数字键7~9以行为单位阅读序列文字</li>
</ul>
<h1>Access8Math 说明</h1>
<p>此NVDA addon提供数学内容的阅读，原先NVDA亦有此功能，但因是调用MathPlayer的功能，部份功能尚显不足，尤其一些语言未提供导航浏览(交互式阅读部份内容)。</p>
<p>导航浏览对于阅读理解长数学内容相当重要，可协助理解长数学内容的结构。</p>
<h2>功能</h2>
<ul>
<li>可阅读网页浏览器(Mozilla Firefox, Microsoft Internet Explorer and Google Chrome)上以MathML撰写的数学内容</li>
<li>可阅读Microsoft Word上以MathType 撰写的数学内容。(需安装MathType)</li>
<li>在数学内容上按空格键后开启「Access8Math 互动窗口」，窗口内含有「互动」、「复制」按钮。<ul>
<li>互动：与该数学内容进行导航浏览，亦即可部份浏览数学内容中的子内容并在子内容间移动或缩放子内容大小</li>
<li>复制：复制对象MathML原始码</li>
</ul>
</li>
<li>在导航浏览时会提示该项子内容在其上层子内容的意义</li>
<li>在导航浏览时按键：<ul>
<li>向下键缩小当前数学内容成更小的子内容</li>
<li>向上键放大当前数学内容成更大的子内容</li>
<li>向左键向前一项数学内容</li>
<li>向右键向后一项数学内容</li>
<li>home键回到最顶层(完整数学内容)</li>
<li>"Ctrl+c": 复制对象MathML原始码</li>
<li>数字键盘1-9：使用NVDA Reviewing Text方式阅读序列化的数学内容</li>
<li>esc键退出导航浏览模式</li>
</ul>
</li>
<li>ctrl+alt+m：可在Access8Math与MathPlayer间切换阅读器(有安装MathPlayer才能切换)</li>
</ul>
<h2>菜单</h2>
<ul>
<li>「一般设定」对话框，可设定：<ul>
<li>语言：Access8Math 朗读数学内容的语言</li>
<li>项目间隔时间：设定项目间停顿时间，数值从1到100，数值愈小表示停顿时间愈短，反之数值愈大表示停顿时间愈长。</li>
<li>分析内容的数学意义：将数学内容进行语意分析，符合特定规则时，以该规则的数学意义进行朗读</li>
<li>读出字典有定义模式的意义：当字典文件有定义时，使用字典文件读出提示该项子内容在其上层子内容的意义</li>
<li>读出自动生成的意义：当字典文件无定义或不完整时，使用自动产生功能读出提示该项子内容在其上层子内容的意义或项次</li>
</ul>
</li>
<li>「规则设定」对话框：可选择特定规则是否启用的设定。</li>
<li>「unicode 字典」可客制设定各项符号文字的报读方式。</li>
<li>「数学规则」可客制设定各数学类型的报读方式。</li>
<li>「加入新语言」可加入原先于内建未提供的语言，加入后于一般设定内会多出刚新增的语系并可再透过「unicode 字典」与「数学规则」定义读法达到多国语言客制化设定</li>
</ul>
<h2>数学规则</h2>
<p>Access8Math将常用数学式依据类型与逻辑，建立43项数学规则，程序依据这套规则判别数学式的念法与念读顺序，依据各地习惯不同，可以变更数学念读顺序与念法，方法如下：</p>
<p>编辑: 进入"数学规则"后，小窗口列有43项数学规则，选则任一规则可选择"编辑按钮"进入编辑条目。</p>
<p>规则的"编辑条目"可分为两大区块，分别是序列化顺序与子节点角色。
    *   序列化顺序：将数学规则依据念读顺序划分多个区块，在此区域可变更规则子项目的念读顺序及开始、项目间与结束的分隔文字，以分数规则mfrac为例，此规则分为五个念读顺序，顺序0、2和4分别代表起始提示、项目区隔提示与结束提示，可在各字段中输入变更自己习惯的念法，而顺序1与3则可调整子节点念读的先后，可于下拉式选单中变更顺序。
    *   子节点角色：为该数学规则的下一阶层子项目，以分数规则mfrac为例，此项规则就包含分子与分母两项，而在子节点字段中，可以变更该项子内容在其上层子内容的意义文字，。</p>
<p>范例：可先行查阅确认编辑修改后对此类型的数学规则读法。点击后会出现一个预设好符合该对应数学规则的数学内容，供确认对此类型的数学规则读法是否符合预期。</p>
<p>还原默认值：将数学规则列表还原到初始默认值。</p>
<p>汇入：将数学规则档案汇入，可用于加载数学规则档案。</p>
<p>汇出：将数学规则档案储存于指定路径，以利分享或保存数学规则档案。</p>
<h2>其它</h2>
<pre><code>简单规则：简单规则是各种规则的简化版，当其内容仅为单一项目时，便可省略前后标记朗读，以达到更好的理解与阅读，而亦不致造成混淆
</code></pre>
<p>数学内容解析数学规则意义持续增加中</p>
<p>目前先针对以Presentation Markup写成的MathML处理，因word、math type、wiris等MathML图形化输入工具产生的MathML皆为此型态</p>
<p>维基百科上的数学内容皆以MathML写成</p>
<ul>
<li>矩阵乘法：https://zh.wikipedia.org/zh-tw/%E7%9F%A9%E9%99%A3%E4%B9%98%E6%B3%95</li>
<li>
<p>三次方程：https://zh.wikipedia.org/zh-tw/%E4%B8%89%E6%AC%A1%E6%96%B9%E7%A8%8B</p>
</li>
<li>
<p>例子</p>
<ul>
<li>一元二次方程解：
<math xmlns="http://www.w3.org/1998/Math/MathML"><mfrac><mrow><mo>-</mo><mi>b</mi><mo>&#xB1;</mo><msqrt><msup><mi>b</mi><mn>2</mn></msup><mo>-</mo><mn>4</mn><mi>a</mi><mi>c</mi></msqrt></mrow><mrow><mn>2</mn><mi>a</mi></mrow></mfrac></math></li>
<li>二项式定理：
<math xml:lang="zh_TW">
  <semantics>
<mrow class="MJX-TeXAtom-ORD">
  <mstyle displaystyle="true" scriptlevel="0">
    <mo stretchy="false">(</mo>
    <mn>1</mn>
    <mo>+</mo>
    <mi>x</mi>
    <msup>
      <mo stretchy="false">)</mo>
      <mrow class="MJX-TeXAtom-ORD">
        <mi>α<!-- α --></mi>
      </mrow>
    </msup>
    <mo>=</mo>
    <munderover>
      <mo>∑<!-- ∑ --></mo>
      <mrow class="MJX-TeXAtom-ORD">
        <mi>n</mi>
        <mo>=</mo>
        <mn>0</mn>
      </mrow>
      <mrow class="MJX-TeXAtom-ORD">
        <mi mathvariant="normal">∞<!-- ∞ --></mi>
      </mrow>
    </munderover>
    <mi>C</mi>
    <mo stretchy="false">(</mo>
    <mi>α<!-- α --></mi>
    <mo>,</mo>
    <mi>n</mi>
    <mo stretchy="false">)</mo>
    <msup>
      <mi>x</mi>
      <mrow class="MJX-TeXAtom-ORD">
        <mi>n</mi>
      </mrow>
    </msup>
    <mspace width="1em"></mspace>
    <mi mathvariant="normal">∀<!-- ∀ --></mi>
    <mi>x</mi>
    <mo>:</mo>
    <mrow>
      <mo>|</mo>
      <mi>x</mi>
      <mo>|</mo>
    </mrow>
    <mo>&lt;</mo>
    <mn>1</mn>
    <mo>,</mo>
    <mi mathvariant="normal">∀<!-- ∀ --></mi>
    <mi>α<!-- α --></mi>
    <mo>∈<!-- ∈ --></mo>
    <mrow class="MJX-TeXAtom-ORD">
      <mi mathvariant="double-struck">C</mi>
    </mrow>
  </mstyle>
</mrow>
<annotation encoding="application/x-tex">{\displaystyle (1+x)^{\alpha }=\sum _{n=0}^{\infty }C(\alpha ,n)x^{n}\quad \forall x:\left|x\right|&lt;1,\forall \alpha \in \mathbb {C} }</annotation>
  </semantics>
</math></li>
</ul>
</li>
</ul>
<p>原始码：https://github.com/tsengwoody/Access8Math</p>
<p>欢迎提出见意与bug回报，谢谢！</p>
</body>