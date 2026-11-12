# Organization profile artwork

The header embeds the approved B2 Balanced Cube geometry unchanged from
`../branding/logos/logo.svg`. Teal #28C7BE and graphite #101C1B anchor the
dark palette. Light artwork uses darker teal #11766F for readable text.
All SVGs are self-contained: no scripts, external fonts, embedded HTML or remote assets.

## GitHub rendering

`profile/README.md` uses GitHub-supported picture/source/img markup.
Dark and light artwork is selected with prefers-color-scheme; light is the fallback.
The header scales down from 840 pixels. Each 280-pixel service card is an
independent inline image, so cards wrap as the available width decreases.
GitHub constrains images to their container width. There are no fixed-width tables
or custom CSS dependencies. Service copy is repeated in image alternative text.

Absolute raw URLs work on the organization overview as well as the repository.
They pin the asset commit (feb7902d308eeee98e56a837635e38706ee9bfbd) so artwork also resolves during PR review
and remains stable after merging. To update artwork, commit the new SVGs first,
then update the pinned SHA in the profile README.

## Review

Check the PR's rendered profile README in GitHub light/dark appearance and at
mobile width. GitHub may apply its own image spacing and caching. Browser theme
selection follows prefers-color-scheme as supported by GitHub.
