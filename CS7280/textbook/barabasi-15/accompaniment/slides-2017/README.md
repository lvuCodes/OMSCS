# Slides (2017) — Normalization Notes

This directory holds the lecture slide decks accompanying the CS7280 / Network Science textbook. The folder and file layout has been normalized from the original downloaded material. This document records every variance from that original state so the provenance remains traceable.

## Normalization Rules Applied

- **Folder names** standardized to lowercase-kebab in the form `chapter{N}_{topic-name}`. The `_` separates the chapter segment from the topic segment; `-` separates words within the topic segment.
- **Year-bearing file names** restructured to lead with the year as its own segment: `{year}_{remainder}`. The remainder retains all original tokens (no tokens dropped) and is rendered in lowercase-kebab. `camelCase` boundaries in the original names were expanded to hyphens.
- **Scope**: every file whose name embedded a four-digit course year (`2015`–`2017`) was renamed, including files in single-year folders.
- **Non-year files** (video, audio, archives, and other media) were left at their original names.

## Folder Rename Mapping

| Original folder | Normalized folder |
|---|---|
| `CLASS1-Introduction` | [chapter01_introduction](chapter01_introduction) |
| `CLASS2-Graph_Theory` | [chapter02_graph-theory](chapter02_graph-theory) |
| `CLASS3-Random_Networks` | [chapter03_random-networks](chapter03_random-networks) |
| `CLASS4-Scale_Free_Property` | [chapter04_scale-free-property](chapter04_scale-free-property) |
| `CLASS5-BA_Model` | [chapter05_ba-model](chapter05_ba-model) |
| `Chapter6-Evolving_Networks` | [chapter06_evolving-networks](chapter06_evolving-networks) |
| `Chapter7-Degree_Correlations` | [chapter07_degree-correlations](chapter07_degree-correlations) |
| `Chapter8-Robustness` | [chapter08_robustness](chapter08_robustness) |
| `Chapter9-Communities` **+** `CLASS9-Community_Structure` | [chapter09_communities](chapter09_communities) |
| `Chapter10-Spreading_Processes` | [chapter10_spreading-processes](chapter10_spreading-processes) |

### Prefix Reconciliation

The original download used two inconsistent folder-prefix conventions: `CLASS1`–`CLASS5` and `CLASS9` used the `CLASS` prefix, while `Chapter6`–`Chapter10` used the `Chapter` prefix. All ten folders were unified to a single `chapter{N}` convention.

### Chapter 9 Folder Merge

Chapter 9 (Communities) was the only topic that existed under two separate folders in the original download:

- `Chapter9-Communities/` held the 2015 and 2016 decks.
- `CLASS9-Community_Structure/` held the 2017 deck and its PDF.

Both were consolidated into [chapter09_communities](chapter09_communities). The emptied `CLASS9-Community_Structure/` folder (which retained only a `.DS_Store`) was moved to the Trash (recoverable).

## File Rename Mapping

| Folder | Original file | Normalized file |
|---|---|---|
| chapter01_introduction | `CLASS1_2017_NEU.pptx` | `2017_class01-neu.pptx` |
| chapter02_graph-theory | `Class2_2016_theory.pptx` | `2016_class02-theory.pptx` |
| chapter02_graph-theory | `Class2_2017_theory.pptx` | `2017_class02-theory.pptx` |
| chapter02_graph-theory | `Class2_2017_Graphs_QuestionsFormat.pptx` | `2017_class02-graphs-questions-format.pptx` |
| chapter03_random-networks | `Class3_RandomNetworks_2016.pdf` | `2016_class03-random-networks.pdf` |
| chapter03_random-networks | `Class3_RandomNetworks_2016.ppt` | `2016_class03-random-networks.ppt` |
| chapter03_random-networks | `Class3_RandomNetworks_2016_questions.pdf` | `2016_class03-random-networks-questions.pdf` |
| chapter03_random-networks | `Class3_RandomNetworks_2016_questions.ppt` | `2016_class03-random-networks-questions.ppt` |
| chapter03_random-networks → chapter05_ba-model | `Class5_NEU_2016_BAmodel [Autosaved].pptx` | `2016_class05-neu-ba-model-autosaved.pptx` |
| chapter04_scale-free-property | `Class4_SF-2016.pdf` | `2016_class04-sf.pdf` |
| chapter04_scale-free-property | `Class4_SF-2016.pptx` | `2016_class04-sf.pptx` |
| chapter04_scale-free-property | `Class4_SF-Questions-2016.pdf` | `2016_class04-sf-questions.pdf` |
| chapter04_scale-free-property | `Class4_SF-Questions-2016.pptx` | `2016_class04-sf-questions.pptx` |
| chapter05_ba-model | `Class5_NEU_2016_BAmodel.pdf` | `2016_class05-neu-ba-model.pdf` |
| chapter05_ba-model | `Class5_NEU_2016_BAmodel.pptx` | `2016_class05-neu-ba-model.pptx` |
| chapter05_ba-model | `Class5_NEU_2016_BAmodel_newimgs.pdf` | `2016_class05-neu-ba-model-newimgs.pdf` |
| chapter05_ba-model | `Class5_NEU_2016_BAmodel_newimgs.pptx` | `2016_class05-neu-ba-model-newimgs.pptx` |
| chapter06_evolving-networks | `Class6_NEU_2016_EvolvingNetworks.pdf` | `2016_class06-neu-evolving-networks.pdf` |
| chapter06_evolving-networks | `Class6_NEU_2016_EvolvingNetworks.pptx` | `2016_class06-neu-evolving-networks.pptx` |
| chapter07_degree-correlations | `Class_2016_degreee_correlations.pdf` | `2016_class-degreee-correlations.pdf` |
| chapter07_degree-correlations | `Class_2016_degreee_correlations.pptx` | `2016_class-degreee-correlations.pptx` |
| chapter07_degree-correlations | `Class_2017_degree_correlations.pdf` | `2017_class-degree-correlations.pdf` |
| chapter07_degree-correlations | `Class_2017_degreee_correlations.pptx` | `2017_class-degreee-correlations.pptx` |
| chapter08_robustness | `CLASS8-error-attack_2016.pdf` | `2016_class08-error-attack.pdf` |
| chapter08_robustness | `CLASS8-error-attack_2016.pptx` | `2016_class08-error-attack.pptx` |
| chapter09_communities | `Class_2015_CommunityStructure2.pptx` | `2015_class-community-structure02.pptx` |
| chapter09_communities | `Class_2016_CommunityStructure1.pptx` | `2016_class-community-structure01.pptx` |
| chapter09_communities | `Class_2017_CommunityStructure.pdf` | `2017_class-community-structure.pdf` |
| chapter09_communities | `Class_2017_CommunityStructure.pptx` | `2017_class-community-structure.pptx` |
| chapter10_spreading-processes | `CLASS10-2016-Spreading_questions_format.pptx` | `2016_class10-spreading-questions-format.pptx` |

