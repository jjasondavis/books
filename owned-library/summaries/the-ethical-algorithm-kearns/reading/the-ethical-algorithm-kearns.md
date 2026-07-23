<!-- SUMMARY (not the full book) extracted from a summary PDF the owner owns. -->
Source file: the-ethical-algorithm-kearns-en-38001.pdf
Summary of: the-ethical-algorithm-kearns; third-party book summary (getAbstract/ExecSummaries); owned copyright â€” personal use, do not distribute. NOT the book's own words â€” use to locate themes/positions, never quote as the author.

Rating
9

Qualities Scientific Eye Opening Visionary

The Ethical Algorithm
The Science of Socially Aware Algorithm Design
Michael Kearns and Aaron Roth | Oxford UP © 2019
Algorithms decide what ads people see online and whether consumers get loans. These computerexecuted recipes acquire more and more power over humans' lives. Do they wield it fairly? Can humans design algorithms to behave ethically? The message of Michael Kearns and Aaron Roth, computer scientists at the University of Pennsylvania, is yes ­ sometimes. Kearns and Roth explain when humans can expect algorithms to behave ethically, and in what cases computer science still struggles to accomplish this. They detail the conundrums and solutions in accessible language, even if it can be hard to follow along. This book will give you a good sense of when you can expect algorithms to behave ethically, and in what cases computer science still has its work cut out.
Take-Aways
· Algorithms raise questions of privacy, fairness, safety, transparency, accountability and even morality.
· Protecting privacy is hard, but randomness helps. · A more fair algorithm must be less precise. · Algorithms can create games, and games can create algorithms. · Scale and adaptivity make for treacherous algorithms. · Artificial intelligence may be on the road to a "singularity." · Algorithms are fallible, but a world without them is unthinkable.

BatchLoginContext[cu=5482345,asp=3498,subs=0,free=0,lo=en,co=US] 2020-06-12 13:07:14 CEST

www.getabstract.com

Summary
Algorithms raise questions of privacy, fairness, safety, transparency, accountability and even morality.
Companies and governments accumulate vast amounts of data about us. Computers collect and analyze these according to certain algorithms. This leads to valuable insights and helps provide services. But it can also divulge private information. And an algorithm may take or propose decisions about people that they would consider unfair or immoral.
Some approaches use algorithms that process data according to step-by-step instructions. Others use machine learning which allows the system to evolve. Such systems build internal models that are hard to understand for humans. And while processing data according to their rules, these systems may even arrive at solutions that offend social norms.
"An algorithm, after all, is just a human artifact, like a hammer, and who would entertain the idea of an ethical hammer?"
Regulations can help to ensure that systems are used according to their purpose. And when developers design algorithms for a purpose, they're ideally led by the FATE principle: fairness, accuracy, transparency and ethics. However, a successful implementation of FATE can come with a price ­ the resulting algorithms can be less precise or efficient as compared to a design that doesn't follow the principle.
Protecting privacy is hard, but randomness helps.
When a government agency released anonymized medical data of employees for research, an MIT student succeeded in extracting the data of the state's governor, William Weld. It turns out that anonymizing data does not safeguard privacy.
This problem remains even if data fields that can uniquely identify a person remain confidential. Neither is only releasing aggregate data a solution. In both cases, it is often possible to still retrace some information about individuals.
"The world is full of curious correlations, and as machine learning gets more powerful and data sources become more diverse, we are able to learn more and more facts about the world that let us infer information about individuals that they might have wanted to keep private."
To design algorithms that safeguard privacy, it is useful to define the concept in terms of harm. Privacy is preserved if a person isn't disadvantaged if his or her data appear in a published data set. This can be achieved through so-called differential privacy. Algorithms can provide this kind of privacy by randomizing some of the data. But differential privacy comes at a cost: The more

BatchLoginContext[cu=5482345,asp=3498,subs=0,free=0,lo=en,co=US] 2020-06-12 13:07:14 CEST

www.getabstract.com 2 of 7

