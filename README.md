# Ex03 Time Table
# Date:
# AIM
To write a html webpage page to display your slot timetable.

# ALGORITHM
## STEP 1
Create a Django-admin Interface.

## STEP 2
Create a static folder and inert HTML code.

## STEP 3
Create a simple table using `<table>` tag in html.

## STEP 4
Add header row using `<th>` tag.

## STEP 5
Add your timetable using `<td>` tag.

## STEP 6
Execute the program using runserver command.

# PROGRAM
```
{% load static %}
<html>
    <head>
        <style>
            table,th,td{
                margin:auto;
                background-color:rgb(31, 65, 200);
                border-radius: 10px;
            }
            th,td{
                border:solid 3.5px;
                padding:5px;
                align:center;
                margin:auto;
                border-radius:10px;
                border-color: rgb(11, 12, 12);
                color:antiquewhite
            }
            img{
                display:block;
                margin:auto;
                padding-bottom: 50px;
                width:auto;
            }
            caption{
                font-family: algerian;
                font-size: 50px;
                padding-bottom:50px;
                color:rgb(27, 9, 102);
                text-shadow: inset(0,0,10px);
            }
            .mine{
                writing-mode: vertical-rl;
                text-orientation:upright;
                align:center;
                margin:auto;
            }
            th{
                color:rgb(99, 243, 195);
            }
            .jolt{
                margin:auto;
            }
        </style>
    </head>
    <body bgcolor="aqua">
        <img src="{% static 'logo.png' %}">
        <table>
            <caption><u>TIME TABLE</u></caption>
            <tr class="jolt"><th>DAY</th><th>8-10</th><th>10-12</th><th>12-1</th><th>1-3</th><th>3-5</th></tr>
            <tr>
                <td style="color:aquamarine;margin:auto">MONDAY</td>
                <td></td>
                <td>WEB DEVELOPMENT</td>
                <td rowspan="6"><div class="mine">LUNCH</div></td>
                <td>PUBLIC SPEAKING</td>
                <td></td>
            </tr>
            <tr>
                <td style="color:aquamarine;margin:auto">TUESDAY</td>
                <td>WEB DEVELOPMENT</td>
                <td></td>
                <td>WEB DEVELOPMENT</td>
                <td>PUBLIC SPEAKING</td>
            </tr>
            <tr>
                <td style="color:aquamarine;margin:auto">WEDNESDAY</td>
                <td></td>
                <td>C PROGRAMMING</td>
                <td>MENTOR MEET</td>
                <td>C PROGRAMMING</td>
            </tr>
            <tr>
                <td style="color:aquamarine;margin:auto">THURSDAY</td>
                <td colspan="2">C PROGRAMMING</td>
                <td>PUBLIC SPEAKING</td>
                <td></td>
            </tr>
            <tr>
                <td style="color:aquamarine;margin:auto">FRIDAY</td>
                <td>PUBLIC SPEAKING</td>
                <td></td>
                <td>WEB DEVELOPMENT</td>
                <td></td>
            </tr>
            <tr>
                <td style="color:aquamarine;margin:auto">SATURDAY</td>
                <td>WEB DEVELOPMENT</td>
                <td>C PROGRAMMING</td>
                <td colspan="2">PUBLIC SPEAKING</td>
            </tr>
        </table>
    </body>
</html>
```
# OUTPUT
![alt text](<table.html - Google Chrome 29-09-2025 18_42_35.png>)
![alt text](<views.py - ex03 - Visual Studio Code 29-09-2025 18_44_03.png>)
![alt text](<Downloads - File Explorer 29-09-2025 18_43_50.png>)


# RESULT
The program for creating slot timetable using basic HTML tags is executed successfully.
