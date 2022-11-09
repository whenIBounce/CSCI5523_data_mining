
# Homework #4
# Name: Tianhong Zhang
# UMN Email: zhan4868@umn.edu
# Student ID: 5293616

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

## Question 2. 
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

## Question 3. 

| Sequence s                  | Sequence t      | Yes/ No |
|-----------------------------|-----------------|--------:|
| <{1,2,3} {2,4} {6}>         | <{2,4}>         | Yes     |
| <{1,2,3} {2,4} {6}>         | <{1}{2}{4}>     | No      |
| <{1}{3}{1,3}>               | <{1,3}{1}>      | No      |
| <{1,2} {1,2} {1}{2}>        | <{1}{1,2}{2}>   | Yes     |
| <{1,2,4}{1,4}{1}{2,3}>      | <{2}{3}>        | Yes     |
| <{1} {1,2} {1} >            | <{1,2} {1} {1}> | No      |
| <{1,2}{2}{1}>               | <{1}{2}{1,2}>   | No      |
| <{1,2,4}{1,4}{2,3}{1,2,3}>  | <{1}{2}{3}>     | Yes     |
| <{1,2,4}{1,4}{2,3}{1,2,3}>  | <{1}{2,4}{3}>   | No      |

## Question 4.

|                 | Candidate Generated | Candidate Pruned |
|-----------------|---------------------|------------------|
| <{p,t},{r},{t}> | Y                   | Y                |
| <{p},{t},{r,t}> | N                   | NA               |
| <{p},{r,t},{t}> | Y                   | N                |

## Question 5. 
1. a) Write the support count of the following subsequences:
   - (i) s({1,2}) = 1
   - (ii) s({1} {2}) = 3
   - (iii) s({2} {5}) = 3
   - (iv) s({2}{4,5}) = 2
   - (v) s({1}{2,5}) = 2
2. b) Which of the following rules satisfy the minconf requirement?
   - (i) conf({1} → {2}) = 1 > minconf
   - (ii) conf({2} → {5}) = 0.6 = mincong
   - (iii) conf({3} → {5} = 1 > minconf
3. c) Suppose there were 100 customers similar to A, 200 customers similar to B, 50 customers similar to
C, and 500 customers similar to D and E each. Repeat parts a) and b) for this scenario.
   - For support count:
     - (i) s({1,2}) = 1
     - (ii) s({1} {2}) = 3
     - (iii) s({2} {5}) = 3
     - (iv) s({2}{4,5}) = 2
     - (v) s({1}{2,5}) = 2
   - For conf:
     - (i) conf({1} → {2}) = 1 > minconf
     - (ii) conf({2} → {5}) = 800/1350 =0.59 <> mincong
     - (iii) conf({3} → {5} = 1 > minconf
4. d) Do the rules {2} → {5} and {2} → {2,5} have the same confidence? Give a brief justification.
   No, they are not the same. The support count for {2}{5} is differenct from {2}{2, 5}.

## Question 6.
1. (a) For each sequence s, determine if the given sequence t is a valid subsequence:

| Sequence s         | Sequence t  | Is a valid subsequence |
|--------------------|-------------|:----------------------:|
| <{2,4} {2,4} {6}>  | <{2} {4,6}> |           No           |
| <{3,4} {2,3} {1}>  | <{4}{1}>    |           Yes          |
| <{5} {1,2} {4,1}>  | <{2}{5}>    |           No           |
| <{4} {2,3} {1,2}>  | <{3}{2}>    |           Yes          |

2. (b) Assume that the four sequences in the left column are the only frequent 5-sequences (i.e., sequences
with 5 events) found from a sequence data set. Which candidate 6-sequences can be generated from these
four 5-sequences: {3, 4}{2, 3}{1, 2}

## Question 7. 
For each of the described data sets, decide what type of clustering should be used (hierarchical or
partitional, exclusive or overlapping or fuzzy, complete or partial (incomplete)). Briefly explain your
reasoning if you feel there may be several possible answers.

1. a) Proteins perform different biological functions that are organized into a hierarchical taxonomy (GO) defined by biologists. Some proteins can be multi-functional as well. You want to group them based on those functions. Some proteins may also be missing functional annotation.
   **hierarchical, overlapping, partial**
2. b) A nutritionist asks you several questions (e.g., your calorie intake, types of food you eat, your
physical activity labels, and so on) to assess your risks for diabetes in three different groups: low,
medium, and high.
   **partitional, exclusive, complete**. Assume that there is no other class between "low" and "medium"; "medium" and "high", that's how I decide the type of clustering. 
3. c) The objects are the applicants to a college. Each applicant is assigned a score from 0 to 10, indicating the likelihood/desirability of their admission. Even before any decisions have been made, the admissions personnel view the students as belonging to two groups: those that will be accepted and those that will be rejected.
   **hierarchical, exlusive, complete**. If the class label is "willBeAccepted" and "willBeRejected", one student cannot belong to both class, and if you see score 0 to 10 as subsets, then there hierarchical relationship between score labels and class labels.
4. d) Grouping of cities based on the various locations, namely county (local region), state or province, and country.
   **hierarchical, exclusive, complete**. Assume that no one city can belong to two countries. 

## Question 8.
1. a) All of the initial centroids are located in one of the circles.
   The centroids will move, there may be 0 centroids in each circle. To minimize the objective function, all centroids will move towards another cricle. After several iterations, it is possible for all five centroids end up locating between two circles. Assume that A(0,0) and B(4,0), if the centroid is at (0,0), the summed error is 4^2 + 0^2 = 16; if the centroid is at the mean (2,0), the summed error is 2^2 + 2^2 = 8; So in this case, we call not decide how many centroids will end up in each circle eventually. 
2. b) At least one initial centroid in each circle. In this case, the centroilds will move and at least one centroid in each circle. Five centroids are likely to be distributted in both circles. 
3. c) If the number of points in the larger circle is far greater than the number of points in the smaller circles, no matter how the initial centroids are located, then it is very likely that all five centroids end up in the larger circle. 
