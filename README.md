# mech-sax

A mechanization of the proof theory of the semi-axiomatic sequent calculus
(SAX) in the proof assistant Beluga. The translation between SAX and the
standard sequent calculus G3 is mechanized for the full SAX system. The
proofs of cut admissibility, cut elimination, and the subformula property
are mechanized for Soprillo, a fragment of SAX covering identity,
implication, tensor, and snips.

## Prerequisites

- [Beluga](https://github.com/Beluga-lang/Beluga) (latest version)

## Structure

The mechanization is located in the `beluga/` directory and consists of
the following files:
- `sax.bel` — LF encoding of the SAX rules
- `labeled.bel` — LF encoding of Soprillo with eligibility
- `equiv.bel` — translation between SAX and the standard sequent calculus G3
- `cut-admis.bel` — mechanized proofs of cut admissibility and cut elimination 
- `subformula.bel` — mechanized proof of the subformula property

## Running

From the root of the repository, run:
```
beluga beluga/proj.cfg
```
