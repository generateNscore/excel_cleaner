# xlcolumnizer

## What is it?

A package that helps you recover columns of Excel data converted from PDF files.

## Where to get it

<pre lang=sh>pip install xlcolumnizer</pre>

## Dependencies

<ul><li><a href="https://openpyxl.readthedocs.io/en/stable/">openpyxl</a></li>
<li><a href="https://github.com/ragardner/tksheet">tksheet</a></li></ul>

## Changes
<ul>
<li>Version 0.0.1</li>

```python

import xlcolumnizer as xl

xlpath='<full name of your excel file including extension>'
xl.sheet(xlpath)

```

<ul><li>A GUI with tksheet will be opened with the contents of excel file.</li>
<li>Here is a recommending set of steps:</li>
<ol><li>Remove unwanted rows</li>
<li>Remove unwanted columns or combine columns</li>
  <li>Click a cell to insert or delete the cell/li></ol>


<li>Click a topmost row number and drag to the row to select</li>
<li>Press a Function key, for example F7, to delete the selected rows.</li>

</ul>
<br>
