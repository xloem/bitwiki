# bitwiki
This is a concept for an on-chain wiki on BSV.

The wiki would be managed by javascript.
A community fund would provide for anonymous edits.

The wiki would be stored using git, as D:// packfiles.
`isomorphic-git` would be used to access it, as in js-gitview.
It would be rendered as an interconnected tree of markdown files, like most git wikis.

A fork might need to be made of isomorphic-git to provide for http alternative support, which lets multiple accounts
provide views of the wiki while sharing data resources.
