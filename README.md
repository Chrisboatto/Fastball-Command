# Fastball-Command

**Fastball Command**

Fastball command is a major factor that is analyzed to evaluate a pitcher. The pitch that is meant to be thrown in the strike zone the most is the fastball, including both two seam and four seam. Pitchers that can command their fastball within the strike zone will have their secondary pitches become much more effective. Being able to know your fastball’s trajectory and placement consistently would allow a pitcher to determine where to start their off-speed pitches to create the illusion of a fastball for every pitch. The vast majority of pitchers pitch off their fastball and need to establish their fastball early in the game to have success.



With the fastballcommand.xlsx data set, I used the Random Forest multivariate model to develop a predictive score for each observation. I used ‘Strikes’ as a predictive attribute because I am trying to predict which pitcher is able to most frequently throw his fastball in the strike zone. Random Forest is a multivariate mathematical model that creates multiple decision trees simultaneously to predict an outcome. It produces many trees to avoid error bias. For this reason, I decided to use the Random Forest model as opposed to another model like Gradient Boosting which grows each tree one by one and then takes the average result of all trees. Growing each tree simultaneously would give a better understanding of the predicted score than the average of each tree individually. I also did not want to create only one tree using a Decision Tree model because it can be biased whereas using multiple trees, or an entire forest, would remove the bias issue



The tree below is a depiction of the 100th tree in the “command_tuned_model”. It shows the flow in which the model made its decision to determine the predictive score of a strike. The model makes a binary decision at each node or parameter, “Yes” or “No”, which then leads to another and another until you reach a final predictive score grouping at the bottom.

![Image of Decision Tree](https://raw.githubusercontent.com/Chrisboatto/Fastball-Command/main/Decision%20Tree.png)


If you're interested in the project, download the data set and run my RMD file. All graphs and results will show within the file. You will then be able to cross reference them to their respective graphs labeled as such in this repository
