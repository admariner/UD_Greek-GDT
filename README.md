# Summary

The Greek UD treebank (UD_Greek-GDT) is derived from the Greek Dependency Treebank
(http://gdt.ilsp.gr), a resource developed and maintained by
researchers at the Institute for Language and Speech Processing/Athena
R.C. (http://www.ilsp.gr).

# Introduction

The Greek UD treebank consists of 2,521 sentences (61,673 tokens). The
data in the current release derive from primary texts that are in the
public domain, including wikinews articles and european parliament
sessions. The treebank is licensed under the terms of [Creative
Commons Attribution-NonCommercial-ShareAlike, CC BY-NC-SA
3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/).

The morphological and syntactic annotation of the Greek UD treebank
was originally created through a semi-automatic conversion of
PDT-style annotations in GDT data. The syntactic annotation of the 2.1
release was generated by manual corrections of several constructions
of the UD annotation, which is now the only manual syntactic
annotation used for new data added to the resource. The harmonization
with UD v2 is work in progress.

# Acknowledgments

We wish to thank all contributors to the original annotation
efforts. A large part of those annotations was work by students of the
postgraduate programme Technoglossia IV, organised by the Institute
for Language and Speech Processing, the University of Athens and the
National Technical University of Athens.

## References

* Prokopis Prokopidis and Haris Papageorgiou. Universal Dependencies for Greek. In Proceedings of the NoDaLiDa 2017 Workshop on Universal Dependencies (UDW 2017), pages 102-106, Gothenburg, Sweden, May 2017.

* Prokopis Prokopidis, Elina Desypri, Maria Koutsombogera, Haris Papageorgiou, and Stelios Piperidis. Theoretical and Practical Issues in the Construction of a Greek Dependency Treebank. In Montserrat Civit, Sandra Kubler, and Ma. Antonia Marti, editors, Proceedings of The Fourth Workshop on Treebanks and Linguistic Theories (TLT 2005), pages 149-160, Barcelona, Spain, December 2005. Universitat de Barcelona.

# Data splits

- Train/dev/test sets: 1662/403/456 sentences, 41212/10139/10422 tokens

# Changelog

* 2024-11-15 v2.15
  * Fixed wrong dependency labels that lead to leaf-det-clf errors
  * Fixed errors in lemma annotations

* 2023-05-15 v2.12
  * Converted `parataxis` to `ccomp` in reported speech constructions
  * Changed upos to DET for pronouns functioning as determiners
  * Fixed errors in lemma annotations of uppercase words
  * Fixed xpos errors for MWTs

* 2019-11-15 v2.5
  * Fixed issues concerning constructions with the `orphan` relation

* 2019-05-15 v2.4
  * Fixed upos in cases related to the `AUX`-for-`aux` constraint
  * Fixed issues concerning punctuation (most of them related to punctuation creating non-projectivity)

* 2018-11-15 v2.3
  * Added nsubj:pass, csubj:pass subtypes to relevant subject nodes
  * Added obl:agent subtypes to agents of passive verbs

* 2018-04-15 v2.2
  * Repository renamed from UD_Greek to UD_Greek-GDT.
  * Fixed issues concerning specific constructions (most of them related to `flat` in multi-token names and to `parataxis` in reported speech)

* 2017-11-15 v2.1
  * Fixed issues concerning specific constructions (most of them related to deprels of pronouns and to oblique dependents in constructions with copulas)

* 2017-03-01 v2.0
  * Semi-automatic conversion to UD v2.0
  * New data split into train/dev/test sets

* 2016-11-15 1.4
  * Fixed issues in conversion of POS for articles

* 2016-05-15 v1.3
  * Added PronType and NumType attribute/value pairs to certain types of determiners and numerals
  * Improved conversion of abbreviations

* 2015-11-15 v1.2
  * Fixed issues in conversion of determiner pos and adjective degree

* 2015-05-15 v1.1
  * Initial release of automatic conversion to UD

<pre>
=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v1.1
License: CC BY-NC-SA 3.0
Includes text: yes
Genre: news wiki spoken
Lemmas: manual native
UPOS: converted from manual
XPOS: converted from manual
Features: converted from manual
Relations: converted with corrections
Contributors: Prokopidis, Prokopis
Contributing: elsewhere
Contact: prokopis@ilsp.gr
===============================================================================
</pre>
