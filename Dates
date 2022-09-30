<h2>Regex Date 1</h2>

<h4>Explanation</h4>
D/M/YYYY DD/M/YYYY D/MM/YYYY DD/MM//YYYY and also swapped around as well (year/month/day)
with seperators being - / or ' '(whitspace)
(\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])[-/\s]+(1[0-2]|0[1-9]|[1-9])[-/\s]+(\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])
Group 1, 2 and 3 can be used to decipher between year or date at the start.

<h4>Example in Psuedo/Python Code</h4>
<h6>CODE:</h6>
regular_expression = (\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])[-/\s]+(1[0-2]|0[1-9]|[1-9])[-/\s]+(\d{4}|3[01]|[1-2][0-9]|0[1-9]|[1-9])
string1 = '12/4/2012'
regular_expression_complete = ReGex(regular_expression , string1)
print(regular_expression_complete[0])
print(regular_expression_complete[1])
print(regular_expression_complete[2])
<h6>OUTPUT:</h6>
>>> 12
>>> 4
>>> 2012


<h2>Regex Date 2</h2>

<h4>Explanation</h4>

<h4>Example in Psuedo/Python Code</h4>
<h6>CODE:</h6>
<h6>OUTPUT:</h6>
