<h2>Regex Date 1</h2>

<h3>Explanation</h3>
<p>D/M/YYYY DD/M/YYYY D/MM/YYYY DD/MM//YYYY and also swapped around as well (year/month/day)
with seperators being - / or ' '(whitspace)</p>
<p>(\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])[-/\s]+(1[0-2]|0[1-9]|[1-9])[-/\s]+(\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])</p>
<p>Group 1, 2 and 3 can be used to decipher between year or date at the start.</p>

<h3>Example in Psuedo/Python Code</h3>
<h5>CODE:</h5>
<p>regular_expression = (\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])[-/\s]+(1[0-2]|0[1-9]|[1-9])[-/\s]+(\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])</p>
<p>string1 = '12/4/2012'</p>
<p>regular_expression_complete = ReGex(regular_expression , string1)</p>
<p>print(regular_expression_complete[0])</p>
<p>print(regular_expression_complete[1])</p>
<p>print(regular_expression_complete[2])</p>
<h5>OUTPUT:</h5>
<p><i>12</i></p>
<p><i>4</i></p>
<p><i>2012</i></p>
