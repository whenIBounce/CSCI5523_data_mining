# Association Analysis

1. Itemset and support count
   - An itemset X is called **freuqent** if s(X) is __ ?
2. Association Rule
   - The strength of an association rule can be measured in terms of its **support** and **confidence**,
   - How to calculate support and confidence given an association rule of the form $X \rightarrow Y$ and $X \cap Y = \emptyset$
   - Why Use Support and Confidence?
   - Assuming that neither the left nor the right-hand side of the rule is an empty set, the total number of possible rules, R, extracted from a data set that contains d items is ?
   - Association rule mining algorithms is to decompose the problem into two major subtasks: **Frequent Itemset Generation** and **Rule Generation**

> Is the **support of a rule** $X \rightarrow Y$ the same as the **support of its corresponse itemset**, $X \cup Y$ ?
3. Frequent Itemset Generation
   - , a data set that contains k items can potentially generate up to __ frequent itemsets, excluding the null set. 
   - Theorem 5.1 (Apriori Principle).
    If an itemset is frequent, then all of its subsets must also be frequent.
   - Candidate Generation: Brute-force method; $F_{k-1} \times F_1$ method; $F_{k-1} \times F_{k-1}$ method. 
4. Compact Representation of Frequent Itemsets
   - Maximal frequent itemset: do not contain the support information of their subsets. 
   - Closed frequent itemset
   - What are relationships among frequent, closed, closed frequent, and maximal frequent itemsets.