## Content Preserved Verbatim

The following original characteristics were intentionally **not** altered, to preserve fidelity to the source material:

- **Original spelling**: the misspelled token `degreee` (in the chapter 7 file names) was retained exactly as downloaded. Note the source itself was inconsistent — the 2017 PDF used the correct `degree` while the 2017 PPTX used `degreee`.
- **Embedded citation years were not treated as course years.** Tokens such as `Dashun08` (a 2008 reference) and `PRE2002` (Physical Review E, 2002) were left untouched; only delimited four-digit `20xx` course years were promoted to the leading segment.
- **Media and non-year files** retain their original names, including files with spaces or mixed case (for example, `Connected - HOW KEVIN BACON CURED CANCER.m4v`, `Scale invariance in the critical Ising model.mp4`, `Ch4-scalefreeproperty.docx`).

## Oversized-Deck PDF Handling

Several source `.pptx` decks exceed the repository's 30MB file limit and are therefore gitignored and retained locally only. For course use, a compressed single-file PDF under 30MB was produced for each oversized deck (verified complete against the source slide counts; lower page counts reflect hidden slides not exported, not truncation).

An earlier full-resolution export had split two of these decks into `_part-0X.pdf` segments. Those segments were superseded by the compressed single PDFs and, being unreferenced and redundant, were moved to the Trash on 2026-07-15 (recoverable):

| Folder | Removed part files | Superseded by |
|---|---|---|
| chapter04_scale-free-property | `2016_class04-sf_part-01/02/03.pdf` | `2016_class04-sf.pdf` |
| chapter04_scale-free-property | `2016_class04-sf-questions_part-01/02/03.pdf` | `2016_class04-sf-questions.pdf` |
| chapter07_degree-correlations | `2016_class-degree-correlations_part-01/02.pdf` | `2016_class-degree-correlations.pdf` |

## Anomalies Flagged

- **Relocated deck**: `2016_class05-neu-ba-model-autosaved.pptx` is a PowerPoint AutoRecover copy of Chapter 5 (BA Model) content that was found inside the Chapter 3 (Random Networks) folder in the original download. It was moved to its correct topic folder, [chapter05_ba-model](chapter05_ba-model). It remains an AutoRecover artifact rather than an authored deck.
- **Removed temporary file**: an orphaned Microsoft Office lock file, `~$Class_2015_CommunityStructure2.pptx`, was present in the original chapter 9 material. It was a zero-content lock artifact, not a slide deck, and was removed during cleanup (it was cleared automatically by iCloud before manual deletion was required).

## Split Files

Files over 50MB are stored as 45MB byte-split parts in a subfolder named for the file's stem, so each part stays under GitHub's 100MB file limit. The whole copy is kept locally as `<stem>_original.<ext>` and is gitignored. Reassemble from this folder with `cat <folder>/<stem>/<stem>_pt*.part > <folder>/<stem>.<ext>`, for example `cat chapter03_random-networks/erdos/erdos_pt*.part > chapter03_random-networks/erdos.mov`.

| Folder | File | Parts |
|---|---|---|
| (root) | `Background-Rete-preview.mov` | 5 |
| chapter02_graph-theory | `MAURO-HumanPPI-Tedmed.mov` | 2 |
| chapter03_random-networks | `erdos.mov` | 3 |
| chapter03_random-networks | `erdossaund.mov` | 4 |
| chapter04_scale-free-property | `2016_class04-sf.pptx` | 2 |
| chapter04_scale-free-property | `2016_class04-sf-questions.pptx` | 2 |
| chapter07_degree-correlations | `2017_class-degree-correlations.pptx` | 2 |
| chapter10_spreading-processes | `2016_class10-spreading-questions-format.pptx` | 5 |
