coala Enhancement Proposals
===========================

|Metadata|                                   |
|--------|-----------------------------------|
|cEP     |0                                  |
|Version |1.1                                |
|Title   |coala Enhancement Proposals        |
|Authors |Lasse Schuirmann <lasse@gitmate.io>|
|Status  |Active                             |
|Type    |Process                            |

Abstract
--------

This cEP describes the introduction of cEP's (coala Enhancement Proposals) to
the coala community.

cEP's are used to propose and discuss new major features. After specifying
features with a cEP they should be implemented as specified. Unspecified
features should not be implemented.

They are obviously inspired by
[PEP1](https://www.python.org/dev/peps/pep-0001/).

Spelling
--------

As we all know, coala is written with a lower case c. The proper spelling of a
cEP is `cEP-#`.

Invalid ways to express cEP specifications include `CEP-#`, `cEP#` and `cep-#`.

Purpose
-------

cEP's are in place so features in coala will be designed before implementation.
Implementing major features usually happens from a technical perspective and
may lead to not well designed content - developer and user wise. This can
especially save a lot of coding work when big features are written which are
oftentimes not well enough designed initially.

This also makes sure, major features are properly documented.

Structure
---------

Any cEP must at least hold the following information:

- A metadata table in the header.
- An abstract.

Further chapters may be added as needed.

Metadata
--------

The metadata table must hold the following items:

- A **cEP** number. This number is final.
- A **Version** number. Initially proposed cEPs start with 0.1 and raise until
  they get accepted, which bumps the version to 1.0. They may be iterated upon
  using [semantic versioning](http://semver.org/).
- A **Title**.
- The name(s) and e-mail address(es) of the **Authors**.
- A **Status** which may be one of `Proposed`, `Deferred`, `Implementation Due`
  (for code changes), `Active`, `Deprecated` or `Rejected`.
- A **Type** which may be one of `Process` or `Feature`.

The Process
-----------

Any process changes may be initiated by level B decisions as described in
cEP-1.

### Status: Proposed

cEP's can be proposed by any contributor. In order to propose cEP's a pull or
merge request to the cEP git repository is done. The cEP may be reviewed like
any usual coala pull request (level A decision) but must enter the repository
with a `Proposed` state.

If a cEP is not merged it is invalid and has no state.

Follow up states are `Deferred`, `Implementation Due`, `Active` or `Rejected`.

### Status: Deferred

A cEP may be deferred to a later time if it is considered too cumbersome to
implement or depends on other work that is not ready yet.

Follow up states are `Proposed`.

### Status: Implementation Due

Feature requests may be set to this state if they have been discussed and
accepted but are not implemented yet.

Follow up states are `Active` or `Rejected`.

### Status: Active

Any cEP may be in an active state which indicates that it's contents are valid,
maintained and described features are implemented in the latest coala version.

Follow up states are `Deprecated`.

### Status: Deprecated

A cEP may be marked deprecated if its contents are no longer useful to the
community.

### Status: Rejected

A cEP may be rejected if the community determines.

Follow up states are `Proposed`.

Patching cEP's
--------------

cEP's may be changed. If a cEP is changed, the version number has to be
increased according to [semantic versioning](http://semver.org/).

Patching a cEP to a higher version can be done with a B level decision.
