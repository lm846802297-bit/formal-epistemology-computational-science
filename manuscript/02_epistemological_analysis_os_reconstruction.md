# 2. The Osterwalder–Schrader Formalization Network

## 2.1. The mathematical setting

The Osterwalder–Schrader programme establishes conditions under which Euclidean field-theoretic data can be related to relativistic quantum field theory. Its Euclidean objects are Schwinger functions; the reconstructed relativistic objects are Wightman functions or distributions. The original OS papers formulate axioms for Euclidean Green functions and develop the corresponding reconstruction theorem (Osterwalder & Schrader, 1973, 1975). Osterwalder and Schrader (1975, pp. 282, 287–288) identify a gap in the 1973 forward proof and leave open there whether E0–E4 alone suffice. Their Section IV reconstruction theorem assumes E0′ together with E1–E4 and yields the output bound R0′.

The mathematical setting is not unique. Glimm and Jaffe (1987) formulate the Euclidean theory in terms of a probability measure on field configurations and its generating functional. The original OS formulation, by contrast, is expressed in terms of Schwinger functions as distributions on an appropriate test-function space. Douglas, Hoback, et al. (2026) choose the Glimm–Jaffe formulation for their Lean formalization because it makes the construction of a Euclidean field theory a problem about a functional measure, a mathematical structure well supported by Mathlib. They explicitly note that this is a variant of the original OS axioms and explain the relationship between their use of Schwartz functions and the compactly supported test functions in the Glimm–Jaffe presentation. Glimm and Jaffe (1987, p. 91, n. 1) also discuss the Schwartz-space extension and the free-field measure on tempered distributions. The three formalization projects considered below should therefore be understood as related representations of the OS programme, not as interchangeable encodings of a single record.

## 2.2. OSforGFF: the probability-measure formulation

