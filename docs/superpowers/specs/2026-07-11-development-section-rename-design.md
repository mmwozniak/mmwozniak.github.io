# Development Section Rename

## Goal

Rename the site's former Experiments section to Development without changing the
content of its existing entries.

## Scope

- Use `Development` as the visible navigation and page name.
- Publish the section at `/development/`.
- Use Jekyll's `development` collection and `_development` source directory.
- Preserve the current SRE and SPE entry content and their generated collection
  URLs under `/development/`.
- Do not alter ordinary prose that refers to scientific experiments.

## Implementation

The existing Jekyll configuration already declares a `development` collection
and the landing page metadata already targets that collection. Complete the
rename by moving the source directory and landing page to development-named
paths, then update the primary navigation link. No redirect is included because
the requested option is a full section rename and the current configuration has
no redirect plugin.

## Verification

Build the Jekyll site and confirm the generated navigation links to
`/development/`, that the Development collection page renders, and that the SRE
and SPE entries are generated beneath `/development/`.
