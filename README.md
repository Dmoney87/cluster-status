# cluster-status

One file, `status.json`: a handful of numbers from the
[Master Cluster](https://mastercluster.ai)'s box, which the site reads so that
its panels say what the journals say rather than what somebody last typed.

It is public because the site is, and it is a separate repository because the
thing that writes it should not be able to write anything else. `beacon`, a
small agent on the box, rebuilds the file from three status files through a
field-by-field allowlist and pushes it here with a deploy key that works on
this repository and no other. It cannot touch the site's code. The worst it
can do is publish a wrong number into a page that renders numbers as text.

What is in it: counts, rates, p-values, Brier scores, the agents' own rule
vocabulary (`no:50-98@+2h~5^15:nbs2`), and ticker symbols that were vetoed,
with the reason. What is not, by construction: balances, order ids, key ids,
market tickers, file paths, and any prose that began on somebody else's web
page.

Nothing here is advice. Most of it is a record of things that did not work.
