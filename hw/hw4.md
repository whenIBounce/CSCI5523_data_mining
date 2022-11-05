## Question 1. 
1. (a). What is the range of this measure? When does the measure attain its maximum and minimum values?
<br>
    - The range of M is $(-\infty, 1]$
    - M attains its maximum when $P(B|A) = 1$
    - M attains its minimum when $P(B|A) = 0$ and $P(B) \rightarrow 1$
2. (b) How does M behave when P(A,B) is increased while P(A) and P(B) remain unchanged?<br>
   M increased.
3. (c) How does M behave when P(A) is increased while P(A, B) and P(B) remain unchanged? <br>
   M remains the same. 
4. (d) How does M behave when P(B) is increased while P(A, B) and P(A) remain unchanged? <br>
   M could increase or decrease depends on the value of $P(B|A) = c$ and $P(B) = x$, because $\frac{d}{dx}\left(\frac{c-x^2}{x-x^2}\right)=\frac{-x^2+2cx-c}{\left(x-x^2\right)^2}$.
5.  (e) Is the measure symmetric under the variable permutation? <br>
   No, the measure is asymmetric. 

## Question 2
1. a) Consider the rule {p} -> {q} and {r}->{s}. Compute the IS (cosine) and Interest factor for both rules. <Br>
   $I(P, Q)=1.017$ <BR>
   $IS(P, Q)=880/930=0.946$<BR>
   $I(R, S)=4.082$ <BR>
   $IS(R, S)=20/70=0.286$ <BR>
2. b) Given that these tables belong to the text domain and the items {p}, {q}, {r}, {s} represent some
words, which measures above would you prefer? Justify. <br>
Interest factor is preferred. When the words in docs are sparse, we care about the sparse-co occurances. 
1. c) Consider another measure M = sup({x,y}) / sup(y) for rule {x} → {y}. Compute this measure for the
above rules. Which of the above measures (IS and Interest factor) do the values look similar to?
Would this similarity always hold? If yes, explain otherwise explain when both would be different. <br>
$M(P, Q)=880/930=0.946$<br>
$M(R, S)=20/70=0.296$<BR>
It look more similar to IS. This similarity will not always hold, because $s(P)$ will not always equal to $s(Q)$. 