privacy it provides, the more data companies or researchers will have to collect to draw reliable conclusions.
Both Google and Apple make use of this method. Their software mixes information they collect from each device with arbitrary data, which means their users do not have to trust them with their private information. This is the local model of privacy. The US Census Bureau will use differential privacy for the 2020 census. It will gather exact data, but randomize them afterwards ­ the centralized model of privacy.
Differential privacy cannot protect information that belongs to large groups of people. In 2017, a company that collected information from workout devices such as Fitbits released data on where its users walked or ran, including the locations of military bases in Afghanistan's Helmand province.
Additionally, the desire of many people to know what their DNA says about them made it possible to find family members of a serial killer ­ and then the Golden State Killer himself.
A more fair algorithm must be less precise.
A Google research team in 2016 discovered a case of sexism in the company's own data when an algorithm figured out what words often occurred close to each other in texts. The team summarized it in the title of a journal article: "Man is to Computer Programmer as Woman is to Homemaker?" A similar problem was discovered in a machine learning algorithm of Amazon that selected job applicants: It valued women less. If the data are biased, then the output of the algorithm that learns from the data will be biased, too.
Humans can't prevent an algorithm from producing biased output by striking information about persons from its input. For instance, leaving out race does not mean the algorithm can't accurately guess a person's race, which it bases on other factors such as a zip code. Instead, designers must explicitly demand neutrality on certain criteria. This will diminish accuracy.
"Just as with people, sometimes the failings of algorithms and models are far more revealing and interesting than their strengths."
Different ways to define fairness exist. One is that different groups of people have the same chance of a favorable outcome ­ say, getting a loan. But this is problematic if real differences exist between the groups. In this case, it could be their average creditworthiness. Enforcing such fairness will depress the bank's profits.
Another approach is to require that an algorithm is evenhanded in the mistakes it makes. Members of the two groups should be equally likely to get a loan undeservedly, and equally likely not to get one in spite of good credit. In practice, a tradeoff will occur between the number of mistakes and the desired level of fairness.

BatchLoginContext[cu=5482345,asp=3498,subs=0,free=0,lo=en,co=US] 2020-06-12 13:07:14 CEST

www.getabstract.com 3 of 7

Even more definitions of fairness abound. Mathematicians have proved that it is not possible to satisfy them all at once, so people will have to make the tradeoff and choose the desired fairness type.
Making an algorithm as fair as possible for several large groups may cause them to become unfair to some well-defined small group. To prevent this, algorithms exist that modify themselves in a game, in which a "Learner" tries to maximize the performance of the algorithm, while a "Regulator" proposes subgroups that have to receive fair treatment. But this cannot go so far that it guarantees fairness for a group of one.
Other problems arise if the data are contaminated by bias. In crime statistics, if some areas have more crime, more police will be present and observe even more crime. This is a hard problem to solve by algorithm.
Algorithms can create games, and games can create algorithms.
Algorithms can have problematic results because of people's actions.
In 2013, a journalist using a dating app found she only received offers from Asian males. When she reluctantly changed her preference to not being interested in Asian males, she exacerbated the oversupply, probably inducing other women to face the same dilemma.
Here, the problem is not just the algorithm, but also the way people react to it. This is the province of game theory. Everyone acts in his or her own interest. Often an equilibrium, good or bad, will result. Researchers working in the rapidly evolving field of algorithmic game theory try to design better algorithms for such situations.
An example of such a game is the daily commute by car. Route-finding apps like Waze suggest the fastest route to work or home, taking account of what all the other commuters do. The result is not optimal. An alternative app would send some users via a longer route, which would benefit many people.
People can defeat this "maximum social welfare solution" if they cheat and refuse to sacrifice some driving time for the greater good. At some point, self-driving cars may be forbidden to cheat. Until then, drivers could want to cooperate if they know that the app will select everyone equally often to take a detour. Even better, the algorithm can be designed in such a way that not using it or not obeying it is always a worse option.
"Commuting was a game, but people couldn't play it very well. This is where technology changed everything ­ and, as we shall see, not necessarily for the collective good."
Another context in which algorithm meets game theory is shopping. On the basis of purchases and ratings, it is possible to define user types. Once someone buys something, this information makes

BatchLoginContext[cu=5482345,asp=3498,subs=0,free=0,lo=en,co=US] 2020-06-12 13:07:14 CEST

www.getabstract.com 4 of 7

it possible to recommend additional things to buy. That next purchase then influences the model of the online store again. This may may make shoppers converge to a limited set of products.
That seems harmless, but the same thing can happen when people use social media and read news online. This will lead them into an echo chamber of one-sided information. A solution can be to inject variety. Random information would not be welcome. But algorithms can select information just outside the user's private bubble, or from a totally opposing viewpoint. Algorithms from game theory also work well in matching markets. For instance, they help choose which donor organ should go to which donor recipient to maximize the number of transplants of compatible organs.
Game theory can also help in designing algorithms. This idea got started when researchers gave the rules of a game, such as Go, to a machine learning algorithm and let it play against itself to develop strategic capabilities. In the same way, they can develop algorithms for other purposes. For instance, an algorithm that recognizes pictures of cats gets good at it because an algorithm that generates cat pictures challenges it many times. This approach is also suitable for developing algorithms that adhere to specified ethical standards.
Scale and adaptivity make for treacherous algorithms.
One algorithm may convince people that you know the future. It consists of making random predictions about a stock going up or down to a million people. For half a million people, the prediction will come true. To those, you send another prediction. You end up with about 1,000 people who believe in you. They estimate the probability you were right by chance as tiny. But they didn't know you made use of scale and adaptivity.
This scenario occurs in real life. Hedge funds report good years, but not bad years. Scientists report exciting research, but not boring or negative results. This has led to the announcement of many interesting discoveries that later turned out to be impossible to replicate ­ such as the effect on one's political position of seeing the American flag, or the health effects of wine, chocolate or green tea.
In scientific research, the problem of scale crops up because it is common for scientists to do many experiments and report only the successful ones. They do this both individually and collectively. Researchers will also perform many different statistical tests on their data, and report only the ones that support their hypothesis ­ this practice is known as p-hacking.
One way to correct for the problem of scale is the Bonferroni correction. It says that the probability that a result just came about by luck ­ a number that a researcher would like to be low ­ has to be adjusted to account for the number of experiments that were actually done.
This correction doesn't help for the problem of adaptivity. In scientific research, this problem takes the form of adapting questions about the data on the basis of what scientists observe during analysis. This means that people don't raise many other possible questions.

