# `about` document pattern

This is an document pattern for associating personal information (e.g. display
names, avatars, bios) with a particular identity (e.g. `@suzy.baaa...`).

All of the below are optional, and an identity may have any or all of the below
documents specified.

## Display name

Identity addresses begin with a shortname to make the address easier to
identify, (e.g. `suzy`). These shortnames cannot be changed and are always four
characters long, which makes them unsuitable for most names and the fluctuating
nature of identity.

Therefore it is desirable to have a free-form display name which can be changed
at any time.

### Document path

`about / displayName`

### Document payload

The desired display name as UTF-8 encoded bytes.

## Avatar

It's also fun to have an image to associate with a given identity.

### Document path

`about / avatar.{IMAGE_EXTENSION}`

where `IMAGE_EXTENSION` must be the common file extension of an image format
(e.g. `gif`, `jpg`, `png`) which allows clients to know how to interpret the
payload data for this document.

### Document payload

The payload should be image data of the format corresponding to the path's
`IMAGE_EXTENSION`. The image data should have a 1:1 aspect ratio. Try to make it
a good size, as applications may not display avatars that are too big.

## Biography

### Document path

`about / bio`

### Document payload

The desired biography as UTF-8 encoded bytes. Can be any length, but
applications may not display long bios.
