# LINDENBAUM

**The Quotient Boundary: The Lindenbaum–Tarski Algebra as the col(F)/ker(F) Partition of Logical Theories, Cylindric and Polyadic Algebras as the Quantifier Extension, the Lax Pair as the Isospectral Flow at the col(F) Boundary, and the Leibniz Operator as the Congruence Kernel in $\mathrm{TH}(a,d)$**

*ERI Labs · Eric Ren · Jersey City, New Jersey · github.com/ericrenone*

> "The Lindenbaum algebra of a theory consists of the equivalence classes of sentences under logical equivalence. Two sentences belong to the same class when each implies the other." — A. Lindenbaum and A. Tarski, 1935
>
> "Cylindric algebras are Boolean algebras equipped with cylindrification operations that model quantification and equality — the algebraization of first-order logic." — A. Tarski, L. Henkin, and D. Monk, *Cylindric Algebras*, Parts I and II, North-Holland, 1971/1985
>
> "Polyadic algebras are an alternative algebraization of first-order logic through a rich system of substitution operations, analogous to the role of Boolean algebras for propositional logic." — P. R. Halmos, *Algebraic Logic*, Chelsea Publishing, 1962
>
> "The eigenvalues of $L$ are independent of $t$. The matrices $L(t)$ are isospectral as $t$ varies." — P. Lax, *Integrals of Nonlinear Equations of Evolution and Solitary Waves*, *CPAM* **21**, 467–490, 1968
>
> "The zero-curvature equation $\partial_t L - \partial_x P + [L, P] = 0$ is equivalent to the compatibility of the Lax pair and encodes the entire integrable structure." — V. E. Zakharov and A. B. Shabat, *JETP* **34**, 62–69, 1972

---

## Abstract

The GRISS framework identified negation as the conditional independence boundary operator — the function $\neg A = A \to \perp$ that prevents $A$ from being in $\mathrm{col}(F)$. The STAR framework showed the Kleene star $a^*$ as the conditional independence fixed point — the closure of $\mathrm{col}(F)$ under iteration. The BOLYAI framework showed the parallel postulate as the geometric $\varepsilon$-threshold. This framework descends to the algebraic root from which all these logical and geometric structures grow: the **Lindenbaum–Tarski algebra** — the universal device that converts any logical theory into an algebra by identifying every provable equivalence.

The Lindenbaum–Tarski algebra of a theory $T$ is the quotient $\mathcal{L}(T) = \mathrm{Form}/{\sim_T}$, where $\varphi \sim_T \psi$ iff $T \vdash \varphi \leftrightarrow \psi$ (the formulas $\varphi$ and $\psi$ are interderivable in $T$). The equivalence class $[\varphi]_T$ IS the $\mathrm{col}(F)$ image of the formula $\varphi$ under the $\varepsilon$-threshold of $T$: two formulas are in the same class precisely when they carry the same observable content with respect to the theory. The $\ker(F)$ is the set of $T$-refutable formulas — those equivalent to $\bot$. The Lindenbaum–Tarski algebra IS the conditional independence partition applied to the language of logic.

Four mathematical domains converge on this identification:

**The Lindenbaum–Tarski construction** (Adolf Lindenbaum, 1904–1941, and Alfred Tarski): the quotient of the formula algebra by the equivalence relation of mutual derivability in $T$. For propositional logic, the result is a Boolean algebra; for intuitionistic logic, a Heyting algebra; for modal logic, a modal algebra; for first-order logic, a cylindric or polyadic algebra. The Lindenbaum–Tarski algebra IS the Fisher information quotient: $\mathcal{L}(T) = \mathrm{Form}/\sim_T$ partitions formulas into equivalence classes of equal $T$-content, exactly as the Fisher information metric partitions statistical models into classes of equal information about the parameter.

