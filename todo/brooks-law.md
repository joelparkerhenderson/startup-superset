# Brooks's law

Brooks's law is an observation about software project management according to which "adding manpower to a late software project makes it later".[1][2] It was coined by Fred Brooks in his 1975 book The Mythical Man-Month. According to Brooks, under certain conditions, an incremental person when added to a project makes it take more, not less time.

## Explanations

According to Brooks himself, the law is an "outrageous oversimplification",[1] but it captures the general rule. Brooks points to the main factors that explain why it works this way:

* It takes some time for the people added to a project to become productive. Brooks calls this the "ramp up" time. Software projects are complex engineering endeavors, and new workers on the project must first become educated about the work that has preceded them; this education requires diverting resources already working on the project, temporarily diminishing their productivity while the new workers are not yet contributing meaningfully. Each new worker also needs to integrate with a team composed of several engineers who must educate the new worker in their area of expertise in the code base, day by day. In addition to reducing the contribution of experienced workers (because of the need to train), new workers may even make negative contributions, for example, if they introduce bugs that move the project further from completion.

* Communication overhead increases as the number of people increases. Due to combinatorial explosion, the number of different communication channels increases rapidly with the number of people.[3] Everyone working on the same task needs to keep in sync, so as more people are added they spend more time trying to find out what everyone else is doing.

* Adding more people to a highly divisible task, such as cleaning rooms in a hotel, decreases the overall task duration (up to the point where additional workers get in each other's way). However, other tasks including many specialties in software projects are less divisible; Brooks points out this limited divisibility with another example: while it takes one woman nine months to make one baby, "nine women can't make a baby in one month".

## Exceptions and possible solutions

There are some key points in Brooks's law that allow exceptions and open the door for possible solutions.[4][5]

The first point is to note that Brooks's law only applies to projects that are already late.[6] Projects can be brought back into (or kept in) control if people are added earlier in the process.[7] It is also important to determine if the project is really late, or if the schedule was originally overly optimistic. Scheduling mistakes account for a large number of late projects. Correcting the schedule is the best way to have a meaningful and reliable time frame for the project's completion.[8]

The quantity, quality and role of the people added to the project also must be taken into consideration. One simple way to circumvent the law on an overrun project is to add more people than needed, in such a way that the extra capacity compensates the training and communication overhead.[9] Good programmers or specialists can be added with less overhead for training.[10] People can be added to do other tasks related with the project, for example, quality assurance or documentation; given that the task is clear, ramp up time is minimized.[11]

Good segmentation helps by minimizing the communication overhead between team members. Smaller sub-problems are solved by a smaller team, and a top-level team is responsible for systems integration. For this method to work, the segmentation of the problem must be done correctly in the first place; if done incorrectly, this can make the problem worse, not better, by impeding communication between programmers working on parts of the problem which are actually closely coupled, even when the project plan has decreed that they are not.

An example of segmentation are design patterns that simplify the distribution of work, because the entire team can do its part within the framework provided by that pattern. The design pattern defines the rules that the programmers follow, simplifies communication through the use of a standard language, and provides consistency and scalability.

The Bermuda plan, where most developers on a project are removed ("sent to Bermuda") and the remaining are left to complete the software, has been suggested as a way of circumventing Brooks’s law.[12]

