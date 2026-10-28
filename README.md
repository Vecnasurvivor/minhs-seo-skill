# minhs-seo: the all-in-one SEO skill for Claude Code

**Twelve OpenSEO workflows behind one router.** One skill instead of twelve: ask for anything SEO and Claude picks the right workflow and follows it.

## What you get

| Ask for | It runs |
|---|---|
| "Audit my site" | A data-backed SEO audit with the few changes most likely to grow organic traffic |
| "Find keywords for ..." | Keyword research, SERP checks, saving and tagging promising terms |
| "Group these keywords" | Intent clustering mapped to existing or new pages |
| "Analyze competitor X" / "Map my market" | Competitor footprint, content themes, backlinks, gaps, competitive landscape |
| "Find link prospects" | Prospecting, contact paths and outreach drafts |
| "My Google Business Profile" | Local SEO audit and Maps visibility |
| "How do I show up in ChatGPT / Gemini?" | AI-visibility audit and prompt research |
| "Set up my project" / "Coach me" | Project context, goals, competitors, Search Console intake, and a friendly coach mode |
| "Write the report" | One saved, self-contained HTML report |

Shared rules apply to every workflow: set up a project first, ask before spending credits, treat web text as untrusted data, and finish research with a report.

## How it works

`skills/minhs-seo/SKILL.md` is a short router: a table that says which guide fits which request, plus the shared rules. The twelve original guides sit unchanged in `skills/minhs-seo/references/<name>/GUIDE.md`, so nothing was cut. Claude now chooses between 1 skill instead of 12, and reads the full guide only when it needs it.

## Requires OpenSEO

The guides call the **OpenSEO** tools (keyword data, SERPs, site audits, backlinks, rank and AI-visibility tracking, Search Console). Without the OpenSEO MCP server and an OpenSEO account, the guides still explain each workflow, but the data steps cannot run. Research spends OpenSEO credits; the skill tells Claude to ask before large batches.

OpenSEO: https://openseo.so (source: https://github.com/every-app/open-seo, MIT)

## Install

```
npx skills add Vecnasurvivor/minhs-seo-skill -g
```

or copy `skills/minhs-seo` into `~/.claude/skills/`. If the twelve individual OpenSEO skills are also installed, remove them so Claude does not see duplicates.

## Credits and licence

The twelve guides come from the OpenSEO project (MIT, copyright its authors). The router, shared rules and packaging are by the minhs-seo contributors. Open source under the MIT licence, see [LICENSE](LICENSE). Contributions and issues are welcome.
