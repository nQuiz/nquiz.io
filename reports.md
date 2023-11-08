# Reports

Although all questions go through a [review](/review.md) process prior to release, it is possible that a bad question makes it into the question bank.  We therefore have a "report this question" link that allows a player to submit a description (>50 chars) explaining what is wrong with the question, and how it could be fixed.  This is submitted anonymously and shown only to the question creator (in the SUBMIT screen and via a DM notification).

Who can really say though if a question is objectively good or bad? Or if the person reviewing is right or wrong?

It's a difficult call, and so we make the judgement through an algorithm that takes into account the question quality (number of zaps) and the reviewer quality (amount of reputation). This results in a score, and if the score exceeds a threshold, the question is returned to the creator to be revised.

The algorithm is as follows:

`avZaps` = the average number of zaps received per question, or 1, whichever is higher. Calculated daily.
`avRep` = the average amount of reputation per user, or 1, whichever is higher.  Calculated daily.
`qZaps` = number of unique players who have zapped the question revision at the time the report is made
`pRep` = reputation of the player making the report at the time the report is made

The `reportScore` of one report against a question revision is calculated as:  `qZaps/avZaps + pRep/avRep`.  Players may only submit one report per revision.

When the sum of the reports on that question revision exceeds a threshold of `21` the question is removed from the question bank and the creator is notified.  The question must then be adjusted, and resubmitted to the [review](/review.md) process.

