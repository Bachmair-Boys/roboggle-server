# Interview Bot Server

Ensure that you have the lastest version of Node.js installed and preferably the lastest version of sqlite installed. Once this is done run:
'''
git clone https://github.com/Bachmair-Boys/interview-bot-server
cd interview-bot-server
'''

# Running

'''
npm start
'''

# Interview Bot API

# Category Identification
BASIC = 0
BEHAVIORAL = 1
SALARY = 2
BRAINTEASER = 3

# RETURN CODES
SUCCESS = 0
DATABASE_CONNECTION_ERROR = 100
DATABASE_LOOKUP_ERROR = 101

## Methods
---
get-count: POST, Gets the number of questions in a given question category.<br>
Parameters:<br>
&nbsp;&nbsp;&nbsp;&nbsp;**category**: int, category identification number to get count from<br>
Return:<br>
&nbsp;&nbsp;&nbsp;&nbsp;JSON-Encoded Data: {<br>
&nbsp;&nbsp;&nbsp;&nbsp;status: int, SUCCESS if check succeeded, DATABASE_LOOKUP_ERROR otherwise,<br>
&nbsp;&nbsp;&nbsp;&nbsp;count: int, number of comments in the requested category<br>
&nbsp;&nbsp;&nbsp;&nbsp;}<br>
<br>
get-question: POST, Gets the requested question number in the requested question category.<br>
Parameters:<br>
&nbsp;&nbsp;&nbsp;&nbsp;**category**: int, category identification number to find question in.<br>
&nbsp;&nbsp;&nbsp;&nbsp;**question**: int, number of the question in the category<br>
Return: <br>
&nbsp;&nbsp;&nbsp;&nbsp; JSON-Encoded Data: {<br>
&nbsp;&nbsp;&nbsp;&nbsp;status: int, SUCCESS if check succeeded, DATABASE_LOOKUP_ERROR otherwise,<br>
&nbsp;&nbsp;&nbsp;&nbsp;count: int, number of comments in the requested category<br>
&nbsp;&nbsp;&nbsp;&nbsp;}<br>



&nbsp;&nbsp;&nbsp;&nbsp;
