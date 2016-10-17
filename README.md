# Pelagos content

This repository only contains a github pages branch, nothing on master. The
branch has the information and header files for of our in-house cartodb layers
that we provide for pelagos. These files contain metadata about the layers,
such as title, description and configuration information for how the layers are
handled on the client, and they are loaded by the client directly from github
pages. The cartodb layers point at these files from their description fields.

This whole thing is actually a hack. Cartodb doesn't allow per-layer
information in any fields, and the description field (which was the ideal
candidate) has a hard limit of 200 characters, so it doesn't allow us to store
enough information in there. Having these files in github allows us to version
control them as well.
