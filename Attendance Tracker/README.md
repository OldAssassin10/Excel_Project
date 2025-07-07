In here, I'll give a breakdown of the project's content 

The spreadsheet is an attendance for an organization, used to keep track of employees attendance in meeting which is held on Friday every two weeks.

It includes the following details:
- [Serial Number](#serial-number)
- [First Name](#first-name)
- [Last Name](#last-name)
- [Employee ID](#employee-id)
- [Date](#date)
- [Present](#present)
- [Reason](#reason)

### Serial Number

This is just a series of numbers that I generated to keep based on the entry. You can increase it by using the Fill function in Excel on the last number in the sequence.

### First Name

This is the first name of the employees.

### Last Name

This is the last name of the employees.

### Employee ID

This is a unique identifier for the employees. It is made up of the first two characters from the employee's first name, a number and two characters from the employee's last name. You can automatically fill it by using the Fill function in Excel on the last ID in the sequence.

### Date

This represents the date the meeting held. It can be filled horizontal using the Excel's Fill function (for consistency, copy table cell `H4:J5` and paste at the end of the last date horizontally).

### Present

This signifies if the employee is present or not. It's values are `"Y"` for `"Yes"` and `"N"` for `"No"`.

### Reason

This tells you the reason why an employee was not present during a meeting.
It has two fields:

1. One whose values are: `"PD"`, `"VA"` and `"SL"`, and;
2. The other whose values are: `"Personal Day"`, `"Vacation"` and `"Sick Leave"`

In order to fill these fields, here are the steps needed:
1. Highlight and copy table cells `I6:J6`
2. Highlight and paste in the next corresponding table cells **horizontally**
3. From the newly pasted cells, highlight and fill down to your desired length
4. If done properly, the cells should have either `"-"` or left blank, corresponding with `"Y"` or `"N"`. If any thing other than this is present, refer back to step 1.
5. For the part left blank after step 3, highlight the cell and you'll see this: `=IF(H9="Y", "-", "")` in this `fx` section. In the empty double quotes, `""`, type `"SL"`, `"VA"` or `"PD"` to correspond with their reasons.
