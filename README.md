# Mauritania: The Sahelian Republic (v1.0.0)

A Millennium Dawn country-content expansion for Mauritania (MAU). The campaign is grounded in the country's post-2000 political history and links political transitions, resource development, social policy and Sahelian security.

## Included content

- **73 national focuses** across political development, SNIM and iron exports, fisheries, oil and gas, agriculture, electricity, armed forces, regional diplomacy and social development.
- **19 historical and flavour events** covering the 2001 National Assembly election, the 2002 ban on Action for Change, the 2003 coup attempt, the 2005 military takeover, the 2006–2007 transition, the 2008 coup, the 2009 election, anti-slavery legislation, the 2019 transfer of power, the 2024 election and Greater Tortue Ahmeyim gas exports.
- **Native Millennium Dawn political integration**: the existing 24-party slot array, party popularity, party bans, ruling-party changes, government coalitions and the `on_new_term_election` on-action.
- National ideas, 8 decisions, historical AI strategy plans and English localisation.
- Historical leader changes for the main military and civilian transitions.

## Installation

This release is intended for the matching Millennium Dawn 2.0.2 codebase / Hearts of Iron IV 1.19.x.

1. Enable Millennium Dawn.
2. Extract the ZIP directly into the Hearts of Iron IV `mod` directory so the `Mauritania_Sahelian_Republic` folder and `Mauritania_Sahelian_Republic.mod` file sit side by side.
3. Enable the Mauritania submod after Millennium Dawn.

**Important integration requirement:** the matching Millennium Dawn branch must also contain the two shared political-view changes made with this expansion:
- `common/scripted_localisation/00_MD_politicsview_scripted_localisation.txt`
- `localisation/english/MD_politics_view_parties_l_english.yml`

Those are shared Millennium Dawn files. They are deliberately not shipped as replacements inside this submod ZIP, because replacing the complete shared files from a submod would erase other countries' party localisations and political hooks. The accompanying GitHub branch/PR contains the compatible edits. Merge those edits into the Millennium Dawn base before using the package if you are not running the merged branch directly. See `integration/README.md`.

## Historical and gameplay notes

- The 2001 National Assembly seat distribution follows the IPU election record: PRDS 64, Action for Change 4, UDP 3, RFD 3, UFP 3, RDU 3 and Popular Front 1. The seat shares are used as a proxy for party-support weighting in the native MD election array; they are not represented as popular-vote percentages.
- At the 2000 start, the party-support distribution is rebalanced among the PRDS, UDP, Action for Change, APP, UFP, RDU, RFD, UNDD and military influence. Action for Change's January 2002 ban is modelled separately from its 2001 election result; the event preserves the party's already elected parliamentary members in the narrative.
- The 2003 coup attempt is represented as a choice, with the historical AI prioritising the failed coup outcome.
- The 2005 and 2008 coups are separate transitions, with civilian handover and negotiated alternatives.
- The 2007 anti-slavery law and the later specialised anti-slavery courts are distinct events. The courts were inaugurated in 2016.
- The Greater Tortue Ahmeyim event is placed in 2025, after first gas production and the start of LNG exports.

## Compatibility and validation

The submod does not replace Mauritania's map, states, order of battle, division templates or existing military characters. It adds country-specific files and makes small, deliberate additions to the shared party-display hooks.

The GitHub branch includes structural checks and an automated package workflow. Repository validation can catch script, localisation, icon and reference errors. A full Hearts of Iron IV launch and campaign playtest still has to be completed in-game before calling the release fully playtested.

## Source and design approach

Historical party names and the 2001 seat count are based on the International Parliamentary Union and the historical CIA World Factbook party list. The focus design follows Millennium Dawn's own emphasis on connected branches, historically credible AI, meaningful alternatives and country-specific mechanics.