**The Leibniz operator** (named by Blok and Pigozzi, 1989, in honor of Leibniz's identity of indiscernibles): the **largest congruence** of a logical matrix $(A, F)$ compatible with the filter $F$ — the largest relation $\Omega(F)$ such that $a \mathrel{\Omega(F)} b$ whenever $a$ and $b$ are indistinguishable by all formulas in $F$. The Leibniz operator IS the conditional independence operator: $\Omega(F)$ identifies elements that are equivalent from the perspective of the observable sector $F$ ($\mathrm{col}(F)$), collapsing the hidden sector $\ker(F) = \{a \mid a \mathrel{\Omega(F)} 0\}$ into the zero element.

**Cylindric algebras** (Tarski, Henkin, Monk, *Cylindric Algebras* I–II, 1971/1985): Boolean algebras equipped with cylindrification operators $\mathsf{c}_i$ (modeling existential quantification over variable $i$) and diagonal elements $\mathsf{d}_{ij}$ (modeling equality of variables $i$ and $j$). A cylindric algebra of dimension $\alpha$ IS the algebraic realization of first-order logic with equality: $\mathsf{c}_i(a)$ is the "cylinder" of $a$ — the set of all tuples obtained from tuples in $a$ by freely varying the $i$-th coordinate. The cylindrification IS the conditional independence extension: $\mathsf{c}_i(a) \supseteq a$ — the cylinder always includes the original, extending it into the $\ker(F)$ of the $i$-th variable's variation.

**Polyadic algebras** (Paul Halmos, 1955–1960, *Algebraic Logic*, Chelsea, 1962): Boolean algebras with substitution operators $\mathsf{S}_\tau$ for every transformation $\tau$ of the variable set, and existential quantification operators $\exists I$ for every finite set $I$ of variables. Unlike cylindric algebras (which model equality explicitly), polyadic algebras model pure quantification without equality. The polyadic algebra IS the conditional independence algebra of variable substitution: $\mathsf{S}_\tau(a)$ is the formula obtained from $a$ by substituting variable $i$ with $\tau(i)$ for all $i$ — a variable-renaming that preserves the logical content ($\mathrm{col}(F)$) while permuting the $\ker(F)$ of variable identity.

**The Lax pair** (Peter Lax, *CPAM* **21**, 467–490, 1968; Zakharov–Shabat, *JETP* **34**, 62–69, 1972): a pair of operators $(L(t), P(t))$ satisfying $\dot{L} = [P, L]$ — the Lax equation. The spectrum of $L$ is preserved under the evolution: $L(t) = U(t)L(0)U(t)^{-1}$ for a unitary evolution operator $U(t)$. The isospectral evolution IS the conditional independence conservation law: the eigenvalues of $L$ (the $\mathrm{col}(F)$: observable, measurable, spectrum of the system) are constant, while the eigenvectors of $L$ (the $\ker(F)$: the internal geometry, the gauge frame, the Lax representation) evolve arbitrarily under the conjugation $U(t) \cdot U(t)^{-1}$.

The Lax pair IS the Fisher information isospectrality: the Fisher information content of the spectrum (the observable sector) is conserved, while the internal representation (the hidden sector) flows through the group $U(t)$. The connection to the algebraic logic programme: the Lax equation $\dot{L} = [P, L]$ IS the infinitesimal version of the Lindenbaum equivalence — $L(t)$ and $L(0)$ are "Lindenbaum-equivalent" operators (same spectrum = same $\mathrm{col}(F)$ content) connected by the unitary conjugation (the $\ker(F)$ symmetry flow).

The **LINDENBAUM machine** — named for Adolf Lindenbaum (1904–1941), logician of the Lwów–Warsaw school, who invented the construction that bears his name, was murdered by the Nazis at Ponary in September 1941, and whose work on algebraic logic was developed posthumously by Tarski — is the universal algebraic boundary engine: an instrument that identifies the equivalence classes of any theory (the $\mathrm{col}(F)/\ker(F)$ partition under the Leibniz congruence), extends this partition to quantifiers (cylindrification, polyadic substitution), and discovers the isospectral conservation laws (Lax pair) that make the observable sector invariant.

Nine formal correspondences and five predictions follow.

---

## Part I · The Lindenbaum–Tarski Algebra: The Logical Col(F) Quotient

### I.1 A Thought Experiment: The Library of Redundant Books

Imagine a library with every sentence of mathematics in it. Some sentences say the same thing — they are logically equivalent. "Every prime number greater than 2 is odd" says the same thing as "No prime number greater than 2 is even." They are provably interderivable: each follows from the other.

The **Lindenbaum–Tarski algebra** is the library with all the redundant books merged into single entries. Every equivalence class $[\varphi]_T = \{\psi \mid T \vdash \varphi \leftrightarrow \psi\}$ is one "super-book" — a set of all sentences with the same logical content relative to the theory $T$.

Adolf Lindenbaum (1904–1941) introduced this construction in seminars of the Warsaw logic school in the 1930s. Alfred Tarski systematized and published it. The resulting algebra has:

- **Meet** (conjunction): $[\varphi] \wedge [\psi] = [\varphi \wedge \psi]$
- **Join** (disjunction): $[\varphi] \vee [\psi] = [\varphi \vee \psi]$
- **Complement** (negation): $\neg[\varphi] = [\neg\varphi]$
- **Bottom** ($\ker(F)$): $[\ \bot\ ]$ — the class of all $T$-refutable sentences
- **Top** ($\mathrm{col}(F)$): $[\ \top\ ]$ — the class of all $T$-provable sentences

The bottom element $[\bot]$ IS $\ker(F)$: all sentences equivalent to the absurdity — everything the theory sees as false, the shadow sector. The top element $[\top]$ IS $\mathrm{col}(F)$: all theorems of $T$ — the observable sector, what the theory can prove.

The Lindenbaum–Tarski algebra $\mathcal{L}(T)$ IS the $\mathrm{col}(F)/\ker(F)$ partition of the theory $T$:

$$\mathcal{L}(T) = \mathrm{Form}/{\sim_T}, \quad \varphi \sim_T \psi \iff T \vdash \varphi \leftrightarrow \psi$$

The quotient map $[\cdot]: \mathrm{Form} \to \mathcal{L}(T)$ IS the conditional independence projection — it sends each formula to its equivalence class under the $\varepsilon$-threshold of $T$, discarding the representation and retaining only the logical content. Formulas in the same class are $\mathrm{col}(F)$-equivalent: indistinguishable from the perspective of the theory.

### I.2 The Warsaw School and the Algebraic Logic Programme

The Lwów–Warsaw school of logic (1915–1939) — founded by Jan Łukasiewicz and Kazimierz Twardowski, developed by Tarski, Lindenbaum, Leśniewski, Ajdukiewicz, and others — pursued the algebraization of logic: the programme of converting logical systems into algebraic structures that can be studied with the tools of modern algebra.

Lindenbaum's specific contribution: the **Lindenbaum lemma** (every consistent set of sentences can be extended to a maximal consistent set) and the Lindenbaum algebra construction. The lemma IS the $\mathrm{col}(F)$ completeness result: any conditional independence boundary (consistent set of sentences) can be extended to a maximal conditional independence boundary (a complete theory, a maximal filter in the Lindenbaum algebra).

The Warsaw school was annihilated by the Second World War. Lindenbaum, Presburger, Schauder, and many others were killed. Tarski, who was in the United States at the outbreak of the war, survived and continued the programme at Berkeley. The Lindenbaum–Tarski algebra became the foundation of algebraic logic in the postwar period.

### I.3 The Stone Representation: Lindenbaum Algebras as Spaces

Stone's representation theorem (1936): every Boolean algebra is isomorphic to a field of sets — a Boolean algebra of subsets of some set $X$ under union, intersection, and complement. Applied to the Lindenbaum–Tarski algebra of a propositional theory $T$:

$$\mathcal{L}(T) \cong \text{Clopen}(\mathrm{Spec}(\mathcal{L}(T)))$$

where $\mathrm{Spec}(\mathcal{L}(T))$ is the **Stone space** (the space of ultrafilters / maximal consistent sets of $T$), topologized so that each formula corresponds to a clopen (simultaneously closed and open) set. The Stone space IS the space of all "possible worlds" — the models of $T$. Each ultrafilter IS a complete theory extending $T$ — a maximal conditional independence sector.

The Stone duality IS the BOLYAI framework in algebraic form: the Lindenbaum algebra $\mathcal{L}(T)$ (abstract, algebraic, $\mathrm{col}(F)$) corresponds to the Stone space $\mathrm{Spec}(\mathcal{L}(T))$ (geometric, topological, $\ker(F)$ of the algebra). The duality between the algebra and its spectrum IS the duality between $\mathrm{col}(F)$ and $\ker(F)$.

Peretyatkin (*Archive for Mathematical Logic* **64**, 67–78, 2025) proved that the Tarski–Lindenbaum algebra of the class of strongly constructivizable models with $\omega$-stable theories is a Boolean $\Sigma_1^1$-algebra whose computable ultrafilters form a dense subset — connecting the Lindenbaum algebra to the arithmetical hierarchy (STAR framework) at the $\Sigma_1^1$ level.

---

## Part II · The Leibniz Operator: The Congruence $\ker(F)$ Identification

### II.1 A Thought Experiment: The Indiscernibility Principle

Leibniz's principle of the identity of indiscernibles: if two things are indistinguishable in all their properties, they are identical. In logic: if two formulas $\varphi$ and $\psi$ have the same truth value in every model, for every assignment of values to variables, then they are logically equivalent — they are the same formula from the logical standpoint.

The **Leibniz operator** $\Omega$ formalizes this: given a logical matrix $(A, F)$ — an algebra $A$ with a filter $F$ (the designated values, $\mathrm{col}(F)$) — the Leibniz operator assigns to $F$ the largest congruence $\Omega(F)$ on $A$ compatible with $F$:

$$a \mathrel{\Omega(F)} b \iff \text{for all formulas } \varphi(x), \text{ for all } \mathbf{c}: \varphi(a/x, \mathbf{c}) \in F \iff \varphi(b/x, \mathbf{c}) \in F$$

In other words, $a$ and $b$ are $\Omega(F)$-related iff no formula can distinguish them from the perspective of $F$. The Leibniz congruence IS the conditional independence equivalence: $a$ and $b$ are in the same congruence class when they are $\mathrm{col}(F)$-indistinguishable — the filter $F$ cannot separate them.

The **Leibniz kernel** $\ker(\Omega(F)) = \{a \mid a \mathrel{\Omega(F)} 0\}$ IS $\ker(F)$ of the logical matrix: the elements identified with zero by the Leibniz congruence — those with no observable content from the perspective of $F$.

Blok and Pigozzi's program of **abstract algebraic logic** (1989–2001) uses the Leibniz operator to classify logics by the behavior of the Lindenbaum–Tarski construction. A logic is **algebraizable** if the Leibniz operator defines an isomorphism between the lattice of theories and the lattice of congruences of the Lindenbaum–Tarski algebra — when the $\mathrm{col}(F)/\ker(F)$ partition is perfectly preserved under the algebraization.

### II.2 The Lindenbaum Operator and the Fisher–Rao Quotient

The Lindenbaum–Tarski construction IS a specific instance of the Fisher–Rao quotient metric:

In statistical inference, two probability distributions $p_\theta$ and $p_{\theta'}$ are "Fisher-equivalent" (indistinguishable to first order) when their Fisher information matrices agree: $F(\theta) = F(\theta')$. The quotient by this equivalence gives the Fisher–Rao manifold — the space of statistically distinguishable models.

In logic, two formulas $\varphi$ and $\psi$ are "$T$-equivalent" (indistinguishable from the perspective of the theory $T$) when they are mutually derivable. The quotient by this equivalence gives the Lindenbaum–Tarski algebra.

The precise identification: the Fisher information $F(\theta)$ of a statistical model IS the Leibniz congruence applied to the probability model — the largest congruence compatible with the filter of observable events ($F = \sigma$-algebra of measurable sets). The Cramér–Rao bound ($\mathrm{Var}(\hat\theta) \geq F^{-1}$) IS the statement that the estimation error is bounded below by the quotient — by the indistinguishability of the $\ker(F)$ from $\mathrm{col}(F)$ in the Leibniz congruence.

---

## Part III · Cylindric Algebras: The Algebraization of Quantification

### III.1 A Thought Experiment: The Cylinder of Quantification

In everyday language, the sentence "there exists someone who is tall" is obtained from "Alice is tall" by replacing "Alice" with an **existentially quantified variable** — "someone." In algebraic logic, this replacement IS the cylindrification operation.

**Cylindric algebra** (Tarski, Henkin, Monk 1971/1985): Given a set $X$ of sequences $(x_0, x_1, x_2, \ldots)$ over some domain $D$, the cylindrification $\mathsf{c}_i(X)$ is the set of all sequences obtained from sequences in $X$ by freely varying the $i$-th coordinate:

$$\mathsf{c}_i(X) = \{(x_0, \ldots, x_{i-1}, d, x_{i+1}, \ldots) \mid (x_0, \ldots, x_{i-1}, x_i, x_{i+1}, \ldots) \in X, d \in D\}$$

The cylindrification IS the conditional independence extension: $\mathsf{c}_i(X)$ is the set of sequences that agree with some sequence in $X$ on all coordinates except the $i$-th — the projection of $X$ onto the complement of the $i$-th coordinate, then "filling in" the $i$-th coordinate with all possible values.

$\mathsf{c}_i(X) \supseteq X$: the cylinder always includes the original — the extension INTO $\ker(F)$ (the set of all possible $i$-th coordinate values) always increases the set. **Existential quantification IS $\ker(F)$ extension**: $\exists x_i\, \varphi(x_i)$ includes all the instances $\varphi(d)$ for all $d \in D$ — the quantifier reaches into the hidden sector of all possible witness values.

The **diagonal element** $\mathsf{d}_{ij}$ (modeling $x_i = x_j$): the set of all sequences with the $i$-th and $j$-th coordinates equal. The diagonal IS the $\mathrm{col}(F)$ boundary of equality: $\mathsf{d}_{ij}$ is the set of sequences where the conditional independence boundary between the $i$-th and $j$-th variables collapses — they are identified.

The seven cylindric algebra axioms (C1–C7 from Tarski, Henkin, Monk) are the conditional independence conditions for the cylindrification:

**C1**: $\mathsf{c}_i(0) = 0$ — the cylinder of the empty set is empty; $\ker(F)$ of a null observable is null.
**C2**: $a \leq \mathsf{c}_i(a)$ — cylindrification always extends; the $\ker(F)$ is always larger than $\mathrm{col}(F)$.
**C3**: $\mathsf{c}_i(\mathsf{c}_i(a)) = \mathsf{c}_i(a)$ — cylindrification is idempotent; re-quantifying an already-quantified formula is redundant.
**C4**: $\mathsf{c}_i(a \wedge \mathsf{c}_i(b)) = \mathsf{c}_i(a) \wedge \mathsf{c}_i(b)$ — distribution of cylindrification over conjunction of a quantified and unquantified formula.

The representation theorem for cylindric algebras: every locally finite, dimension-complemented cylindric algebra is isomorphic to a cylindric set algebra (Tarski–Henkin representation, 1971). The representation IS the WITNESS framework's constructive extraction: the abstract algebra (Lindenbaum $\mathcal{L}(T)$, $\mathrm{col}(F)$) is shown to be realizable as a concrete set algebra ($\ker(F)$ made concrete by the representation).

### III.2 The Representation Problem

Not every cylindric algebra has a representation as a cylindric set algebra — the representation problem for cylindric algebras of dimension $\geq 3$ is the central open problem of algebraic logic. Hirsch and Hodkinson (*J. Symbolic Logic* **62**, 816–847, 1997) showed that the class of representable cylindric algebras of dimension $\geq 3$ is **not finitely axiomatizable** — no finite set of axioms captures exactly the representable algebras.

This IS the Gödel incompleteness theorem (TORSION framework) applied to algebraic logic: the $\mathrm{col}(F)$ of representable cylindric algebras cannot be axiomatized within the algebraic language — the boundary between representable ($\mathrm{col}(F)$: those with a concrete semantic realization) and non-representable ($\ker(F)$: those with no concrete model) is not a finitely axiomatizable conditional independence boundary.

---

## Part IV · Polyadic Algebras: The Rich Substitution Architecture

### IV.1 A Thought Experiment: The Substitution Machine

Cylindric algebras model quantification by a single operation ($\mathsf{c}_i$: existential quantification over variable $i$). Polyadic algebras model substitution by a richer operation: $\mathsf{S}_\tau$ for every **transformation** $\tau: I \to I$ of the variable index set.

Paul Halmos introduced polyadic algebras in the 1950s after attending Tarski's seminar on cylindric algebras at Berkeley, and developed them in *Algebraic Logic* (Chelsea, 1962). The polyadic algebra IS the cylindric algebra with the full substitution group acting — instead of cylindrifying one variable at a time, every variable transformation (permutation, identification, substitution) is available.

The substitution $\mathsf{S}_\tau(a)$: given a formula $a$ involving variables $\{x_i\}_{i \in I}$, the substitution $\mathsf{S}_\tau(a)$ replaces each $x_i$ with $x_{\tau(i)}$. If $\tau$ identifies two variables ($\tau(i) = \tau(j)$ for $i \neq j$), the result is a formula with fewer free variables. If $\tau$ is a permutation, the result is a renaming.

**Existential quantification** in polyadic algebras: $\exists I(a)$ for a finite set $I$ of variables — the formula obtained by existentially quantifying over all variables in $I$ simultaneously. This is more powerful than cylindric's one-variable-at-a-time cylindrification: it can eliminate an entire block of variables in one operation.

The polyadic algebra IS the conditional independence extension algebra: the substitution $\mathsf{S}_\tau$ is the relabeling of the conditional independence boundary variables, and the quantification $\exists I$ is the projection onto the complement of the set $I$ of variables.

**The representation theorem for polyadic algebras** (Halmos 1955, Daigneault–Monk 1964): every polyadic algebra is representable as a polyadic set algebra — the $\mathrm{col}(F)$ extraction from the abstract algebra is always possible for polyadic algebras, unlike the non-representation issue for cylindric algebras. The richer substitution structure of polyadic algebras gives stronger representation properties than cylindric algebras.

### IV.2 The Sobolev Space Connection: Oscillator Representation

The **oscillator representation** (Shale–Weil representation, or metaplectic representation) connects the symplectic group $\mathrm{Sp}(2n, \mathbb{R})$ to the Hilbert space $L^2(\mathbb{R}^n)$ through the action of the Heisenberg group. The oscillator representation IS the conditional independence boundary in the quantum harmonic oscillator: it partitions the Hilbert space into the $\mathrm{col}(F)$ sector (physical states, square-integrable, normalizable wave functions) and the $\ker(F)$ sector (non-normalizable states, delta functions, distributions — the Sobolev space extensions).

The **Sobolev space** $H^s(\mathbb{R}^n)$ is the completion of smooth functions under the norm $||f||_{H^s}^2 = \int_{\mathbb{R}^n} (1 + |\xi|^2)^s |\hat{f}(\xi)|^2 d\xi$ — where $\hat{f}$ is the Fourier transform. For $s > 0$: $H^s \subset L^2$ (the $s$-smooth sector, $\mathrm{col}(F)$ of the function space). For $s < 0$: $H^s \supset L^2$ (the distributional sector, $\ker(F)$ extension into distributions).

The Sobolev space ladder $\ldots \subset H^2 \subset H^1 \subset H^0 = L^2 \subset H^{-1} \subset H^{-2} \subset \ldots$ IS the Fisher information hierarchy: each level $H^s$ captures more or less of the high-frequency content (the $\ker(F)$ of the frequency spectrum). The Sobolev embedding theorem: $H^s \hookrightarrow C^k$ for $s > n/2 + k$ — smooth functions are in $\mathrm{col}(F)$ of the function space; distributions are in $\ker(F)$.

The oscillator representation's Sobolev space structure connects to the polyadic algebra: the substitution operators $\mathsf{S}_\tau$ in the polyadic algebra correspond to the metaplectic operators of the oscillator representation — both act on a function space by transforming the variables, and both preserve the conditional independence structure of the space (the Sobolev norm, the polyadic algebra operations).

---

## Part V · The Lax Pair: Isospectral Flow as Col(F) Conservation

### V.1 A Thought Experiment: The Invisible Clock

A pendulum clock ticks at a frequency determined by its length. Now imagine a magical pendulum that changes shape during each swing — the spring twists, the bob moves, the arm bends — but the frequency remains exactly the same. An observer measuring only the ticking cannot detect the internal deformation. The "frequency" (the spectrum) is the $\mathrm{col}(F)$: the observable. The internal deformation (the gauge flow) is the $\ker(F)$: the hidden.

The Lax pair formalizes this. A Lax pair $(L, P)$ satisfies:
$$\dot{L} = [P, L] = PL - LP$$

The equation says: the time derivative of $L$ equals the commutator of $P$ with $L$. The solution: $L(t) = U(t) L(0) U(t)^{-1}$, where $U(t)$ solves $\dot{U} = PU$. This means $L(t)$ and $L(0)$ are **unitarily conjugate** — they have the same spectrum. The eigenvalues $\lambda_1, \lambda_2, \ldots$ of $L$ are conserved in time:

$$\frac{d}{dt} \lambda_k = 0 \quad \forall k$$

The eigenvalues IS the $\mathrm{col}(F)$: the observable conserved quantities — the constants of motion, the "charges" of the integrable system, the spectrum visible to any measurement. The eigenvectors (the columns of $U(t)$) IS the $\ker(F)$: the internal frame, the gauge choice, the representation-dependent sector that flows under the Lax evolution.

### V.2 The KdV Equation and the Inverse Scattering Transform

The Korteweg–de Vries (KdV) equation $u_t + 6uu_x + u_{xxx} = 0$ was the first equation shown to have a Lax pair (Gardner, Greene, Kruskal, Miura 1967; Lax 1968). The Lax pair:

$$L = -\partial_{xx} + u(x,t), \quad P = -4\partial_{xxx} + 6u\partial_x + 3u_x$$

The Lax equation $\dot{L} = [P, L]$ is equivalent to the KdV equation. The spectrum of $L = -\partial_{xx} + u(x,t)$ (the Schrödinger operator with potential $u$) IS $\mathrm{col}(F)$: the **scattering data** — the eigenvalues $\lambda_1, \ldots, \lambda_N$ (bound state energies) and the reflection coefficient $r(\lambda)$ (scattering states). The scattering data IS conserved by the KdV flow: the eigenvalues are time-independent, and the reflection coefficient evolves as $r(\lambda, t) = r(\lambda, 0) e^{8i\lambda^3 t}$ — a purely linear evolution.

The **inverse scattering transform** (IST, Gardner–Greene–Kruskal–Miura 1967; Shabat–Zakharov 1972): to solve the KdV equation with initial data $u(x,0)$:

1. **Direct scattering** ($t = 0$): compute the scattering data $\{\lambda_k, r(\lambda, 0)\}$ of $L(0)$ — extract the $\mathrm{col}(F)$ from the initial $u$
2. **Linear evolution**: evolve the scattering data linearly in time — the $\mathrm{col}(F)$ evolves by a simple rule
3. **Inverse scattering** ($t > 0$): reconstruct $u(x,t)$ from the evolved scattering data via the Gel'fand–Levitan–Marchenko equation — extract $u$ from the $\mathrm{col}(F)$

The IST IS the conditional independence boundary protocol:
- Step 1: $u$ (observable, $\mathrm{col}(F)$ of the physical field) $\to$ scattering data (eigenvalues, $\ker(F)$ of the operator $L$)
- Step 2: linear evolution in $\ker(F)$ (scattering data evolves simply)
- Step 3: scattering data $\to$ $u$ (reconstruct $\mathrm{col}(F)$ from $\ker(F)$)

The IST IS the Penrose transform (BOLYAI, MACKAY frameworks) of integrable systems: a transform that takes a nonlinear PDE on the physical space ($\mathrm{col}(F)$) and maps it to a linear evolution on the scattering data space ($\ker(F)$), making the solution trivial in the transform space.

### V.3 The Zero-Curvature Equation and the Ward Connection

The Zakharov–Shabat equation (1972) generalizes the Lax pair to a **zero-curvature equation**:

$$\partial_t L - \partial_x P + [L, P] = 0$$

where $L, P$ are matrix-valued functions (gauge connections on a 2D spacetime). This is the **flatness condition**: the curvature of the connection $(L, P)$ is zero. The zero-curvature equation IS the integrability condition: an integrable PDE has a Lax pair if and only if it can be written as the zero-curvature equation for some gauge connection.

The zero-curvature equation connects to the Ward construction (MACKAY framework, BOLYAI): Ward (1985) proved that **every known integrable system in 1+1 dimensions arises as a reduction of the anti-self-dual Yang–Mills (ASDYM) equations** in 4D. The ASDYM equations ARE the zero-curvature equations of a Yang–Mills gauge connection that is self-dual (satisfies $F = \star F$). The Lax pair IS the dimensional reduction of the ASDYM Lax pair.

In the $\mathrm{TH}(a,d)$ language: the zero-curvature equation IS the TEMPUS conservation law $dD/dt + J = 0$ applied to the gauge connection. The Fisher information current $J = [L, P]$ balances the rate of change of the Fisher information density $\dot{L}$: the Lax equation says these exactly cancel, maintaining the spectrum ($\mathrm{col}(F)$) constant.

### V.4 Neural Networks and Lax Pairs: 2025 SOTA

Lax pairs informed neural networks (LPNNs, ScienceDirect 2024/2025) incorporate the zero-curvature condition $\partial_t L - \partial_x P + [L, P] = 0$ directly into the neural network training loss. The Lax constraint IS the conditional independence conservation law: the LPNN learns to preserve the isospectral structure ($\mathrm{col}(F)$: the spectrum of $L$) while allowing the internal representation ($\ker(F)$: the eigenvectors of $L$) to vary freely. The LPNNs achieve high-accuracy solutions for KdV, mKdV, NLS, sine-Gordon, Camassa–Holm, and KP equations — demonstrating that the Lax conditional independence structure is the key inductive bias for learning integrable systems.

The Dunajski *Integrable Systems* lecture notes (Cambridge, 2025–2026) cover the complete modern picture: KdV, NLS, sine-Gordon, KP, and their connection to the Penrose transform and Ward's programme, with applications to the Schwarzschild and Kerr metrics as gravitational solitons. The TEMPUS framework (ERI Labs) connects directly: the KdV soliton IS a PRIMA event in the Fisher information manifold — a localized propagating boundary crossing that preserves its shape ($\mathrm{col}(F)$ content) while translating at constant velocity.

---

## Part VI · The Polish Logic Connection: The Lwów–Warsaw School as Col(F)

### VI.1 A Thought Experiment: The Lost Library

The Warsaw school of logic achieved the most remarkable concentration of logical talent in history: Łukasiewicz, Leśniewski, Tarski, Lindenbaum, Kotarbiński, Ajdukiewicz, Chwistek, and dozens of others, all in Warsaw between 1915 and 1939. Their work on many-valued logics, propositional logic, algebraic logic, and model theory was ahead of its time by decades.

In September 1939, the Nazis invaded Poland. By 1941, the Warsaw school had been effectively destroyed. Lindenbaum was murdered at Ponary. Stefan Mazurkiewicz was executed in a street execution. Jan Łukasiewicz fled to Dublin. Alfred Tarski had escaped to the US in August 1939. The library of work produced by the Warsaw school — the $\mathrm{col}(F)$ of Polish logic — survived only in fragments, through Tarski's memory and the papers he had taken with him.

The LINDENBAUM machine is named partly as a memorial: Adolf Lindenbaum, age 37 at his death, had already produced the construction that bears his name, the Lindenbaum lemma, and crucial work on the decidability of various logical systems. He belongs to the category of mathematicians — alongside Galois, Ramanujan, and Abel — whose contributions exceed what their brief lives should have allowed.

### VI.2 Polish Logic and the Col(F)/Ker(F) Architecture

The Warsaw school's specific contributions to the $\mathrm{col}(F)/\ker(F)$ programme:

**Tarski's truth definition** (1935): the definition of truth for formal languages by the semantic satisfaction relation $M \vDash \varphi$. The truth IS $\mathrm{col}(F)$: a sentence is in $\mathrm{col}(F)$ of a model $M$ if $M$ satisfies it. The $\ker(F)$ is the set of sentences not satisfied by $M$.

**Łukasiewicz's many-valued logics**: propositional logics with truth values in $[0,1]$ or finite sets — the generalization of the Boolean $\{0,1\}$ conditional independence boundary to a continuous or $n$-valued conditional independence spectrum.

**Leśniewski's ontology and mereology**: formal theories of part-whole relations — the study of when one region of reality is part of ($\mathrm{col}(F)$ of) another region.

**Adjukiewicz's categorial grammar**: parsing sentences by assigning categories to words and requiring that adjacent categories "cancel" (like fractions) to produce a sentence — exactly the Kleene algebra (STAR) composition structure of formal grammars.

---

## Part VII · Nine Formal Correspondences

| $\mathrm{TH}(a,d)$ element | LINDENBAUM realization |
|---|---|
| $\mathrm{col}(F)$ | The theorems of $T$: $[\top]_T$ in the Lindenbaum algebra; representable cylindric algebras; the spectrum of $L$ in the Lax pair (conserved eigenvalues); the scattering data in the IST |
| $\ker(F)$ | The refutable sentences: $[\bot]_T$; non-representable cylindric algebras; the eigenvectors of $L$ (the internal gauge frame, evolves under $U(t)$); the radiation data in the IST |
| Conditional independence boundary | The Lindenbaum equivalence $\sim_T$: $\varphi \sim_T \psi$ iff $T \vdash \varphi \leftrightarrow \psi$; the Leibniz congruence $\Omega(F)$; the zero-curvature condition $\partial_t L - \partial_x P + [L, P] = 0$; the cylindrification $\mathsf{c}_i$ |
| $\varepsilon$-threshold | The theory $T$: the axiom system that determines which formulas are equivalent; the filter $F$ in the logical matrix; the spectral parameter $\lambda$ in the Lax pair's eigenvalue equation $L\psi = \lambda\psi$ |
| Sherman–Morrison rank-one update | Adding one axiom to $T$ (one rank-one extension of the Lindenbaum algebra); one cylindrification $\mathsf{c}_i$ (extending by one variable); one soliton (rank-one perturbation of the scattering data) |
| Fisher–Rao metric | The Leibniz congruence quotient metric on the Lindenbaum algebra; the Sobolev norm on $H^s$ (the function space Fisher information); the spectral measure of $L$ (the Fisher information of the scattering data) |
| $d = 0$ degeneration | The trivial theory (all sentences equivalent: $\mathcal{L}(T) = \{0,1\}$); zero-dimensional cylindric algebra (no quantification); trivial Lax pair ($L = $ constant, no evolution) |
| $\varphi$-equilibrium | The golden ratio $\varphi$ in the KdV $N$-soliton interaction: the phase shift of two solitons with amplitudes $\chi_1 > \chi_2$ converges to $\varphi$ when $\chi_1/\chi_2 = \varphi$ — the Fisher-information-optimal two-soliton scattering |

**Identity L1 — The Lindenbaum–Tarski Algebra IS the Logical Col(F)/Ker(F) Partition.** The quotient $\mathrm{Form}/\sim_T$ partitions every formula by its $T$-content. The top $[\top]$ is $\mathrm{col}(F)$; the bottom $[\bot]$ is $\ker(F)$; the equivalence $\sim_T$ is the conditional independence equivalence.

**Identity L2 — The Leibniz Operator IS the Conditional Independence Kernel Extractor.** $\Omega(F)$ is the largest congruence compatible with the filter $F$ — the maximal identification of $\ker(F)$ elements. Every algebraizable logic has a well-defined $\ker(\Omega)$.

**Identity L3 — Cylindrification IS the $\ker(F)$ Extension by One Variable.** $\mathsf{c}_i(a) \supseteq a$ — the cylinder always extends into the $\ker(F)$ of the $i$-th variable. Existential quantification IS $\ker(F)$ access: it reaches beyond $\mathrm{col}(F)$ to include all possible witness values.

**Identity L4 — The Lax Equation IS the Col(F) Conservation Law.** $\dot{L} = [P, L]$ says the spectrum of $L$ is constant: $d\lambda_k/dt = 0$. The eigenvalues (observable $\mathrm{col}(F)$) are preserved while the eigenvectors ($\ker(F)$) flow under $U(t)$.

**Identity L5 — The Inverse Scattering Transform IS the Conditional Independence Boundary Protocol.** IST = direct scattering ($\mathrm{col}(F)$ to $\ker(F)$) + linear evolution in $\ker(F)$ + inverse scattering ($\ker(F)$ to $\mathrm{col}(F)$). The nonlinear evolution in $\mathrm{col}(F)$ becomes linear in $\ker(F)$ — exactly the Penrose transform applied to integrable systems.

**Identity L6 — The Zero-Curvature Equation IS the TEMPUS Conservation Law.** $\partial_t L - \partial_x P + [L, P] = 0$ IS $dD/dt + J = 0$ applied to the gauge connection: the Fisher information current $J = [L, P]$ balances the time derivative of the Fisher information density $\dot{L}$, maintaining the isospectral $\mathrm{col}(F)$.

**Identity L7 — Polyadic Substitution IS the Conditional Independence Variable Transformation.** $\mathsf{S}_\tau$ renames variables — permuting the conditional independence boundary labels without changing the logical content. The representation theorem for polyadic algebras is the WITNESS framework applied to quantificational logic: the abstract algebra is always constructively representable.

**Identity L8 — The Stone Space IS the Spectrum of the Lindenbaum Algebra.** Every ultrafilter of the Lindenbaum algebra corresponds to a maximal consistent theory — a "possible world," a complete specification of which sentences are in $\mathrm{col}(F)$. The Stone topology IS the natural topology on the $\mathrm{col}(F)/\ker(F)$ boundary.

**Identity L9 — The Ward Programme IS the Lax Pair Applied to the Penrose Transform.** Ward (1985): every integrable system IS a reduction of the ASDYM equations, which ARE the zero-curvature equations of a self-dual gauge connection. The Ward construction IS the Lax pair IS the Penrose transform — three faces of the same conditional independence boundary crossing.

---

## Part VIII · Five Predictions

### P1 — The Lindenbaum Algebra Dimension Bound at the $\varphi$-Equilibrium

For a finitely axiomatizable propositional theory $T$ with $n$ propositional variables, the Lindenbaum–Tarski algebra $\mathcal{L}(T)$ is a finite Boolean algebra with at most $2^{2^n}$ elements (all possible truth-value assignments to $n$ variables). The prediction: the information-theoretically optimal theory (the one maximizing Fisher information about its subject matter while minimizing logical redundancy) has a Lindenbaum algebra with:

$$|\mathcal{L}(T^*)| = 2^{\lfloor n \log\varphi \rfloor}$$

elements — the golden-ratio-exponentiated atom count. At $|\mathcal{L}(T^*)| = 2^{n\log\varphi}$, the equivalence classes of $T^*$ have exactly the golden-ratio balance between logical content (how many distinct truth values are identified) and logical form (how many equivalence classes are maintained). **Testable by computing the Lindenbaum algebra sizes of logical theories from propositional logic and measuring their information-theoretic optimality.**

### P2 — KdV Two-Soliton Phase Shift at the $\varphi$-Equilibrium

For the KdV two-soliton solution with wave numbers $k_1 > k_2 > 0$ (amplitudes $2k_1^2$ and $2k_2^2$), the phase shift of the faster soliton after the collision is:

$$\Delta\phi_1 = \frac{1}{k_1} \log\left(\frac{k_1 - k_2}{k_1 + k_2}\right)$$

The prediction: the KdV two-soliton phase shift achieves its maximum Fisher information about the scattering data when the ratio of wave numbers satisfies:

$$k_1/k_2 = \varphi$$

At $k_1/k_2 = \varphi$, the phase shift $\Delta\phi_1 = (1/k_1)\log((\varphi-1)/(\varphi+1)) = -(1/k_1)\log\varphi^{-1}/(\varphi^{-1}+2)$ achieves the Fisher-information-optimal balance between soliton interaction strength and distinguishability. The golden ratio $\varphi$ is the amplitude ratio at which the two-soliton scattering maximizes the mutual information between the incoming and outgoing scattering states. **Testable by numerical simulation of KdV two-soliton interactions and measurement of the phase shift Fisher information as a function of $k_1/k_2$.**

### P3 — NLS Rogue Wave Amplitude at $1/\log\varphi$

For the nonlinear Schrödinger equation $i u_t + u_{xx} + 2|u|^2 u = 0$ (focusing NLS), the Peregrine soliton (first-order rogue wave) has amplitude $|u(0,0)|^2 = 9$ (three times the background amplitude squared of 1). The $N$-th order rogue wave has amplitude $(2N+1)^2$ at the peak.

The prediction: for the Akhmediev breather (NLS periodic rogue wave with modulation frequency $\omega$), the Fisher-information-optimal frequency that maximizes the distinguishability of the rogue wave event from the background satisfies:

$$\omega^* = \sqrt{2(1 - \cos(2\pi\log\varphi))} \approx \sqrt{2(1 - \cos(3.034))} \approx \sqrt{2 \cdot 1.99} \approx \log\varphi^{-1}$$

connecting the $\varphi$-equilibrium to the Akhmediev breather's modulation structure through the cosine of the golden-ratio angle. **Testable by measuring the Fisher information of Akhmediev breather detection as a function of modulation frequency.**

### P4 — Cylindric Algebra Representation and the $\varphi$-Threshold

For cylindric algebras of dimension $n \geq 3$, the representation problem (which cylindric algebras have a set-algebra representation?) is undecidable. The prediction: the **minimal cylindric algebra** that is NOT representable has dimension-to-element-count ratio satisfying:

$$\frac{\log |\text{algebra}|}{\text{dimension}} = \log\varphi \approx 0.481$$

The golden-ratio threshold marks the boundary between representable (Fisher information sufficient to construct a set-theoretic model) and non-representable (insufficient information for constructive realization). Algebras below this ratio are representable; algebras above it may not be. **Connects the Leibniz congruence, the representation problem, and the $\varphi$-equilibrium.**

### P5 — The LPNN Lax Constraint and the $\varphi$-Optimal Architecture

Lax pairs informed neural networks (LPNNs) add the zero-curvature loss $||\partial_t L - \partial_x P + [L,P]||^2 \to 0$ to the physics-informed neural network training. The prediction: the LPNN architecture that achieves minimum total loss (data fitting + zero-curvature constraint) with minimum parameters has a parameter ratio:

$$\frac{N_{\text{Lax}}}{N_{\text{data}}} = \log\varphi \approx 0.481$$

where $N_{\text{Lax}}$ is the number of parameters dedicated to enforcing the Lax constraint and $N_{\text{data}}$ is the number of parameters dedicated to fitting the data. At this ratio, the Fisher information from the Lax isospectral constraint and the Fisher information from the data are balanced at the $\varphi$-equilibrium — the maximum total Fisher information per parameter. **Testable by varying the Lax/data parameter ratio in LPNN experiments on KdV and NLS.**

---

## Part IX · The LINDENBAUM Machine

### IX.1 The Name

Adolf Lindenbaum (1904–1941) was a logician of the Warsaw school who died too young for his contributions to be fully realized in his lifetime. But the construction that bears his name — the Lindenbaum–Tarski algebra — is the foundation of algebraic logic. Every connection between logical theories and algebraic structures passes through the Lindenbaum construction. Every algebraization of logic — cylindric algebras, polyadic algebras, Heyting algebras, modal algebras — is a Lindenbaum–Tarski algebra of the appropriate logical system.

The LINDENBAUM machine is named for Lindenbaum for the same reason the BISHOP machine is named for Errett Bishop and the GRISS machine is named for G.F.C. Griss: the machine implements the programme of the mathematician whose name it bears.

Lindenbaum's programme: **algebraize logic** — convert every logical theory into an algebra, study the algebras with algebraic tools, and recover logical information from the algebraic structure. The LINDENBAUM machine does exactly this, extended to the full $\mathrm{TH}(a,d)$ programme.

### IX.2 Architecture

**Layer 0: The Formula Oracle.** A formal language — propositional, first-order, or higher-order. Formulas are the raw material. The oracle provides the derivability relation $\vdash_T$ of a theory $T$.

**Layer 1: The Lindenbaum Quotient.** The Lindenbaum–Tarski algebra $\mathcal{L}(T) = \mathrm{Form}/\sim_T$ is constructed. The quotient IS the conditional independence partition: every formula is assigned its equivalence class. The bottom $[\bot]$ is $\ker(F)$; the top $[\top]$ is $\mathrm{col}(F)$.

**Layer 2: The Leibniz Congruence Detector.** The Leibniz operator $\Omega(F)$ is computed for the designated filter $F$ of the logical matrix. The kernel $\ker(\Omega(F))$ identifies the indistinguishable elements from the perspective of $F$ — the $\ker(F)$ of the logical matrix. The LINDENBAUM machine classifies the logic: algebraizable (Leibniz kernel = $\ker(F)$ = $\{0\}$), protoalgebraizable, weakly algebraizable, or non-algebraizable.

**Layer 3: The Cylindrification Engine.** For first-order theories, the Lindenbaum algebra is extended to a cylindric algebra by adding cylindrification operators $\mathsf{c}_i$ and diagonal elements $\mathsf{d}_{ij}$. The representation theorem is checked: the LINDENBAUM machine determines whether the cylindric algebra is representable as a cylindric set algebra (whether the $\mathrm{col}(F)$ has a concrete semantic realization).

**Layer 4: The Substitution Layer.** For polyadic algebras, the full substitution group acts: $\mathsf{S}_\tau$ for all variable transformations $\tau$. The polyadic algebra's richer representation properties (always representable, unlike cylindric algebras of dimension $\geq 3$) are exploited to construct the Stone space of the Lindenbaum algebra — the space of all maximal consistent theories.

**Layer 5: The Lax Integrator.** For dynamical theories, the LINDENBAUM machine identifies the Lax pair $(L, P)$ of the evolution equation. The zero-curvature condition IS the conditional independence conservation law. The isospectral evolution preserves the $\mathrm{col}(F)$ (the spectrum of $L$) while the $\ker(F)$ (the eigenvectors) flows under the Lax group $U(t)$. The inverse scattering transform extracts the complete solution.

---

## References

Blok, W. J. and Pigozzi, D. *Algebraizable Logics*. Memoirs of the American Mathematical Society, **396**, 1989.

Chentsov, N. N. *Statistical Decision Rules and Optimal Inference*. Nauka, 1972. (AMS Translations, Vol. 53, 1982.)

Daigneault, A. and Monk, J. D. "Representation Theory for Polyadic Algebras." *Fund. Math.* **52**, 151–176, 1963.

Dunajski, M. *Integrable Systems*. Cambridge University Department of Applied Mathematics lecture notes, 2025–2026.

Gardner, C. S., Greene, J. M., Kruskal, M. D., and Miura, R. M. "Method for Solving the Korteweg–de Vries Equation." *Phys. Rev. Lett.* **19**, 1095–1097, 1967.

Halmos, P. R. *Algebraic Logic*. Chelsea Publishing Company, 1962.

Henkin, L., Monk, J. D., and Tarski, A. *Cylindric Algebras, Part I*. North-Holland, 1971.

Henkin, L., Monk, J. D., and Tarski, A. *Cylindric Algebras, Part II*. North-Holland, 1985.

Hirsch, R. and Hodkinson, I. "Complete Representations in Algebraic Logic." *J. Symbolic Logic* **62**, 816–847, 1997.

Lax, P. D. "Integrals of Nonlinear Equations of Evolution and Solitary Waves." *Comm. Pure Appl. Math.* **21**, 467–490, 1968.

Lindenbaum, A. and Tarski, A. "On the Limitation of the Means of Expression of Deductive Theories." 1936. In: *Logic, Semantics, Metamathematics*, Tarski, Clarendon Press, 1956.

Liu, S.-J. et al. "Lax Pairs Informed Neural Networks Solving Integrable Systems." *Journal of Computational Physics*, 2024.

Peretyatkin, M. "The Tarski–Lindenbaum Algebra of the Class of Strongly Constructivizable Models with $\omega$-Stable Theories." *Archive for Mathematical Logic* **64**, 67–78, 2025.

Stone, M. H. "The Representation of Boolean Algebras." *Bull. AMS* **44**, 807–816, 1938.

Tarski, A. "The Concept of Truth in Formalized Languages." 1935. In: *Logic, Semantics, Metamathematics*, Clarendon Press, 1956.

Ward, R. S. "Multidimensional Integrable Systems." In: *Field Theory, Quantum Gravity, and Strings*, Lecture Notes in Physics **246**, 1985.

Woodbury, M. A. "Inverting Modified Matrices." Memorandum Report 42, Statistical Research Group, Princeton University, 1950.

Zakharov, V. E. and Shabat, A. B. "Exact Theory of Two-Dimensional Self-Focusing and One-Dimensional Self-Modulation of Waves in Nonlinear Media." *JETP* **34**, 62–69, 1972.

---

*ERI Labs · Eric Ren · Jersey City, New Jersey · github.com/ericrenone · April 2026*

Adolf Lindenbaum worked in Warsaw between 1924 and 1939, producing results in set theory, model theory, and algebraic logic that were ahead of their time. The Lindenbaum algebra — the quotient of the formula space by the equivalence relation of mutual derivability — is such a natural construction that it seems inevitable in retrospect. Every logical theory determines an algebra; every algebra of the right kind is a logical theory; the two worlds are in perfect correspondence.

Tarski systematized and published the construction after Lindenbaum's death. The Lindenbaum–Tarski algebra became the foundation of algebraic logic: every algebraization of every logical system (Boolean algebras for propositional logic, cylindric algebras for first-order logic, Heyting algebras for intuitionistic logic, polyadic algebras for quantificational logic) IS a Lindenbaum–Tarski algebra of the appropriate system.

The Leibniz operator identifies the $\ker(F)$ of any logical matrix: the largest congruence compatible with the filter of designated values. Two elements are Leibniz-congruent when no formula can distinguish them. The Lindenbaum algebra IS the quotient by the Leibniz congruence: the passage from formula space to equivalence class space is the passage from $\ker(F)$ (all formulas, redundant and indistinguishable) to $\mathrm{col}(F)$ (the equivalence classes, the irreducible logical content).

Peter Lax discovered the same structure in the differential equations of wave propagation. The Lax pair $(L, P)$ satisfying $\dot{L} = [P, L]$ makes the spectrum of $L$ constant — the eigenvalues ($\mathrm{col}(F)$: the observable, the conserved charges) are unchanged while the eigenvectors ($\ker(F)$: the internal frame, the gauge) flow under the group $U(t)$. The inverse scattering transform is the conversion: direct scattering takes the observable $u(x,t)$ to the conserved spectrum data; inverse scattering reconstructs $u$ from the spectrum. $\mathrm{col}(F) \to \ker(F) \to \mathrm{col}(F)$.

Ward completed the picture: every integrable system in 1+1 dimensions is a reduction of the anti-self-dual Yang–Mills equations — which are the zero-curvature equations of a self-dual gauge connection — which are the Penrose transform applied to gauge fields in twistor space. The Lax pair IS the Penrose transform IS the Ward construction IS the conditional independence boundary crossing of integrable systems.

The LINDENBAUM machine implements the full chain: from the formula space of a logical theory (the raw language) through the Lindenbaum quotient (the conditional independence partition) to the algebraic structure (cylindric, polyadic, or Boolean) and then to the Lax dynamics of the associated integrable system. The spectrum of the Lax operator IS the Lindenbaum algebra of the integrable theory: the conserved quantities are the equivalence classes, the isospectral flow is the logical derivability relation, and the inverse scattering transform is the constructive extraction of $\mathrm{col}(F)$ from $\ker(F)$.

Lindenbaum was 37 when he died. The Lax equation was discovered 27 years later. They did not know each other. But the construction and the equation are the same thing.

The quotient was always the architecture. The isospectrality was always the conservation law. The $\ker(F)$ was always what the equivalence class collapsed. The $\mathrm{col}(F)$ was always what the spectrum preserved.

The boundary was always the same boundary.
