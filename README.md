# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident that you know how the function works.
* Write a summary of what the function does.

*SUMMARY*
1) The function takes some input `user` which must be an object that contains `username: " "`, and `isActive: true` or `isActive: false`.
2) If the user has an active subscription, they are greeted with their username. If the user does not have an active subscription, the function uses their username to ask if they would like to renew their subscription. 

```js
function (user){
  if (user.isActive){
    return `Welcome back, ${user.username}!`
  } else {
    return `Hey ${user.username}! Would you like to renew your subscription?`
  }
}
```

Inputs and outputs should be valid JavaScript values!

| Input | Output |
| ----- | ------ |
| user.Kristofer = {isActive: true, username: "Kristoffzz"}; |  Welcome back, Kristoffzz!      | 
| user.Joseph = {isActive: false, username: "Joey is Here"}; |   Hey Joey is Here! Would you like to renew your subscription? | 
| user.Agile = {isActive: true, username: "Real_Agile"};     | Welcome back, Real_Agile!       | 

<table>
  <tr>
    <th>What does this program do?</th>
    <td>This program detects if a user has an active subscription or not and greets them accordingly. </td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible
