# MIDTERM_GROUP_9

# LOGICAL FUNCTION
<b>ISBLANK Function</b><br>
>-The **ISBLANK** function in Excel is used to check whether a cell is empty or not. It returns **TRUE** if the cell is empty and **FALSE** if it contains any value or formula. <br>
-The syntax for the function is as follows: <br>
```
=ISBLANK(value)
```
>-Here, `value` is the cell or range that you want to check for blank cells. The function returns a Boolean value of `TRUE` or `FALSE` based on whether the selected cell or range of cells is blank or not ³.<br>
-You can also use an empty string (`""`) with Excel's math operators `=` or `<>` to test for empty cells instead of the ISBLANK function. For example, to test if A1 is empty, you can use:<br>
```
= A1 = ""
```

>-This syntax can be used interchangeably with ISBLANK.<br>
![image](https://github.com/ralphgrm/MIDTERM_GROUP_9/assets/134179620/8749b6c4-3c8b-4712-8b9e-f1d4fa894c37)


<b>COUNTIF Function</b><br>
>-The **COUNTIF** function in Excel is used to count the number of cells in a range that meet a certain criterion ¹²³. The syntax for the function is as follows: <br>
```
=COUNTIF(range, criteria)
```

>-Here, `range` is the range of cells that you want to count, and `criteria` is the condition that must be met for a cell to be counted. The `criteria` can be a number, expression, cell reference, or text string. <br>
-For example, if you have a list of numbers in cells A1 through A10 and you want to count how many of them are greater than 5, you can use the following formula:<br>
```
=COUNTIF(A1:A10, ">5")
```

>-This formula will return the number of cells in the range A1:A10 that contain a value greater than 5.<br>
-You can also use wildcards with the COUNTIF function. For example, if you have a list of names in cells A1 through A10 and you want to count how many of them start with the letter "J", you can use the following formula:<br>
```
=COUNTIF(A1:A10, "J*")
```

>-This formula will return the number of cells in the range A1:A10 that start with the letter "J".<br>
![image](https://github.com/ralphgrm/MIDTERM_GROUP_9/assets/134179620/84d063d5-24fe-4117-84d1-cf66b612b1b4)


# LOOKUP FUNCTION
<b>LOOKUP Function</b><br>
>-The **LOOKUP** function in Excel is used to look up information in a row or column. It is one of the lookup and reference functions in Excel ¹. There are two ways to use the LOOKUP function: vector form and array form. <br>
-The vector form of the LOOKUP function searches only one row or column for a value and returns a value from the same position in a second one-row or one-column range. The syntax for the vector form of the LOOKUP function is as follows:<br>

```
=LOOKUP(lookup_value, lookup_vector, [result_vector])
```

>-Here, `lookup_value` is the value that you want to search for in the first vector. `lookup_vector` is the range that contains only one row or one column. The values in `lookup_vector` can be text, numbers, or logical values. The values in `lookup_vector` must be placed in ascending order; otherwise, LOOKUP might not return the correct value ². `result_vector` is an optional argument that specifies a range that contains only one row or column. The `result_vector` argument must be the same size as `lookup_vector`. If you omit this argument, the function returns the result from `lookup_vector`.<br>
-The array form of the LOOKUP function searches multiple rows and columns for a value and returns a value from the same position in a second range of cells. The syntax for the array form of the LOOKUP function is as follows:<br>

```
=LOOKUP(lookup_value, lookup_array)
```

>-Here, `lookup_value` is the value that you want to search for in the array. `lookup_array` is an array of cells that contains the data you want to search. The data must be sorted in ascending order for this form of LOOKUP to work correctly.<br>
![image](https://github.com/ralphgrm/MIDTERM_GROUP_9/assets/134179620/ba373c14-b4cd-4332-8c39-8be7f8e3f837)


<b>MATCH Function</b><br>
>-The **MATCH** function in Excel is used to locate the position of a lookup value in a row, column, or table and returns the relative position of an item in an array that matches a specified value in a specified order. The syntax for the function is as follows:

```
=MATCH(lookup_value, lookup_array, [match_type])
```

>-Here, `lookup_value` is the value that you want to match in `lookup_array`. `lookup_array` is the range of cells being searched. `match_type` is an optional argument that specifies how Excel matches `lookup_value` with values in `lookup_array`. The default value for this argument is 1.
-The following table describes how the function finds values based on the setting of the `match_type` argument:

| **Match Type** | **Behavior** |
|----------------|--------------|
| 1 or omitted    | MATCH finds the largest value that is less than or equal to `lookup_value`. The values in the `lookup_array` argument must be placed in ascending order. |
| 0              | MATCH finds the first value that is exactly equal to `lookup_value`. The values in the `lookup_array` argument can be in any order. |
| -1             | MATCH finds the smallest value that is greater than or equal to `lookup_value`. The values in the `lookup_array` argument must be placed in descending order. |

>-The function returns the relative position of the matched value within `lookup_array`, not the value itself ². For example, if you have a list of numbers in cells A1 through A5 and you want to find the position of the number 3, you can use the following formula:

```
=MATCH(3,A1:A5,0)
```

>-This formula will return 3 because 3 is located at position 3 within the range A1:A5.
![image](https://github.com/ralphgrm/MIDTERM_GROUP_9/assets/134179620/5707f70c-98da-4320-a9b4-b704a87ba046)


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
>
># MATH FUNCTION
<b>ABS Function</b><br>
>-The ***ABS*** function in Excel is used to calculate the absolute value of a number. The absolute value of a number is its distance from zero on the number line, regardless of whether the number is positive or negative. In other words, it returns the positive value of a number.<br>
-The syntax for the function is as follows: <br>
```
=ABS(number)
```
<br>

<b>SIGN Function</b><br>
>-The ***SIGN*** function in Excel is used to determine the sign of a number. It returns the following results:<br>
>If the number is positive, it returns 1.<br>
>If the number is negative, it returns -1.<br>
>If the number is zero, it returns 0.<br>
-The syntax for the function is as follows: <br>
```
=SIGN(number)
```
<br>

<b>ABS Function</b><br>
>-The ***SUM*** function in Excel is used to add up a range of numbers. It calculates the total sum of values in a selected range of cells.<br>
-The syntax for the function is as follows: <br>
```
=SUM(number1, number2, ...)
```
<br>

***Table Used***
>![image](https://github.com/DMBysnGnzls/MIDTERM_GROUP_9/assets/143982031/cccc2ea2-351d-4cac-a643-ed708d059c51)
<br>

***ABS, SIGN, AND SUM Function in one table***
>![image](https://github.com/DMBysnGnzls/MIDTERM_GROUP_9/assets/143982031/df731e94-13e6-40a1-9488-d35ab5fa9be3)

># INFORMATION FUNCTION
<b>TYPE Function</b><br>
>-***TYPE*** function is used to determine the type of data in a cell. It returns a number that corresponds to the data type of the cell's content. <br>
-The syntax for the function is as follows: <br>
```
=TYPE(value)
```
<br>

<b>ISNUMBER Function</b><br>
>-***ISNUMBER*** function is used to check if a value is a numeric (number) data type. It returns ***TRUE*** if the specified value is a number and ***FALSE*** if it is not. <br>
-The syntax for the function is as follows: <br>
```
=ISNUMBER(value)
```
<br>

<b>ISODD Function</b><br>
>-***ISODD*** function in Excel is used to determine whether a given number is odd. It checks if a numeric value is an odd number and returns ***TRUE*** if the number is odd, and ***FALSE*** if it's not.<br>
-The syntax for the function is as follows: <br>
```
=ISODD(number)
```
<br>

<b>ISEVEN Function</b><br>
>-***ISEVEN*** function in Excel is used to determine whether a given number is even. It checks if a numeric value is an even number and returns ***TRUE*** if the number is even, and ***FALSE*** if it's not.<br>
-The syntax for the function is as follows: <br>
```
=ISEVEN(number)
```
<br>

***Table Used***
>![image](https://github.com/DMBysnGnzls/MIDTERM_GROUP_9/assets/143982031/ce6b08df-0581-497d-99cd-3200b7fe3ba2)

***TYPE, ISNUMBER, ISODD, AND ISEVEN Function in one table***
>![image](https://github.com/DMBysnGnzls/MIDTERM_GROUP_9/assets/143982031/0bfbadc5-86de-4999-87be-36aca31c025d)

# DASHBOARD
These different dashboards below were all based on the FIFA 21 data set. FIFA 21 is the latest edition of the popular soccer video game series developed by EA Sports. It was released on October 9, 2020 for various platforms, including Microsoft Windows, Nintendo Switch, PlayStation 4, Xbox One, Stadia, PlayStation 5 and Xbox Series X/S.<br>

<b>VALUE PER DATE JOINED</b><br>
>-Shown in this dashboard are the different values of the date when a player joined. Where the oldest year was on 2004, while 2018 was the latest.<br>
![image](https://github.com/ralphgrm/MIDTERM_GROUP_9/assets/134179620/001c808b-c9a9-4aac-89f0-9530371393e6)

<b>VALUE PER POSITION</b><br>
>-Shown in this dashboard are the different values of the position of the players.<br>
![image](https://github.com/ralphgrm/MIDTERM_GROUP_9/assets/134179620/038e1464-8767-4b15-b2f5-cc5f13b96530)

<b>OVERALL PERFORMANCE PER AGE</b><br>
>-Shown in this dashboard are the different overall performances of the players per age. Peaking on high scores of 94 on ages 33 and 31, whereas dipping down to the score of 89 on ages 27, 26, and 24.<br>
-It is to be noted that not all the players with the same age as the ones peaking to its highest score, and dipping on the lowest score, are all the same. Some of them are in middle ground of the lowest and highest scores.<br>
![image](https://github.com/ralphgrm/MIDTERM_GROUP_9/assets/134179620/7785f948-0514-452c-af03-0196e45071d7)

<b>AGE PER POTENTIAL POTENTIAL POINTS</b><br>
>-Shown in this dashboard are the different potential points that can be acquired by the players according to their respective age.br>
![image](https://github.com/ralphgrm/MIDTERM_GROUP_9/assets/134179620/1a9b1438-7a16-47d4-a161-495c8d8b261f)

![image](https://github.com/DMBysnGnzls/MIDTERM_GROUP_9/assets/143982031/c6844735-b751-4a6a-a688-adc55c7cc97b)


# SOURCE/S
Manral, M. (2022, August 14). Sports data analysis. Kaggle. https://www.kaggle.com/datasets/mukeshmanral/fifa-data-for-eda-and-stats?fbclid=IwAR3ca5efEtv0CqAx2sjJ7-vxuyuL_aWd5lnQO6okI9EwRBleq2H1AQJNPx0 
