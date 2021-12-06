### Definition
[[Complex Canonical Variables]] are very convenient for proving an important theorem about necessary and sufficient condition for the transformation to be canonical. The theorem states that for the transformation to be canonical, it is necessary and sufficient that the transformation preserves [[Poisson Brackets]]. Furthermore and this is really important for practical applications to prove the canonicity of a given transformation it is sufficient to check that is preserves [[Poisson Brackets]] between old and new variables. Since Poisson brackets are bit sensitive to whether we use complex or real canonical variables, the theorem applies equally well to canonical transformations in terms of both complex and real variables. 

We start with an almost trivial observation that along with a certain set of complex canonical variables, $\{a_j\}$, one can work with a set of arbitrary variables $\{b_s\}, \; b_s \equiv b_s(\{a_j\})$ employing the Poisson brackets to produce equations of motion:

$$\begin{gather} i\dot b_s = i\{H,b_s\} = \sum_j\left[\frac{\partial b_s}{\partial a_j}\frac{\partial H}{\partial a^*_j}-\frac{\partial b_s}{\partial a_j^*}\frac{\partial H}{\partial a_j}\right]\end{gather}$$

However, there exist special sets of new variables that are also canonical - independently of the particular form of $H$; that is equivalent to:

$$\begin{gather} i\dot b_s = \frac{\partial H}{\partial b^*_s}\end{gather}$$

for any $H$. To arrive at the necessary and sufficient conditions for the new variables to be canonical, we note that what we require amounts to:

### Relations
$$\begin{gather} \sum_j\left[\frac{\partial b_s}{\partial a_j}\frac{\partial}{\partial a^*_j} - \frac{\partial b_s}{\partial a^*_j}\frac{\partial}{\partial a_j}\right] \equiv \frac{\partial}{\partial b_s^*} = \sum_j\left[\frac{\partial a_j^*}{\partial b_s^*}\frac{\partial}{\partial a_j^*} +\frac{\partial a_j}{\partial b_s^*}\frac{\partial }{\partial a_j}\right]\end{gather}$$

where the right most equality is the [[Multivariable Chain Rule]] for complex partial derivatives. By linear independence of the differential operators $\{\partial/\partial a_j,\partial/\partial a_j^*\}$, the above equation is equivalent to:

$$\begin{gather} \frac{\partial b_s}{\partial a_j} =\frac{\partial a_j^*}{\partial b_s}, &&& \frac{\partial b_s}{\partial a_j^*} = -\frac{\partial a_j}{\partial b^*_s} \end{gather}$$

These are the necessary and sufficient conditions for $\{b_s\}$ to be canonical.

The invariance of the [[Poisson Brackets]] under some transformation of variables is a sufficient condition for that transformation to be canonical. Indeed, noticing that, for any $A$, 

$$\begin{gather} \frac{\partial A}{\partial a^*_j} = i\{A,a_j\}, &&& \frac{\partial A}{\partial a_j} = i\{a^*_j,A\}\end{gather}$$

and requiring the invariance of the Poisson brackets, we arrive at:
$$\begin{gather} \frac{\partial b_s}{\partial a_j} = i\{a^*_j,b_s\} =\frac{\partial a^*_j}{\partial b_s^*}, &&& \frac{\partial b_S}{\partial a^*_j} = i\{b_s,a_j\} = -i\{a_j,b_s\} = -\frac{\partial a_j}{\partial b_s^*} \end{gather}$$

Even more importantly from the practical point of view, this above equation tells us that to prove the canonicity it is sufficient to check the invariance of Poisson brackets between the old and new variables. And this can be done in terms of both complex and real variables, meaning that the criterion applies to real canonical variables as well.

### Poisson brackets between canonical variables

An equivalent and quite useful form of the necessary and sufficient condition for the variables to be canonical deals with Poisson brackets between all the new variables calculated with respect to the old ones. Here the requirement is that all the Poisson brackets have the following canonical form. For complex canonical variables, we have/need 
$$\begin{gather}\{b_s,b_r^*\} = (i/\lambda)\delta_{sr}, &&& \{b_s,b_r\}=0 \end{gather}$$

In terms of real variables, the canonical form of Poisson brackets is:

$$\begin{gather} \{q_s,q_r\} = 0, &&& \{p_s,p_r\} = 0, &&& \{p_s,q_r\}=\delta_{sr}\end{gather}$$

These relations are also interesting in the context of the correspondence between the variables of classical mechanics and their quantum (operator) counterparts. The counterparts of $b^*_s$ and $b_s$are the creation and annihilation operators, $\hat b^\dagger_s$ and $\hat b_s$, respectively; these are related to the operators of [[Generalized Coordinates]] and momentum, $\hat q_s$ and $\hat p_s$, by the transformation with $\lambda = \hbar$. The counterparts of the Poisson brackets are the [[Commutator]]s times $-i\hbar$