BatchLoginContext[cu=5482345,asp=3498,subs=0,free=0,lo=en,co=US] 2020-06-12 13:07:14 CEST

www.getabstract.com 5 of 7

"If you torture the data long enough, it will confess to anything." ­ Ronald Coase, Nobel Prize-winning economist
The decisions that scientists take while performing research can be like taking a fork in a path. According to statisticians Andrew Gelman and Eric Loken, scientists work in a "garden of the forking paths." Getting lost in it will produce research that may not be reproducible. In preclinical medical research, this waste is approximately worth more than $28 billion per year.
One way to prevent such false discoveries is requiring the preregistration of each study. During data analysis, nothing in the approach can change. But in practice, this is too strict. Scientists often work with the same data sets that formed the foundation of earlier research. And they ask questions that they base on previous research on that data, so they are already somewhere in the garden of forked paths.
Researchers are developing algorithms that sit between scientists and their data, and limit their freedom to choose a path. Interestingly, algorithms that implement differential privacy turn out to be very useful in this context.
Artificial intelligence may be on the road to a "singularity."
Humans would like to see more qualities in algorithms, but have not been able to flesh them out as much.
One is transparency: If humans can understand the models of data that algorithms build, humans can trust them. But to whom should the algorithm be "interpretable" ­ to experts, or to people with little machine learning background? Should humans focus on the data, the algorithm, the model, or the decisions that the model makes? It is possible that a model humans can't understand will make decisions that they do understand.
Ideally, algorithms should also behave morally ­ for instance, when a self-driving car ends up in a traffic situation where someone is going to die, and it has to decide who it will be. The Moral Machine project of MIT asks people about such dilemmas to learn how they would like machines to act.
It is also possible that humans will decide that algorithms should never make some decisions, in the same way that the philosopher Michael Sandel has argued that some things exist that markets can't regulate.
"Maybe the fundamental nature of decisions can change when an algorithm makes them instead of a person."
Finally, some people fear that algorithms that implement artificial intelligence are a threat. They could create better algorithms, which will create even better ones. Soon, a singularity will occur, and machines will rule humans.
www.getabstract.com 6 of 7
BatchLoginContext[cu=5482345,asp=3498,subs=0,free=0,lo=en,co=US] 2020-06-12 13:07:14 CEST

If such a supreme intelligence were to arise, it would indeed be dangerous. It is impossible to predict how it would behave. Counteracting it may be difficult. It might not allow humans to pull the plug ­ if not out of a will to live, then just because this would interfere with some goal. And it is not clear that humans could guarantee that its goal would always conform with their values.
The doomsday scenarios might be too dark. According to AI expert Andrew Ng, it is just as useful to worry about the overpopulation of Mars. It might happen, but only in the very distant future. One reason could be that progress in many things tends to slow down. But it is a serious idea. After all, algorithms keep surprising.
Algorithms are fallible, but a world without them is unthinkable. People can't escape algorithms. Even without computers, they use them to make decisions. Preferably, algorithms should be precise. And people would be giving up much if they abandoned the use of machine learning.
Regulation of algorithms is important, but human oversight will not be able to keep up with the scale and speed of decision-making by algorithms. Algorithmic research should solve the problems that algorithmic decision-making introduces. It should also identify the extent to which it can meet the demands that humans would like to make of it.
While research into algorithms is ongoing, decisions that humans make according to algorithms sometimes cause injustice in the real world. Maybe algorithms in many domains are too naive and primitive. But this is no reason to stop research into algorithms, or to doubt ethical algorithms' great promise.
About the Authors
Michael Kearns, PhD, is a professor of computer and information science at the University of Pennsylvania. He has worked in machine learning and artificial intelligence research at AT&T Bell Labs.
Aaron Roth, PhD, is an associate professor of computer and information science at the University of Pennsylvania.
Did you like this summary? Buy book or audiobook http://getab.li/38001
This document is restricted to the personal use of Jason Davis (jason.s.davis@accenture.com) getAbstract maintains complete editorial responsibility for all parts of this review. All rights reserved. No part of this review may be reproduced or transmitted in any form or by any means ­ electronic, photocopying or otherwise ­ without prior written permission of getAbstract AG (Switzerland).
7 of 7
BatchLoginContext[cu=5482345,asp=3498,subs=0,free=0,lo=en,co=US] 2020-06-12 13:07:14 CEST


