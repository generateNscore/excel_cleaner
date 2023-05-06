# excelcleaner

## What is it?

A package that helps you clean and recover columns of Excel data converted from PDF files.

## Where to get it

<pre lang=sh>pip install excelcleaner</pre>

## Dependencies

<ul><li><a href="https://openpyxl.readthedocs.io/en/stable/">openpyxl</a></li>
<li><a href="https://github.com/ragardner/tksheet">tksheet</a></li></ul>

## Changes
<ul>
<li>Version 0.0.4</li>

```python

import excelcleaner as xl

xlpath='(excel file name with extension)'
xl.sheet(xlpath)

```

<ul><li>A tksheet window will be opened with the contents of excel file.</li>
<li>Here are recommending orders of actions to try:</li>
<ol><li>Remove unwanted rows (F7)</li>
<li>Remove unwanted columns (F7) or combine columns (F5)</li>
  <li>Click a cell to insert (F1) or delete the cell (F3)</li></ol>
<br>

<li>If the same pattern or kind of selected rows/columns is found at other locations, the same action is repeated for the found rows/columns.</li>
  <ul><li>Thus, it would better try one action at the top</li>
  <li>To remove rows, click the row names.</li>
    <li>To remove or combine columns, click the column names.</li></ul>
  <br>
<li>After every action, the contents will be saved to a file that is the original name with a string "_cleaned".</li>
<li>When a cell is inserted, all the cells at right will be shifted to the right and an extra column will be created with empty for all other rows that are not changed.</li>
<li>When a cell is deleted, all the cells at right will be shifted to the left and the cell at the last column will be empty.</li>
  <li>If one action is done by mistake, press function-key F12 to restore the the data before he last action</li></ul>
  <br>
<ul><li>After each action is completed,</li>
<ul><li>the number of columns and rows and the number of patterns of rows will be displayed</li>
<li>either a few columns or muliple rows are highlighted, which are indicative of ok to be deleted.</li></ul>
</ul>
</ul>
<br>
