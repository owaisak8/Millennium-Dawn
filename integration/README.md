# Millennium Dawn integration notes

The Mauritania submod relies on two shared Millennium Dawn files for date-sensitive party names:

1. `common/scripted_localisation/00_MD_politicsview_scripted_localisation.txt`
2. `localisation/english/MD_politics_view_parties_l_english.yml`

The branch `mauritania-complete-v1.0.0` contains edits to both files. These are changes to the Millennium Dawn base, not files that can safely be dropped into a separate submod: they extend shared localisation definitions and the full existing party localisation file must be preserved.

**Recommended installation:** merge the Mauritania integration PR into the Millennium Dawn fork, then enable the country-content submod ZIP.

If you use an unmodified Steam Workshop copy of Millennium Dawn, the country content can be loaded as a submod, but the Action for Change and MITHAQ party labels will not display correctly until those two shared-file additions are applied to the base mod. Do not copy a shortened or partial replacement over either shared file.
