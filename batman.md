# Batman

## Quest
- Integrate with Metabase

## Milestones
- Create a working API for Metabase in Avni Server
- Develop UI for the Admin
- Setup Dashboard with Stats on Metabase
- Define and implement all tandard dashboards that can be created on Metabase

## Progress

### Week 1 (11/06/2024 - 17/06/2024)

A working API for Metabase was built in the week before this.<br>
But the code did not follow good coding practises.<br>
For example the famous DRY principle was being violated.<br>
So this week was basically about refactoring the code so that it adheres to the benchmarks of a good code base!

#### New moves learnt
- DRY
- Code Smell
- Primitive Obsession
- Generic Method

#### Challenges, victories and defeats
- Commit [link](https://github.com/avniproject/avni-server/pull/734/commits/6f304c46fcabc12a38338c85bd1912f5eca3981b)
- Still some code smell and primitive obsesion is left to be removed which will be removed in Week2!

### Week 2 (18/06/2024 - 24/06/2024)
Although this week was also mainly about refactoring the code<br>
But a major chunk of it also went into resolving the errors caused due to some bad changes in last commit.<br>
It took me more than expected time to find and resolve the bug in Groups(Earlier PermissionsGroup).
Also the MetabaseRepository was broken down into smaller and specific parts this week!

#### New moves learnt
- Got to know about debugging at different levels
- Got a feel of OOPs like how we break down into smaller components


#### Challenges, victories and defeats
- Had to debug and find where was problem in PermissionsGroup logic ,was able to fix it!
- Had to reduce down the MetabaseRepository into smaller and specific components ,was able to do that!
- Still some primitive obsession left to be fixed. I am still using Map<> for the graph of permissions
- Commit [link](https://github.com/avniproject/avni-server/pull/734/commits/c0a35e78b71e4f3f1e7e2e8c298eac4a691f2ee3?notification_referrer_id=NT_kwDOBufzr7UxMDg5Njc1MTI4MToxMTU4NjQ0OTU)

### Week 3 (25/06/2024 - 01/07/2024)
In the very beginning of the week the code I had written until now , which automated the setup of DB,Group,Collection,Permissions , got merged into the main code base.
Besides this , the week was basically about researching how XRays work , how visualizations are made with questions  in Metabase.
Also a sample Dashboard was made by adding data for about 20 people in Avni (but couldnt enroll them into programs as the option wasnt showing up! )

#### New moves learnt
- XRays working 
- Visualizations in Metabase

#### Challenges, victories and defeats
- Had to find out how XRays worked, no formal documentation was available!
- Wasn't able to enroll people into programs in Avni!
- PR [link]([https://github.com/avniproject/avni-server/pull/734/commits/c0a35e78b71e4f3f1e7e2e8c298eac4a691f2ee3?notification_referrer_id=NT_kwDOBufzr7UxMDg5Njc1MTI4MToxMTU4NjQ0OTU](https://github.com/avniproject/avni-server/pull/734))


