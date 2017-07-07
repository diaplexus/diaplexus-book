### Functional Scoping

This is the notion that functionality useful for problem X may limit or completely impede the solution to problem Y despite X and Y sharing a very similar problem statement. If a program was designed to observe functional scopes, it may have togglable feature sets that vastly improve the performance and experience for both problem X and problem Y.

For instance, a classic scaling problem:

1. I want to sort one thousand rows.
2. I want to sort one billion rows.
3. I want to sort one million by one billion rows.

Each of these problems have been effectively "solved" such that we've found a solution that operates within the human attention span for the current resources of computers. Yet the solution proximity between these problems is quite large such that moving from one to the next is an insurmountable task for a large percentage of people that have problem \#1 and maybe graduate to problem \#2, or from \#2 to \#3.

The solutions currently sound something like this:

1. Usually trivial even for the most bloated, featureful, or inefficient implementations of a table.
2. Requires a lightweight table implementation and "clever" sorting algorithms that make efficient use of memory.
3. Requires a cluster of computers preconfigured to receive orchestrated map reduce tasks.
4. ...? A fully modular global compute system that can be democratically time shared to solve problem X within an acceptable and predictable time span without exterminating the species if off by an order of magnitude?

Let's look at Excel as an example. Excel is very intuitive for a large class of problems that benefit from both a unique visual layout and the clear visualization of the intermediate calculations of the model. It's also very useful for quickly slicing and understanding fairly small tables of data.

There are two very common ways that Excel's utility starts to break down.

The first is when Excel is used to build some kind of model with a time dimension that causes the repetition of calculations many times over. In this situation, the user inevitably ends up making changes to the model and having to update potentially hundreds of formulas in cells to update the model. The formulas get out of sync and Excel becomes opaque to visualizing which cells are being calculated by which versions of the model. This is solved in other paradigms with a more obvious usage of the DRY principle.

The second is the scaling problem above. Even within Excel's hard defined bounds of 1,048,576 rows by 16,384 columns, its functionality quickly begins to impede its usefulness due to the performance of the application becoming too slow and performing outside of the user's attention span. Now we're loading data into Python's pandas package and slicing the data in a leaner and more efficient implementation of a table, because Excel has been trying to sort for 15 minutes.

Now, what if there was a graceful way for the user to disable functionality that did not pertain to the billion row problem, or better yet, the application was carefully designed to have preconfigured functional scopes that were relevant to the scale of the problem.

"I still want to filter, but coloring and styling individual cells, or even rows, for a billion row dataset is no longer useful."

There have been several attempts to embed Python within Excel as an escape hatch to more elegant solutions for larger and more complex problems. Is it really the case that adding an entirely unrelated lineage of programming inside of another is the most efficient means of handling these functional scopes for similar classes of problems?

Even attempts to clone Excel and challenge its market dominance have seemingly failed, possibly due to not cleanly addressing its functional scopes and building a lesser, almost feature of feature product, that does not elegantly implement the feature set important to 99% of Excel users.

We seem to be engaged in some kind of large scale technological evolution where all feature sets required for a problem are reimplemented in various combinations until a clear metaphor for the atomic parts emerges and sticks in the collective consciousness. Maybe once we have the solution as parts in a hundred different languages, we can construct an implementation with compatible components and a graceful increase of complexity.

