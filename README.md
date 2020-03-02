# bitwiki
This is a concept for an on-chain wiki on BSV.

The wiki would be managed by javascript.
A community fund would provide for anonymous edits.

The wiki would be stored using git, as D:// packfiles.
`isomorphic-git` would be used to access it, as in js-gitview.
It would be rendered as an interconnected tree of markdown files, like most git wikis.

A fork might need to be made of isomorphic-git to provide for http alternative support, which lets multiple accounts
provide views of the wiki while sharing data resources.

## ---
okay ummm
ONGOING: please break code into multiple modules, don't code all in one file
		-> webpack can do this out of the box.  put javascript next to it, do 'export default obj' at the end,
		   and pair that with 'import obj from "./javascript.js"'
1. find git-wikis, and load one
	they are probably git-remote-bsv repos with a certain file in them, to find them
	could be helpful if it's a git-tag, possibly
	then it can be added via git.
2. show a nice interface
3. note: we will want to export to html, so the wiki can be stored elsewhere.  of course, other wiki engines could manage that.
