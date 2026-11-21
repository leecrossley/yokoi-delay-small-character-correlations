# Delayed Yokoi averages with small quadratic twist correlations

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24417504.svg)](https://doi.org/10.5281/zenodo.24417504)

This result is now maintained in [quadratic-mertens-first-crossings](https://github.com/leecrossley/quadratic-mertens-first-crossings/tree/main/results/yokoi-delay-small-character-correlations). This repository is archived and keeps its releases and DOI.

Can a long excess of inert primes be explained by the primes copying the splitting pattern of a second field? In many actual Yokoi fields the excess is larger than every such correlation, even when the comparison field is chosen after seeing the primes.

Let $`d=m^2+4`$ be squarefree with $`m`$ odd. Fix any $`K>0`$. In every sufficiently large discriminant interval $`(D/2,D]`$ at least $`D^{1/2-o(1)}`$ fields have the following property. Their future Mertens average stays positive for every real start from 2 through

```math
 X=2^{\lfloor c_K(\log D/(\log\log D)^2)^{1/3}\rfloor}.
```

At each sufficiently large $`y\le X`$, the absolute weighted correlation with every nonprincipal primitive quadratic character of conductor at most $`y^K`$ is $`O_K(1/\log\log y)`$ times the untwisted prime bias. This includes the characters of 5 and 13. The cutoff exceeds every fixed power of $`\log D`$. The lower bound for the field count is a vanishing fraction of the Yokoi discriminants in the interval. The constants and the threshold on $`D`$ are not computed. It remains open whether positivity through $`d^a`$ for a fixed $`a>0`$ forces a comparable secondary quadratic correlation in genuine fields. The proof uses RH and quadratic Dirichlet GRH, which Alpöge's announced Dirichlet GRH theorem supplies. [Proof](PROOF.md) [Prior work](PRIOR-WORK.md) [Announcement](https://alpo.ge/remark.pdf) [Independent formal checks](https://math.mit.edu/~drew/grh/)

In the field $`d=1543^2+4=2{,}380{,}853`$ the average was previously proved positive through $`d^{9/4}`$. For the complete prime tails at $`y=163`$, multiplying by $`\sqrt y\log y`$ gives values in $`(-1.755,-1.754)`$ without a twist, $`(0.249,0.250)`$ against 5 and $`(-0.013,-0.012)`$ against 13. At the later start $`y=d`$ both secondary tails are larger in magnitude than the untwisted one. Two calculations cover both starts and $`y=3d`$. [Numerical enclosures](CHECKS.md) · [Earlier positive interval](https://github.com/leecrossley/quadratic-mertens-first-crossings/blob/fa7ed4741f735e37fc3552f497952a57f02cbaa2/results/fixed-weight-delay-2380853/PROOF.md)

Install the dependency in [requirements.txt](requirements.txt), then run

```sh
sh verify-release.sh
```

The release contains the paper, verifiers, recorded output and the pinned Lean checks for three supporting lemmas. [How to replay the checks](CHECKS.md) · [File hashes](SHA256SUMS)
