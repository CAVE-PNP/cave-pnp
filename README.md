# Computer-Aided Verification of Existing P/NP Proof Attempts

The goal of the project is to select a sample of existing papers concerning the P/NP problem
and to have the arguments contained therein checked by a (machine) proof assistant.
The aim is not to find an answer to the open question itself,
but to be capable to examine the "mass" of proposed proofs not only manually, but with machine support.
If the number of suggested proofs grows faster than scientific peer review can assess the work and identify possible errors,
then there is a possibility that the solution is actually found, but is lost in the mass of (incorrect) approaches.
This situation should be counteracted with the support of computers, in particular proof assistants.

## Overview

The publications examined (proof approaches) are selected with respect to the following aspects

1. the rigor of the argumentation,
2. the proof techniques applied,
3. "feasibility" of modeling in proof assistants, and
4. the claimed result of the relation of P to NP (equivalent/distinct/unprovable).

### Expected results

Researchers who deal with the question should be given extended possibilities to subject their ideas and arguments
to a mechanical, and thus objective/independent, examination (before publication).
Independently of it the P/NP question serves thus as "study object",
whose investigation is to advance the possibilities of mechanical proof verification,
as an aid, simplification and objectification of scientific Peer reviews.

### What the project can offer

The project shall bring "help for self-help" to accomplish an independent and objective verification of one's own ideas.
In this respect computers offer attractive advantages, because:

- A computer cannot be convinced by authority, reputation or academic affiliation
- and he is unbiased, without vanity and free from own interests or preferences for arguments, proof techniques, or the similar.

The aim is to objectify and verify formal arguments, especially since scientific peer review may not always be available to laypersons, amateurs, or people from outside the field.

### What we cannot offer

We do not do scientific peer reviews of any submissions, or act as a publication organ.
Likewise, we would not confirm the scientific correctness ourselves, as this would be the task of the computer.
We merely support you on the way to this goal.

## Contribute

Proof file sources for individual P/NP attempts are stored in separate repositories,
but are included as submodules in this one.

To add formalisations, add a new repository to this organization.
[Contact the maintainer](mailto:stefan.rass@jku.at) to request access.

To clone this repository and initialize all submodules, run:

```sh
git clone --recurse-submodules --remote-submodules <url>

# OR

git clone <url>
cd <name>
git submodule update --init --recursive --remote
```

To update all submodules, run:

<!-- TODO check if `git pull --recurse-submodules` updates branches -->

```sh
git submodule update --recursive --remote

# OR

git pull --recurse-submodules
```

Note that submodules are configured with ssh URLs.
In cases where access over HTTPS is required, the following [workaround](https://stackoverflow.com/a/50299434) may be of use:

```sh
git config --global 'url.https://gitlab.aau.at/.insteadOf' 'git@gitlab.aau.at:'
```
