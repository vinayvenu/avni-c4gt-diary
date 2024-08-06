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
- Working of XRays 
- Visualizations in Metabase

#### Challenges, victories and defeats
- Had to find out how XRays worked, no formal documentation was available!
- Wasn't able to enroll people into programs in Avni!
- PR [link](https://github.com/avniproject/avni-server/pull/734/commits/c0a35e78b71e4f3f1e7e2e8c298eac4a691f2ee3?notification_referrer_id=NT_kwDOBufzr7UxMDg5Njc1MTI4MToxMTU4NjQ0OTU](https://github.com/avniproject/avni-server/pull/734))

### Week 4 (02/07/2024 - 08/07/2024)
This week was about building sample dashboards manually via UI! 

#### New moves learnt
- N.A.
  
#### Challenges, victories and defeats
- Created a dashboard and it was  reviewed,the stats which was not very useful/which would bloat up the screen was removed
- The second dashboard is yet to be reviewed

### Week 5 (09/07/2024 - 15/07/2024)
This week I figured out which tables in OpenCHS need to be used to proceed ahead in our goal! 

#### New moves learnt
- Learnt about schemas in Databases
  
#### Challenges, victories and defeats
- Wasn't able to find the user schema tables in Avni DB
- Had to setup Avni ETL on my machine , and run it in order to get those tables!

### Week 6 (16/07/2024 - 22/07/2024)
This week I started creating the API to automate the creation of questions in Metabase!

#### New moves learnt
- Object Mapper class in Jackson
  
#### Challenges, victories and defeats
- I wrote down the code to automate the questions but strangely it wasn't yielding correct response each and every time.
- I figured out that the API response isn't the expected one each time
- Couldnt complete the code, the perfect working code is yet to be written!

### Week 7 (23/07/2024 - 29/07/2024)
Questions creation has been automated successfully finally(for "subject types" + "Address" currently)!

#### New moves learnt
- TimeUnit
  
#### Challenges, victories and defeats
- I was not able to find out why sending a POST req from POSTMAN yields the correct response but doing the same from code didnt yield the same expected output.
- Finally after investing a lot of time I realized database sync needs to complete before info related to it can be extracted.
- Therefore I implemented code to wait for sync to complete

### Week 8 (30/07/2024 - 05/08/2024)
Questions creation has been automated successfully finally(for "Programs" + "Address", "Program Encounters" + "Address" currently)!

#### New moves learnt
- PostConstruct
  
#### Challenges, victories and defeats
- Successfully used the fucntions and APIs created in last week to proceed ahead!




