# APIGW-Timestamp

## Description

Often when doing custom logging or event notification, you will want to use timestamps. This is a sample policy that shows a few ways to grab different timestamps and formats for use within these audits, logs, or alerts.

##  Timestamp Policy

This policy was built with the intent of being a framework for utilizing Apache Daffodil within the Axway API Gateway.

- ***Get Current Time in Javascript and Set to current.time Variable:*** This Javascript filter grabs the current time as a formatted output and sets it to a variable that it then returns for use within the policy.

- ***Get Epoch Time in Javascript and Set to epoch.time Variable:*** This Javascript filter grabs the current epoch time and sets it in a variable to be returned to policy.

- ***Get Formatted Time from Command Line and Set Linux Formatted Time to linuxFormTime Variable:*** This pair of Command Execution and Set Attribute filters grab the formatted date via the command line from the underlying Linux OS and saves the execution output to a variable for later use.

- ***Get Epoch Time Linux Command Line and Set Linux Epoch Time to linuxEpochTime Variable:*** This pair of Command Execution and Set Attribute filters grab the epoch time via the command line of the underlying Linux OS and saves the execution output to a variable for later use.

- ***Set Sample Response to Show Variable Outputs and Reflect:*** This simple sets a message with the variable outputs so that you can hit the policy and see the results to determine how you might use it later.

For questions or comments: dwille@axway.com
