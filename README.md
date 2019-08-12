# Overview

Opencog components dependency graph:

![opencog components dependency graph](https://www.plantuml.com/plantuml/svg/VLFBRiCW4Bpp5Vm0xRtg8LBx0Rr7FQpjBR7CmsMn5AdgltS3JhouJIrPmCmm2plYG1bINhnJAe_PeNw3VWABf8r-YNwE0KFMhoFO15wf_WR5VfwiM6UaF406mam2JkZmhEPggeVOJvZqbzByRQAZZZE6Fjh7TJGT--Xt3NHbBi3TNQL88wzbx-ddI9abr6ovWkfR79_n9OzE83uIoWj2ZfxuVYYm9SdLKOCTJJV6MeuNF6zvAguhJ_iI7P_lv25Diltrq09n22aqjdZEc08uasDqxDwGziJtDLqQ1ywbfHm4kt1SfbYEmJAlIjxwsPWc4PdwBxB68j2QYf0KSkjn6GickxgXjJ6xl7RwsqmMlccVglA1Fft-ID5h3yHD-dlN3hsaoly_YZNQ7RZcsQ9Rfh8tZVSw5go6gmuO1dwhFm00)

[source code](https://www.planttext.com/?text=TPFFRiCW3CRlF0Klm7QVTgYqFS3krGvEuj4e_Cd0aIfLU_Uva3OcMtC1VlviWp_ba0aIBTufHICvr1_GJs0nQwFVefzZm43wVGIRm2lLtr7ivycACs6c0GWoKXOueSEpccjHFSH-mgGlIlEtYOuwpXZwQ9_NrNHSHtzgoBV85JpCAaqQUMtxI3_7J2p9JSeDgXznVUOBZKuG7pFA1m95d_bzADYIvEcemOwc6sDjnmVUj_5iIjbLaFSzEhxWoKEQvFphhGLn22aqTV5Cc08uGp4whju4xOaVRBeq3cnC6t8GxC9-cL9o39RZgXYkNurfB96s_mbMNmIjjWX92Mv3BcjXSgmRhOFP6RRJttUoyLtxKfLF-TlfhnIzzf1vIFzdxUZLrfQiNkxWwbzBDm_bB9fkwrfODLCTC0pyS_u2)

# Merging script

Script automatically merges `opencog` repos to `singnet` forks.

In empty directory execute:
```sh
python merge-opencog-to-singnet.py --github-token <github-token> \
	--circleci-token <circleci-token>
```

## Github API token

Github token is used to:
- read public repositories;
- create forks to keep new branches;
- push merge results;
- raise PRs.

You can create one using your Github account.
Use `Settings/Developer settings/Personal access tokens` menu.
Press `Generate New Token` button.
Set following permissions:
- `repo/public_repo`
- `admin:org/read`
Generate new token.

## CircleCI token

TODO
