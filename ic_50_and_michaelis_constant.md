#### Some Definitions
Measurement of 
$\text{IC}_{50}$ 
values is very popular in a number of fields, 
including pharmacology, cell biology, enzymology, and biochemistry,
and each field has a slightly different definition.

As regards enzymology, and in the case of the 
[Cheng-Prusoff](https://pubmed.ncbi.nlm.nih.gov/4202581/)
equation, 
the relevant defintion is the following:

>$\text{IC}_{50}$ is the concentration of a _revesible_ inhibitor 
that produces 50% inhibition. 

The Michaelis constant is best defined as follows:
>$K_m$ is the substrate concentration at half maximal velocity (half 
$V_{max}$) 

<a name="craig_footnote_text_entry"></a>
Both
$K_m$
and 
$\text{IC}_{50}$ 
have dimensions of substrate concentration,
and both are defined in terms of half-maximal effect
(the Michaelis constant has even been considered an
$\text{SC}_{50}$, 
the "concentration of substrate required to produce a half-
maximal initial rate of reaction"
[
[Craig,1993](https://pubmed.ncbi.nlm.nih.gov/8488569/)
]
)
but, it seems to me, that
is as far as the similarities go.
<sup>[[1]](#fnotes)</sup>

What has become known as the Cheng-Prusoff equation , shown in equation 1, was
derived in 
[1973](ref)













#### Michaelis Constant

The Michaelis constant, or 
is best defined as the substrate concentration at
half maximal velocity (or at half 
$V_{max}$).

It has one important property: it is independent of enzyme concentration. 

(Or, to be pedantic, it is independent of enzyme concentration under the assumptions
generally applied in deriving the Michaelis-Menten equation)  

Provided that there are no complicating factors (such as contamination with another
enzyme catalyzing the same reaction), it is possible to determine the 
$K_m$
with a
crude enzyme preparation.

Perhaps more importantly, it allows easy comparison. 
Other factors, such as pH and temperature may affect 
$K_m$,
but the degree of purity of the enzyme preparation is
not one of them, and this (usually) cuts out a lot of argument. 

#### $\text{IC}_{50}$

For a reversible inhibitor 
(which is the only type of inhibition being considered here),
the 
$\text{IC}_{50}$ 
is defined as the inhibitor concentration producing 50% inhibition. 

#### $K_m$ and $\text{IC}_{50}$
Both 
$K_m$ 
and 
$\text{IC}_{50}$ 
have units of concentration (they can be directly 

Although
$\text{IC}_{50}$
values are very popular (they are relatively easy to determine, for example), there are 
two inherent drawbacks that make comparions very difficult:

1. A knowledge of the mechanism of inhibition (whether inhibition is competitive,
uncompetitive, non-competitive or 'mixed') is required. 

(The form of the Cheng-Prusoff equation will change depending on the mechanism of inhibition,
for example). 

2. A knowledge of the substrate concentration _relative to the_
$K_m$ 
_value_ is (almost certainly) required. 

The 
[Cheng-Prusoff](https://pubmed.ncbi.nlm.nih.gov/4202581/)
equation _for comptetitive inhibition_ (Eqn 1) aims to address this second 
problem:
 assuming that two (or more) inhibitors act competitively,
 can 
$\text{IC}_{50}$
 values provide any meaningful information, and how can they be compared (if at all)
 in order to provide some estimate of the relative potency oof the inhibitors? (
 Is A a better inhibitor than B?)

#### Cheng-Prusoff Equation (Competitive Inhibition)


$$ 
K_i 
=
\frac{\text{IC}_{50}}{1 + \frac{[S]}{K_m}}
\tag{1}
$$

One of the 'hallmarks' of a competitive inhibitor is that inhibition may be overcome
by increasing the substrate concentration, and therein lies the problem: the
ic50 
value (for a competitive inhibitor) will _increase_ as the substrate concentration increases.

To illustrate, let's take an example:

Assuming that inhibition is competitive in both cases, if you , working with inhibitor A at at a substrate concentration equal to 9 times the Km value (let's keep the calculations simple), report an 
IC50 
value of 10mM and I, working with inhibitor B at a substrate concentration equal to the 
Km 
value, report an
ic50 
value of  2mM, which is the better inhibitor?  

ICfifty
value of 



#### <a name="fnotes"></a>Footnotes
               
[Craig (1993)](https://pubmed.ncbi.nlm.nih.gov/8488569/) uses the abbreviation 
$\text{EC}_{50}$
(which IMO is a bit misleading: $K_m$ is independent of enzyme concentration)
[[back to main text](#craig_footnote_text_entry)]



#### References

Cheng Y, Prusoff W. H. 
(1973) 
Relationship between the inhibition constant ($K_I$) and the concentration of inhibitor which causes 50 per cent inhibition ($I_{50}$) of an enzymatic reaction. 
Biochemical Pharmacology, 22,3099-3108. 
[
[pubmed](https://pubmed.ncbi.nlm.nih.gov/4202581/)
]


Cheng H. C. 
(2001). 
The power issue: determination of $K_B$ or $K_i$ from $IC_{50}$. 
A closer look at the Cheng-Prusoff equation, the Schild plot and related power equations. 
Journal of Pharmacological and Toxicological Methods, 
46(2), 61–71. 
https://doi.org/10.1016/s1056-8719(02)00166-1


Chou T. 
(1974). 
Relationships between inhibition constants and fractional inhibition in enzyme-catalyzed reactions with different numbers of reactants, different reaction mechanisms, and different types and mechanisms of inhibition. 
Molecular pharmacology, 
10, 235–247.
[[pubmed](https://pubmed.ncbi.nlm.nih.gov/4212316/)]

Cornish-Bowden, Athel (2013)
[Fundamentals of Enzyme Kinetics](https://www.wiley.com/en-us/Fundamentals+of+Enzyme+Kinetics%2C+4th+Edition-p-9783527330744)
4th Ed,   Wiley-Blackwell

Craig D. A. 
(1993) 
The Cheng-Prusoff relationship: something lost in the translation. 
Trends in Pharmacological Sciences, 14, 89–91. 
[[pubmed](https://pubmed.ncbi.nlm.nih.gov/8488569/)]


Naqui A. (1983). What does $I_{50}$ mean?. 
The Biochemical Journal, 
215, 429–430
[[pubmed](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1152414/)]
[[pdf](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1152414/pdf/biochemj00341-0208.pdf)]

$$
E + S \xrightleftharpoons[{k_{-1}}]{k_1} 
ES   
\xrightarrow{k_p}
E + P
$$

$$
E + I \xrightleftharpoons[{k_{-2}}]{k_2} 
EI   
$$

      A mechanism that gives rise to Competitive Inhibition

          E # ES --> E + P
          #
          EI 

Hello

hello

      A mechanism that gives rise to Uncompetitive Inhibition

          E # ES  --> E + P
              #
              EI
