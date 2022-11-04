To answer this question, we need to delve into the world of 
[dimensional analysis](https://en.wikipedia.org/wiki/Dimensional_analysis) 
and to consider when and how rate constants may be compared.

The OP considers the following simple kinetic mechanism, (which, after defining kinetic constants such as
$K_m$
and
$k_{cat}$
in terms of rate constants,
gives rise to the 
[Michaelis-Menten](https://en.wikipedia.org/wiki/Michaelis%E2%80%93Menten_kinetics)
equation):

$$
E + S \xrightleftharpoons[{k_{-1}}]{k_1} 
ES   
\xrightarrow{k_p}
E + P
\tag{1}
$$ 

#### First and Second Order Rate Constants

As written, $k_1$ is a _second-order_ rate constant and  $k_p$ is a _first-order_ rate constant. 

Therefore $k_1$ will have units of  $concentration^{-1}\text{. }time^{-1}$ and $k_1$ will have units of $time^{-1}$.

For example, $k_1$ may be spoken of as having a value of 
$10^9 \text{ M}^{-1}\text{ s}^{-1}$ (
[here](https://bionumbers.hms.harvard.edu/bionumber.aspx?id=103916&ver=2)
and
[here](https://en.wikipedia.org/wiki/Diffusion-limited_enzyme)),
 or as having a value of 
$10^9 \text{ L mol}^{-1}\text{s}^{-1}$, and $k_p$ may be spoken of as having a value of $10^6 \text{ s}^{-1}$.

By the laws of
[dimensional analysis](https://en.wikipedia.org/wiki/Dimensional_analysis),
it is meaningless to compare quantities of different units. 
It is absurd, for example, it ask if pH 7 is greater than (or less than) $10^\text{o}\text{C}$,
or if 2 mol is greater than (or less than) 5 seconds.

So too with rate constants: it is meaningless to ask if a second-order rate constant is greater than or less than (or is equal to) a first-order rate constant. 

The application of dimensional analysis to situations often encountered in enzyme kinetics is well described in 
[Fundamentals of Enzyme Kinetics](https://www.wiley.com/en-us/Fundamentals+of+Enzyme+Kinetics%2C+4th+Edition-p-9783527330744)
(Cornish-Bowden, 2013, 4th Ed, Section 1.3) and the relevant section seems to be freely accessible via 
[Google Books](https://books.google.ie/books?id=_3fqaYnrdosC&printsec=frontcover&dq=Fundamentals+of+Enzyme+Kinetics+Athel+Cornish-Bowden&hl=en&sa=X&ved=2ahUKEwiL26iY1OT1AhWYiVwKHSHeDK4Q6AF6BAgJEAI#v=onepage&q=Fundamentals%20of%20Enzyme%20Kinetics%20Athel%20Cornish-Bowden&f=false).

For example, we can multiply and divide quantities of different dimensions, but we
cannot add or subtract them. 

Thus, inspection of the numerator of the following equation shows that it is CLEARLY WRONG:

$$ 
K_m 
=
\frac{k_p + k_{1}}{k_{-1}}
\tag{2}
$$

The CORRECT expression for $K_m$ for the mechanism shown in Eqn (1) is 
_the sum of the two first-order rate constants, divided by the second-order rate constant_:


$$ 
K_m 
=
\frac{k_p + k_{-1}}{k_{1}}
\tag{3}
$$

We can also infer from Eqn (3) that ${K_m}$ has dimensions of molarity, 
even if we have no idea as to what the symbol ${K_m}$ refers.


$$      
  \frac{\text{s}^{-1}}{\text{M}^{-1}\text{ s}^{-1}} = \text{M} 
  \tag{4}
$$

Application of the rules of dimensional analysis is often useful in 'scanning' the
equations encountered in enzyme kinetics.


$$         
Y= 
\frac
{1}                                      
 {1 + \frac{[A]}{K_m^A} + \frac{[B]}{K_m^B} + X}
 \tag{5}
$$

For example, without any prior knowledge as to what $X$, $Y$, $K_m^A$ and $K_m^B$ refer to, 
inspection of Eqn (5) allows the following conclusions to be drawn:

1. $X$ is dimensionless
2. The quantities $\frac{[A]}{K_m^A}$ and $\frac{[B]}{K_m^B}$ are dimensionless
3. $Y$ is dimensionless

#### _Pseudo_ First-Order Rate Constants

Although $k_1$ and  $k_2$ have different dimensions, 
$k_1 \text{[A]}$
has dimensions of a first-order rate constant $(time^{-1})$ and _can_ be directly compared
with $k_p$ and $k_{-1}$.

The quantity
$k_1 \text{[A]}$
is often referred to as a _pseudo_ first-order rate constant. (Personally, 
I don't like the term)

Thus, to argue that $k_1 \text{[A]}$ >> $k_p$ is perfectly OK from a dimensional 
analysis perspective.

Perhaps more importantly, a _pseudo_ first-order rate constant may be added to or
subtracted from a first-order rate constant.
                                   
Thus, an equation such as the following presents no problems (again from a dimensionless
analysis point of view):

$$         
Y= 
\frac{k_1}                                      
{{k_1} [A]  + k_{-1} + {k_p}}
 \tag{6}
$$


#### Common Confusion Concerning Rate Constants: An Example 

It is surprising how often the laws of dimensional analysis are misapplied in 
the world of enzyme kinetics.

For example, in a paper published in _J. Chem. Educ._ in 2011, it is stated "For the classic Michaelis-Menten enzyme, 
$k{_1} > k_{-1} >>  k{_2}$" where "... $k_1$ is the forward rate constant for the first step, the
fast binding of substrate $(S)$ to enzyme $(E)$ to make the non-
covalent enzyme-substrate complex $(ES)$,  $k_{-1}$ is the reverse
rate constant for the dissociation of $ES$ back into $E + S$; and $k_2$
is the rate constant for the subsequent slow catalytic step converting $S$ to product".  

Let's state it bluntly: $k_1$ _cannot_ be greater than $k_{-1}$, as $k_1$ is a 
second-order rate constant and $k_{-1}$ is a first-order rate constant.

Furthermore (and very surprisingly), _J. Chem. Educ._ has not corrected the error. 

(In my opinion, the paper is otherwise good).


#### Reference

Cornish-Bowden, Athel (2013)
[Fundamentals of Enzyme Kinetics](https://www.wiley.com/en-us/Fundamentals+of+Enzyme+Kinetics%2C+4th+Edition-p-9783527330744)
4th Ed,   Wiley-Blackwell
[ [google books](https://books.google.ie/books?id=_3fqaYnrdosC&printsec=frontcover&dq=Fundamentals+of+Enzyme+Kinetics+Athel+Cornish-Bowden&hl=en&sa=X&ved=2ahUKEwiL26iY1OT1AhWYiVwKHSHeDK4Q6AF6BAgJEAI#v=onepage&q=Fundamentals%20of%20Enzyme%20Kinetics%20Athel%20Cornish-Bowden&f=false) ]


