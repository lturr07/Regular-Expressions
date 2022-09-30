<h2>Regex Date 1</h2>

<h4>Explanation</h4>
<p>D/M/YYYY DD/M/YYYY D/MM/YYYY DD/MM//YYYY and also swapped around as well (year/month/day)
with seperators being - / or ' '(whitspace)</p>
<p>(\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])[-/\s]+(1[0-2]|0[1-9]|[1-9])[-/\s]+(\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])</p>
<p>Group 1, 2 and 3 can be used to decipher between year or date at the start.</p>

<h4>Example in Psuedo/Python Code</h4>
<h6>CODE:</h6>
<p>regular_expression = (\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])[-/\s]+(1[0-2]|0[1-9]|[1-9])[-/\s]+(\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])</p>
<p>string1 = '12/4/2012'</p>
<p>regular_expression_complete = ReGex(regular_expression , string1)</p>
<p>print(regular_expression_complete[0])</p>
<p>print(regular_expression_complete[1])</p>
<p>print(regular_expression_complete[2])</p>
<h6>OUTPUT:</h6>
<p>12</p>
<p>4</p>
<p>2012</p>
