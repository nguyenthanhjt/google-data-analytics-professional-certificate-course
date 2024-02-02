# When you get stuck

Video transcript

- Hi there.
- Data analysts spend a lot of time problem-solving, and that means there's going to be times when you get stuck, but the trick is knowing what to do when that happens.
- In this video, we'll talk about the importance of knowing how to get help, whether that means asking someone else for help or searching the internet for answers.
- Asking other people about a problem you're having can help you find new solutions that move a project forward.
- It's always a good idea to reach out to your peers and mentors, especially if they're working with you on that project.
- Your team members have valuable knowledge and insight that can help you find the solution you need to get unstuck.
- Sometimes we spend a lot of time spinning our wheels saying, "I can do this myself," but we can be way more productive if we engage with other people, find new resources to lean on and try to get as many voices as we can involved.
- For example, let's say you're working with the bike trip time data from the previous videos.
- Maybe you're trying to find the average time between bike rides in a given month.
- Calculating the difference between bike rides before midnight is easy, but you can run into a problem if the elapsed time crosses into the next day.
- If someone went on a bike ride at 11:00 PM, but the next ride wasn't until 06:00 AM, your formula would return a negative number because the end time is less than the start time.
- You know that you can add one minus the start time if two bike rides start and end on different days, but that formula won't work on times that happened in the same day, and it's pretty inefficient to scroll through every bike ride to pinpoint these special cases.
- You need to find a way to build a conditional formula, but you aren't sure how.
- You decide to check in with other analysts working on your team to see if they have any ideas.
- You could send them a quick email, or stop by their desk, to find out if they have a minute to talk it over with you.
- Turns out they had a similar problem on a previous project, and they're able to show you a conditional formula that you could use to speed up your calculations.
- Great! They suggest using an IF formula like this.
- This basically says that, "if the end time is larger than the start time, replace the standard end time minus start time formula with one minus start time plus end time." Now it's also possible that your team members don't have an answer; that's okay too.
- There's definitely someone else with the same problem asking the same questions online.
- Knowing how to find solutions online is an incredibly valuable problem-solving tool for data analysis.
- There's also all kinds of forums where spreadsheet users can ask questions, and you never know what you can turn up with just a basic search.
- For example, let's say you look at "calculate number of hours between times" spreadsheets and find a helpful walk-through for a more complicated formula using MOD.
- This flips the negative values into positive ones, solving your calculation problem.
- Whether you're asking someone you know or searching the internet for answers, reaching out for help can give you some really interesting solutions and new ways to solve problems for future analysis.
- Coming up, we'll learn even more about searching for solutions online.
- See you soon.

## Notes

**Note**: If the units of measurement in the timestamp columns are expressed in hours, adding 1 (day) to the formula would incorrectly calculate the results as a negative value, thus causing an error in the cell. 

**Update**: Since 1 day = 24 hours, you could substitute the number "24" to satisfy the following statement:

Add 24 minus the start time to the formula that's being used for the multi-day trip; then try to apply to another trip that happened in the same day.

### Updated Formula

As a result of the different units of measurement as described in the last pop-up, the following formula would calculate the correct solution:

- `=IF(end>start, end-start, 24+end-start)`
- `MOD(end-start,1)`

## Key Points

- Importance of Seeking Help: Data analysis often involves complex problems, and getting stuck is natural. Knowing how to seek help is crucial.
- Utilizing Peer and Team Support: Your peers and team members can offer valuable insights and solutions. Don't hesitate to reach out to them for assistance, especially if they are working on the same project.
- Efficiency Through Collaboration: Collaborating with others can lead to faster problem-solving and innovative solutions. Engaging with multiple voices can offer different perspectives and approaches.
- Example Scenario: Using a bike trip data analysis scenario, the video illustrates how seeking help can resolve challenges efficiently. In this scenario, dealing with time calculations across different days requires a conditional formula, which can be efficiently solved with input from peers.
- Online Resources: Online platforms and forums are rich sources of information and solutions. Searching for similar problems online can yield helpful tutorials, walk-throughs, and discussions.
