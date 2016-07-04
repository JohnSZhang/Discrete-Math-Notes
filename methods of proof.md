Create Proofs:

* Basic Proof Principles:
    P, P ⇒ Q Proves Q
    P ⇒ Q, Q ⇒ R, Proves P ⇒ R
    P ⇒ Q, Not(Q) Proves Not(P)
    Not(P) ⇒ Not(Q) Proves Q ⇒ P

* Proof by Cases:
    To prove a complicated proof is true, we break it down into each of its cases and prove them separately.

* Proving an Implication:
    These are propositions in the form of If P, then Q. Or simply P ⇒ Q

    Assume P is true: Assume P is true, show that Q follows.

    Prove Contrapositive: Prove Not Q, then it follows that since Not Q ⇒ Not P, P ⇒ Q

* Proving an 'If and Only If':
    Prove Each Statements Separately: Prove both P ⇒ Q and Q ⇒ P

    Construct a Chain of IFFs: A more intricate method which require more ingenuity, create a proof by creating a chain of other IFFs until we can prove Q.

* Proof by Contradiction:
    To prove P is true, assume Not(P) then use Not(P) to derive the falsehood of a truth, hence derived a contradiction to prove P.

    You are proving ¬P => F is true, so P must be true.

    Example, proving that sqrt(2) is irrational.
    Pf (by contradiction).
    Assume sqrt(2) is rational.
    sqrt(2) = a / b, where a and b are lowest terms
    ⇒ 2 = a ^ 2 / b ^ 2
    ⇒ 2 b ^ 2 = a ^ 2
    ⇒ a is even (because a ^ 2 is event), and that a ^ 2 is a multiple of 4
    ⇒ 4 / a ^ 2
    ⇒ 4 / 2 b ^ 2
    ⇒ 2 / b ^ 2
    ⇒ b is even
    ⇒ a / b is contradiction as they are not lowest terms
    ⇒ QED sqrt(2) is not rational

* Proofs about Sets:
    Common Set Definitions: ∅ (empty set), N (natural nonnegative integers), Z (integers), Q (rational numbers), R (real numbers), C (complex numbers).

    | is the symbol for 'such that', or 'restricted to'. So x∈Z | x >= 1 contains all integers greater than or equal to 1.

    ⊆ is the symbol for (subset of), a subset can be the same as the set that it is a subset of.

    ∪ is the union of two sets, and ∩ is the intersect of two sets. When set X - set Y, the result are all elements in set X that's not in set Y.

    A compliment of a set X is the intersection of the Domain and the set X. Two sets are disjoin if their intersect is the empty set.

    Cardinality of a set is the number of elements in it. While the set of all subsets of a set X is called the power set of set X. There are always 2 ^ n sets in the power set of a set size n.

    Product operation of a set creates a new set consisting of all sequences where the first component is grown from first set, second from the second, etc.

    Set builders users a predicate to build a set by selecting only those elements which would make the predicate true (like a kind of filter).

* Well Ordering Principle:
    Every nonempty set of nonnegative integers has a smallest element.

    To prove that P(n) is true for all n∈N:
        define set C of counterexamples to P, ie C:= { n∈N | P(n) is false }
        use proof by contradiction and assume C is nonempty.
        Using well ordering principle, find smallest element n0 in C.
        Find contradiction, conclude C must be empty, and that no conterexample can exist. 

* Proof by Induction:
    Induction Axiom: let P(n) by a predicate. If P(0) is true and ∀n∈N (P(n)⇒P(n + 1)), then ∀n∈N P(n) is true.

    Therom: ∀n>=0, 1 + 2 + 3 + ... + n = n(n+1) / 2
    Pf (by induction)
    Let P(n) be the predicate that sigma of i (i=1 to n) = n(n+1)/2
    sigma of i (i = 1 to 0) = 0 = 0(0 + 1) / 2
    Induction Step
    Assume P(n) is true for purpose of Induction
    1 + 2 + ... + n + (n + 1)
    = (n + 1)(n + 2) / 2
    n (n + 1) / 2 + n + 1
    = (n ^ 2 + n + 2n + 2) / 2
    = (n + 1)(n + 2) / 2
    QED P(0) is true and P(n) ⇒ P(n + 1)
