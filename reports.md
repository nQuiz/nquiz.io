# Reports

Although all questions go through a [review](/review.md) process prior to release, it is possible that a bad question makes it into the question bank.

Who is to say though if a question is good or bad? Or if the review itself was justified, or made without an objective reason?

It's a difficult call, and so we make the judgement through an algorithm that takes into account the question quality (number of zaps) and the reviewer quality (amount of reputation). This results in a score, and if the score exceeds a threshold, the question is returned to the creator to be revised.

The algorithm is as follows:

zaps = number of unique players who have zapped the question revision at the time the report is made
rep = reputation of the user making the report at the time the report is made
weight = the amount contributed by each report event to a particular question revision.

`weight = zaps/50 + rep/5000`

The threshold is set initially to `0.9`

When making a report, the reporter must provide a description (>50 chars) explaining why the question is being reported and how it could be fixed.  This is submitted anonymously and shown only to the question creator (in the SUBMIT screen and via a DM notification).
