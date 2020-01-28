# FRONTEND SKILS ASSESSMENT PROJECT

For this task you will be creating a **React login single page application**.

**It must be production quality according to your understanding of it: testing, readme.md etc. If there's no instruction how to run the code or/and it doesn't compile, it will NOT QUALIFY**

The application should have the following features:
## Features

##### The application should have a login in two steps:
- first step for *email* field and a 'next' button
	- there should be an email validation
	- the email validation can be done while the user writes it or after trying the 'next' button
	- if the email is valid and the user tries the 'next' button, it should go to the next step
- second step for *password* field
	- for test purposes, if both email and password contains the string 'test' the email and password matches
	- if the password doesn't match it should return a message
	- if the password matches it should redirect to the home page.
	
##### Header:
- It contains a title to the page

##### Footer:
- It contains the current date 
	
##### Home page:
You have the data in the folloing format from https://front-end-clip.free.beeceptor.com/transactions
```json
[
   {
      "user_id":123,
      "date":"2019-11-01",
      "amount":100
   },
   {
      "user_id":123,
      "date":"2019-11-07",
      "amount":100
   }
]
```
You need to agregate it by week, like the table below:

| Id | Week start | Week finish | Quantity | Amount | Total Amount |
| :---: | :---: | :---: | :---: | :---: | :---: |
| 123 | 2019-11-08 Friday | 2019-11-14 Thursday | 2 | 10.00 | 00.00 |
| 123 | 2019-11-25 Friday | 2019-11-21 Thursday | 1 | 20.00 | 10.00 |
| 123 | 2019-11-22 Friday | 2019-11-28 Thursday | 4 | 100.00 | 30.00 |
| 123 | 2019-11-29 Friday | 2019-11-30 **Saturday** | 3 | 50.00 | 130.00 |
| 123 | 2019-12-01 **Sunday** | 2019-12-05 Thursday | 6 | 120.00 | 180.00 |
| 123 | 2019-12-06 Friday | 2019-12-12 Thursday | 3 | 100.00 | 300.00 |

- It always start on Friday and finishes on Thursday, except on the start/end of the Month. In the example the total sum of transactions is 400.00.
- If there's no one single day of transaction for the week, the report should hide the week.
- The user can have no transaction in one day of the week, we still need to show the week.
- To get the transaction data you can use the following endpoint: https://front-end-clip.free.beeceptor.com/transactions

#### Observations:
The stylization doesn't need to be too elaborated, it's allowed to use pre made themes but your CSS should be organized.

## FINAL CONSIDERATIONS
Please write this application in React. You are free to implement this however you’d like with whatever resources or 3rd party code you’d want.

**Deadline**: We expect you to get back to us with the solution in 7 days. It won't be better if you delivery before, so if you finish early, improve your code. Finally, don't rush, if you need more time please ask us whenever you need.

Create a private project in GitHub and share with us your code.

The repo should have your name, for example **"_eric-lee-sample-java-test_"**, it will help us to identify your test.

Feel free to ask questions at any time (eric.lee@payclip.com).
