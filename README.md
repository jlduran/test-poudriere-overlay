# Test poudriere overlay

Inspired by https://dan.langille.org/2019/08/10/poudriere-hooks/ and https://gist.github.com/dlangille/924507ce545de8fbbe78b50b752997ce.

This repo is an example poudriere-ports overlay repo.

It will be unionfs-mounted to an actual ports tree, overlaying the local changes.

For the purpose of this demonstration, I have opted to build a patched strongSwan package with its rc script customized.

Once poudriere-bulk is complete, the resulting packages are uploaded as artifacts.

The step-by-step is documented in the [.cirrus.yml](.cirrus.yml) file.
