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
<br>

<li>All action is repeated as long as the selected rows/columns are found at other locations.</li>
  <ul><li>Thus, do start at the top</li></ul>
<li>After every action, the contents will be saved to a file that is the original name with a string "_cleaned".</li>
<li>When a cell is inserted, all the cells at right will be shifted to the right</li>
<li>When a cell is deleted, all the cells at right will be shifted to the left and the cell at the last column will be empty.</li>  
</ul>
<br>
