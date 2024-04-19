# Earthstar Document Patterns

Every Earthstar document has a corresponding _path_. These are very much like
filesystem paths (e.g. `projects/ep/demo_final_final.mp3`) and offer the same
kind of flexibility. This makes it easier for users to store documents in ways
which make sense for them.

But unlike a normal filesystem, an Earthstar share has the concept of multiple
users baked in. `@suzy` may have a document at `my-stuff / todo`, and `@jose`
may _also_ have their own document at `my-stuff / todo` at the same time,
despite being at the same path.

When multiple users agree to store a particular kind of data (e.g. image data)
at a particular kind of path (e.g. `about/avatar`), they have co-authored a
_document pattern_. Document patterns make it easier for users to collaborate
with each other and build interoperable applications which store and retrieve
data according to these patterns.

Document patterns are not standards or specifications. They can be adapted,
adopted, and reshaped according to local pragma. Applications intended for a
wide audience should be able to gracefully fail when documents do not follow the
pattern, while home-cooked programs for small groups can expect local custom to
be followed.

This is a list of document patterns submitted by the community.

# Document patterns

- [`about`](earthstar-community/about.md) - Public profile information such as
  display names, avatars, and bios.

# Submitting your pattern

Make a PR with a link to your document pattern.