OSforGFF (Cherkis et al., 2026) constructs the massive Gaussian free field as a probability measure on the space of tempered distributions \(S'(\mathbb R^D)\), where \(D\geq2\) is the spacetime dimension. The general result applies given a propagator, while a further result supplies the canonical proper-time propagator for every \(D\geq2\). Separate results also give closed-form covariances in dimensions \(D=2,3,4,5\). The constructed measure satisfies the project's Glimm–Jaffe formulation of the OS properties.

The axioms are predicates on the probability measure and its generating functional. OS0 states analyticity of the generating functional in finite collections of complex test-function parameters. OS1 is a regularity condition: there exist \(p\in[1,2]\) and \(c>0\) such that

\[
|Z_\mu(f)| \leq
\exp\left[
c\left(
\int_{\mathbb R^D}|f(x)|\,dx+
\int_{\mathbb R^D}|f(x)|^p\,dx
\right)
\right],
\]

together with a subsidiary local-integrability condition on the two-point function when \(p=2\). For the massive Gaussian free field, the proof uses \(p=2\) and \(c=1/(2m^2)\), and establishes the required two-point condition by identifying the mollified two-point function with the covariance kernel away from coincidence. OS2 expresses invariance under the Euclidean group. OS3 is reflection positivity in a complex generating-functional formulation, with time reflection and complex conjugation. OS4 is represented through clustering and ergodicity; the latter is initially formulated for a specified class of finite exponential functionals and established using a polynomial-clustering estimate.

These choices are not merely notational. The OSforGFF documentation and the accompanying paper explain how the formalized conditions relate to the Glimm–Jaffe presentation. In particular, the use of Schwartz test functions and tempered distributions is stated to imply the corresponding compactly supported test-function formulation, since \(D(\mathbb R^D)\subset S(\mathbb R^D)\) and \(S'(\mathbb R^D)\subset D'(\mathbb R^D)\). The formalized ergodicity condition is initially stated for finite exponential functionals. Douglas et al. (2026, Remark 3.2) explain how density in \(L^1(\mu)\), the \(L^2\)-to-\(L^1\) estimate on a probability space, and invariance of \(\mu\) under time translations extend the time-average result to general integrable observables. This extension is attributed to the authors' argument rather than presented as a direct quotation from the accessible pages of Glimm and Jaffe.

The OS1 condition is particularly relevant to the comparison with OSreconstruction. It is the Glimm–Jaffe exponential regularity bound on the generating functional, with an additional two-point integrability condition. It is not the same predicate as the arity-dependent \(E_0'\) growth condition required by the forward OSreconstruction theorem. The former controls the generating functional in terms of \(L^1\) and \(L^p\) norms of a single test function; the latter is a quantitative estimate on the family of \(n\)-point Schwinger distributions, with Schwartz seminorm orders increasing linearly with \(n\). The shared language of regularity or growth does not establish a mathematical implication between them.

## 2.3. OSreconstruction: zero-diagonal Euclidean data and conditional reconstruction

OSreconstruction (Yin et al., 2026) formalizes reconstruction for every positive spatial dimension \(d\), with spacetime dimension \(d+1\). Its Euclidean input is a family of Schwinger functions acting on the zero-diagonal Schwartz test-function space. Its Wightman distributions act on the full Schwartz space. The zero-diagonal domain is mathematically significant: it accommodates the coincidence singularities of Euclidean Schwinger functions without presupposing that they define distributions on the full Schwartz space.

The Euclidean input satisfies temperedness, linearity and reality on the zero-diagonal test space; translation and connected Euclidean rotation invariance; reflection positivity on Borchers sequences supported in the ordered positive-time region; permutation symmetry; and the cluster property. The forward reconstruction theorem additionally assumes a quantitative growth condition. Schematically, this condition takes the form

\[
\|S_n(f)\|
\leq
\alpha\,\beta^n(n!)^\gamma
\|f\|_{ns,ns},
\]

where \(\alpha\) and \(\beta\) are positive, \(\gamma\) is real, and the Schwartz seminorm orders grow linearly with the arity \(n\). The theorem concludes the existence of a Wightman-function family whose distributions are Wick-paired with the input Schwinger family.

An original-coordinate formulation of the OS-II growth condition requires a positive Sobolev index \(s\) and, for \(n>0\), the estimate

\[
\|S_n(f)\|
\leq
\alpha (n!)^\gamma
\|f\|_{\mathrm{OSII},ns},
\]

where the final seminorm is the original-coordinate seminorm on the zero-diagonal test space. A separate normalization is imposed at \(n=0\). A proved conversion takes this condition to the arity-linear formulation, with the parameter choice

\[
\alpha' = \max\{1,\alpha\},\qquad
\beta'=(d+2)^s,\qquad
\gamma'=\gamma+2s.
\]

The stronger OS-II reconstruction result establishes the existence of a Wick-paired Wightman family, the output growth estimate \(R'_0\), and uniqueness among Wightman families satisfying the same Wick-pairing relation. This uniqueness concerns the distribution family, not all possible physical realizations. The quantitative conversion is part of the mathematical result; it is not an identification based on similar terminology.

The reverse theorem constructs Euclidean Schwinger data from a Wightman-function family and proves the corresponding OS properties for that construction. It does not assume the forward growth condition. The two directions therefore do not form an unconditional biconditional between arbitrary OS data and arbitrary Wightman data. The public endpoint is a family of Wightman distributions satisfying the formalized Wightman-function axioms, including covariance, spectral support, locality, positivity, Hermiticity, and clustering. The subsequent GNS construction of a Hilbert space and operator-valued fields lies outside the scope of this formalization.

The public OSreconstruction package also includes a conditional construction of an OS record from a supplied Wightman family. It does not provide a publicly inspectable concrete example that supplies both the forward OS record and the corrected growth condition. The README reports that a private companion project contains examples for the massive free field and the Proca Wick square. These examples are therefore author-reported; the private proof artifacts are not independently inspectable. The report does not identify the massive-free-field example with the particular probability-measure construction considered in OSforGFF.

## 2.4. Comparator: a formally checked interface between OS records

The OSreconstruction Comparator (Douglas, Yin, et al., 2026) provides an audit representation and a corresponding production representation for the forward, OS-II, and reverse reconstruction results. The two representations are checked separately but share the same underlying mathematical definitions. The Comparator therefore offers a useful example of a formally checked interface without constituting an independently authored physical formalization.

Explicit mappings in both directions preserve the Schwinger-function family and carry the relevant growth assumptions between the two records. They also establish the correspondence between the associated Wick-pairing and output-growth conditions. Under these mappings, the forward, OS-II, and reverse reconstruction statements correspond. The interface is thus more than an informal assertion that the two representations mean the same thing: the correspondence itself is part of the formal mathematical result.

The epistemic scope of this result is limited. Because the two representations share their underlying definitions, the check supports reuse between the corresponding records but does not independently establish that those definitions adequately capture the physical OS framework. The Comparator is therefore a positive example of relative, record-level interface warrant, not an independent derivation or an external validation of the reconstruction theory.

## 2.5. What is and is not connected in the public formalization network

The projects exhibit different kinds of correspondence evidence. For OSforGFF, the authors explain how the probability-measure predicates relate to the Glimm–Jaffe axioms, including the relation between Schwartz and compactly supported test functions and the ergodicity argument. For the Comparator, the correspondence between the audit and production records is itself formally established: the mappings preserve the Schwinger-function family and the relevant growth assumptions, and relate the corresponding reconstruction statements. This is a checked interface between records of common mathematical origin, not an independently developed physical formalism.

Across the public developments considered here, no complete construction has been established that starts from the particular OSforGFF probability measure and supplies both the zero-diagonal Schwinger record and the arity-dependent growth condition required by the OSreconstruction forward theorem. Such a construction would require a map from the measure and generating functional to the relevant Schwinger distributions, a proof that the OS predicates transfer to the zero-diagonal formulation, and a witness for the required growth condition. The absence of such a construction in the public materials considered here is not a claim of mathematical impossibility or of its absence from private work.

The significance of the case does not depend on treating the missing public interface as a defect in either mathematical project. Each project establishes the results it states. The issue is whether, and under what conditions, those results can be composed to support a further scientific claim. This is a question about the warrant of the interfaces between formalizations, not about the validity of the local proofs.
