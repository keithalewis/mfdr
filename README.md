# Mathematical Finance Defect Report

In spite of, or perhaps because of, the seminal work of Fischer Black,
Myron Scholes, and Robert Merton III providing a mathematical foundation
for valuing financial instruments there has been very little progress in
applying the theory to solving problems faced by customers of Mathematical
Finance.  This repository collects a list of such problems.

The most glaring defect in the original theory assumes continuous time
trading.  This is impossible, high-frequency trading notwithstanding. The
B-S/M theory shows how to set up the initial hedge but does not address
the very first problem after that: when should the hedge be adjusted? It
is not possible to hedge "continuously". Given this reality, how does
one measure how well a hedge is performing (risk-management)? The
martingale representation theorem can be use to prove the B-S/M hedge,
assuming prices are geometric Brownian motion, is perfect.
This is of little use to market practitioners dealing with timing and
market liquidity issues.

The second major defect is the lack of a mathematical notation to indicate
who owns what. Not only who owns the underlying instruments but also
who owns the optionality for exercising contract provisions.
There are bonds where the owner has an option to put back the bond
to the issuer and the issuer has an option to call the bond back.
The standard solution in mathematical finance literature is to
assume all parties exercise "optimally" to sweep this under the rug.
A complete theory should allow non-optimal exercise to be incorporated.

There is no unified theory for dealing with all instruments simultaneously.
Historically, each market has developed independent models tailored
to the specific characteristics of the instruments involved.
