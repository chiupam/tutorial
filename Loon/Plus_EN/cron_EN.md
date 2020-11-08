# cron expression

By modifying the cron expression, execute the script regularly

## Learn the basic writing of cron expressions

1, cron 6-digit expression

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/cron_6.png)

-From left to right

  -The first digit represents `seconds`, only numbers between `0-59` are allowed
  
  -The second digit represents `minutes`, only numbers between `0-59` are allowed, and `60` is not allowed
  
  -The third digit represents `hour`, only numbers between `0-23` are allowed, and `24` is not allowed at 12 o'clock in the morning
  
  -The fourth digit represents `Day`, only numbers between `1-31` are allowed
  
  -The fifth digit represents `month`, only numbers between `1-12` are allowed
  
  -The sixth digit represents `week`, only numbers between `0-7` are allowed, `0` and `7` both represent Sunday
  
2. Cron 5-digit expression

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Plus/cron_5.png)

-From left to right
  
  -The first digit represents `minutes`, only numbers between `0-59` are allowed, and `60` is not allowed
  
  -The second digit stands for `hour`, only numbers between `0-23` are allowed, and `24` is not allowed at 12 o'clock in the morning
  
  -The third digit represents `Day`, only numbers between `1-31` are allowed
  
  -The fourth digit represents `month`, only numbers between `1-12` are allowed
  
  -The fifth digit represents `week`, only numbers between `0-7` are allowed, `0` and `7` both represent Sunday
  
3. Special characters

-`,` stands for `and `, such as `0 0,12,18 * * *` means `execute once every day at 0 o'clock, 12 o'clock, and 18 o'clock)

-`*` stands for `any value`, such as `* * * * *` stands for `execute every minute`

-`/` stands for `every`, such as `10-20/5 * * * *` stands for the 10th-20th minute of every hour, which is executed every 5 minutes, namely the 10th minute, 15th minute, and 20th minute Minutes`

  -Special case: you can omit `/1` when you want to express that it will be executed every 1 minute

4. Error demonstration

-`60 * * * * *` Ideal: Execute once every 60th second of every minute. Actual: Unable to execute. Reason: `60` is not allowed in the `second` bit. Correct expression: `0 * * * * *`

-`* 12-18 * * *` Ideal: It will be executed once every day from 12:18 to 0:00. Actual: It will be executed every 1 minute from 12 am to 18 am every day. Reason: The first place is `*`. Correct expression: `0 12-18 * * *`

  -`* 12-18 * * *` Reasons for listing: classic demonstration by group friends, collective blindness series

-`0 18-12 * * *` Ideal: It will be executed once every day from 18:00 to 12:00 the next day at the 0 minute. Actual: Unable to execute. Reason: The time scale cannot be crossed. Correct expression: `0 18-23,0-12 * * *`

-`*/90 * * * * *` Ideal: it will be executed every 90 seconds. Actual: It is executed every 60 seconds. Reason: `Second` is only `60`, when it is greater than `60`, it will be calculated as `60`. Correct expression: currently unable to do it, recommend the curve to save the country

# Reference

-[crontab execution time calculation-online tool](https://tool.lu/crontab/)