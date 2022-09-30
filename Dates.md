<h2>Regex Date 1-1</h2>

<h3>Explanation</h3>
<p>D/M/YYYY DD/M/YYYY D/MM/YYYY DD/MM//YYYY and also swapped around as well (year/month/day)
with seperators being - / or (whitspace)<br>
(\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])[-/\s]+(1[0-2]|0[1-9]|[1-9])[-/\s]+(\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])<br>
Group 1, 2 and 3 can be used to decipher between year or date at the start.</p>

<h3>Example in Psuedo/Python Code</h3>
<h5><b>CODE:</b></h5>
<p>regular_expression = (\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])[-/\s]+(1[0-2]|0[1-9]|[1-9])[-/\s]+(\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])<br>
string1 = '12/4/2012'<br>
regular_expression_complete = ReGex(regular_expression , string1)<br>
print(regular_expression_complete[0]) \#group 1 <br>
print(regular_expression_complete[1])<br>
print(regular_expression_complete[2])</p>
<h5><b>OUTPUT:</b></h5>
<p><i>12</i></p>
<p><i>4</i></p>
<p><i>2012</i></p>



<h2>Regex Date 1-2</h2>

<h3>Explanation</h3>
<p>D/M/YYYY DD/M/YYYY D/MM/YYYY DD/MM//YYYY and also swapped around as well (year/month/day)
with seperators being - / or (whitspace)<br>
(\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])([-/\s]+)(1[0-2]|0[1-9]|[1-9])([-/\s]+)(\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])<br>
Group 1, 3 and 5 can be used to decipher between year or date at the start. while groups 2 and 4 can be used to see what seperators have been used</p>

<h3>Example in Psuedo/Python Code</h3>
<h5><b>CODE:</b></h5>
<p>regular_expression = (\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])([-/\s]+)(1[0-2]|0[1-9]|[1-9])([-/\s]+)(\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])<br>
string1 = '12/4-2012'<br>
regular_expression_complete = ReGex(regular_expression , string1)<br>
print(regular_expression_complete[0]) \#group 1 <br>
print(regular_expression_complete[1])<br>
print(regular_expression_complete[2])</p>
print(regular_expression_complete[3])</p>
print(regular_expression_complete[4])</p>
<h5><b>OUTPUT:</b></h5>
<p><i>12</i></p>
<p><i>/</i></p>
<p><i>4</i></p>
<p><i>-</i></p>
<p><i>2012</i></p>
