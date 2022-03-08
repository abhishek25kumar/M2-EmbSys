# TEST PLAN AND OUTPUT

| TEST ID | Test Case Objective | Input Data  | Expected Output |Actual output| Motor Running Status |
| ----- | ----- | ------- | ------- | ------ |------ |  
|TC_01| Temperature less than 20| Temperature | FAN OFF | X | YES |
|TC_02| Temperature greater than 20 less than 40 | Temperature | FAN ON | X | YES|
|TC_03| Temperature greater than 40 less than 60 | Temperature |FAN ON | X | YES|
|TC_04| TEmperature equal to or greater than 60 | Temperature | FAN Speed Max | X |YES|
