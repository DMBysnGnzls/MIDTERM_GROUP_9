# MIDTERM_GROUP_9

# DATE AND TIME FUNCTION
<b>TEXT Function</b><br>
>-The <b>TEXT(date, format_text)</b> function in Excel is used to convert a date or time value into a text string with a specific format. It allows you to display a date or time in a custom format of your choice. The function takes two arguments:<br>
>-<b><i>date</b></i>: This is the date or time value you want to format as text.
>-<b><i>format_text</b></i>: This is a text string that specifies the format you want for the resulting text. The format_text argument uses various codes to represent different components of the date or time (e.g., "mm" for month, "dd" for day, "yyyy" for year, "hh" for hours, "mm" for minutes, "ss" for seconds, etc.). You can also include separators like slashes, dashes, or spaces in the format_text.<br>
<b>Here are some examples of how you can use the TEXT function:</b><br>
=<b><i>=TEXT(A1, "mm/dd/yyyy")</b></i>: Converts the date in cell A1 into a text string in the format "mm/dd/yyyy". For example, "01/15/2023".<br>
=<b><i>=TEXT(NOW(), "dd-mmm-yyyy hh:mm:ss")</b></i>: Converts the current date and time into a text string in the format "dd-mmm-yyyy hh:mm:ss". For example, "15-Oct-2023 14:30:00".<br>
=<b><i>=TEXT(A2, "dddd, mmmm dd, yyyy")</b></i>: Converts the date in cell A2 into a text string in the format "dddd, mmmm dd, yyyy". For example, "Sunday, October 15, 2023".<br>							
![image](https://github.com/nthnlgmz/MIDTERM_GROUP_9/assets/143614589/e9d119c2-3933-41f8-8432-8d855ada6e06)

<b>DATEDIF Function</b><br>
>-The <b>DATEDIF</b> function in Excel is used to calculate the difference between two dates and return the result in terms of days, months, or years. It stands for "Date Difference." The function takes the following arguments:<br>
>-<b><i>start_date</b></i>: This is the starting date for the calculation.<br>
>-<b><i>end_date</b></i>: This is the ending date for the calculation.<br>
>-<b><i>unit</b></i>: This is a text argument that specifies the unit of time you want to calculate the difference in. The available unit options are:<br>
=<b><i>"d"</b></i>: Calculates the difference in days.<br>
=<b><i>"m"</b></i>: Calculates the difference in months.<br>
=<b><i>"y"</b></i>: Calculates the difference in years.<br>
![image](https://github.com/nthnlgmz/MIDTERM_GROUP_9/assets/143614589/770be4f2-1ff6-4f0a-abf5-639a21a4e9be)

<b>WEEKDAY Function</b><br>
>-The <b><i>WEEKDAY</b></i> function in Excel is used to determine the day of the week (i.e., Sunday, Monday, Tuesday, etc.) for a given date and returns the corresponding number for that day. The function takes the following arguments:<br>
>-<b><i>date</b></i>: This is the date for which you want to find the day of the week.<br>
>-<b><i>[return_type]</b></i> (optional): This is an optional argument that specifies the type of result you want. It can take one of the following values:<br>
=<b><i>1 (default)</b></i>: Returns numbers from 1 (Sunday) to 7 (Saturday).<br>
=<b><i>2</b></i>: Returns numbers from 1 (Monday) to 7 (Sunday).<br>
=<b><i>3</b></i>: Returns numbers from 0 (Monday) to 6 (Sunday).<br>
![image](https://github.com/nthnlgmz/MIDTERM_GROUP_9/assets/143614589/82622b59-9923-47df-8733-f5c8ede416f5)
			
# TEXT FUNCTION
<b>LEN Function</b><br>
>-The <b><i>LENGTH</b></i> function, also known as <b><i>LEN</b></i>, is not a specific function in Excel. Instead, it's typically referred to as LEN in Excel. The LEN function is used to count the number of characters in a text string, including letters, numbers, spaces, and special characters. It can be helpful for various tasks, such as checking the length of a cell's content or manipulating text data.<br>
<b>Syntax: <b><i>=LEN(text)</b></i></b><br>
>-The <b><i>LEN</b></i> function is versatile and can be used in various situations where you need to work with text lengths, such as validating input lengths, truncating text, or performing conditional formatting based on text length.<br>
![image](https://github.com/nthnlgmz/MIDTERM_GROUP_9/assets/143614589/d35ec47f-4971-4240-b0c3-e186b81d15c7)

<b>LEFT Function</b><br>
>-The <b><i>LEFT</b></i> function in Excel is used to extract a specified number of characters from the beginning (left side) of a text string. It's useful when you want to obtain a portion of text from the start of a longer text string. The syntax for the LEFT function is as follows:<br>
<b>Syntax: <b><i>=LEFT(text, num_chars)</b></i></b><br>
<b><i>text</b></i>: This is the text string from which you want to extract characters.<br>
<b><i>num_chars</b></i>: This is the number of characters you want to extract from the beginning of the text string.<br>
![image](https://github.com/nthnlgmz/MIDTERM_GROUP_9/assets/143614589/2ec7d4c7-0c4e-4098-9879-17f5208e22f0)

<b>UPPER AND LOWER Function</b><br>
>-In Excel, the <b><i>UPPER</b></i> and <b><i>LOWER</b></i> functions are used to change the case of text in a cell. Here's how each of these functions works:<br>
<b><i>UPPER Function:</b></i><br>
The <b><i>UPPER</b></i> function is used to convert all the characters in a text string to uppercase (capital letters).<br>
<b>Syntax: <b><i>=UPPER(text)</b></i></b><br>
<b><i>text</b></i>: This is the text string you want to convert to uppercase.<br><br>
<b><i>LOWER Function:</b></i><br>
The <b><i>LOWER</b></i> function is used to convert all the characters in a text string to lowercase (small letters).<br>
<b>Syntax: <b><i>=LOWER(text)</b></i></b><br>
<b><i>text</b></i>: This is the text string you want to convert to lowercase.<br>
![image](https://github.com/nthnlgmz/MIDTERM_GROUP_9/assets/143614589/18fd5017-b4b2-4c86-8f08-305699f122e4)

