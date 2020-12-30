# Fast Principle Component Pursuit via Alternating Minimization

Pual Rodriguez, and Brendt Wohlberg [ICIP, 2013]

## Methodology

PCP problem:

$argmin_{L,S}{\| L \|_* + \lambda \| S \|_1} \;s.t.\; D=L+S$,

where $\lambda = 1/\sqrt{\max(p,n)}$.

Algorithm:

Batched