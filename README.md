# Route Downcaser

This is our Marley Spoon port of the gem `route_downcaser` by Carsten Gehling. The original source code can be found
here: https://github.com/substancelab/route_downcaser.

The gem is working exactly as intended by Gehling with the only exception that we support `include_patterns` besides
the `exclude_patterns` in the original. Unfortunately, nobody has been interested into merging this into the main
branch.

### Releasing a new version

Releasing a new version will update the gem version automatically (no need to update manually in `version.rb`.)

You can use the shorthands to release a new `patch`, `minor` or `major` version:

`PACKAGECLOUD_TOKEN=my_packagecloud_token script/release patch|minor|major`

You can also release a specific version:

`PACKAGECLOUD_TOKEN=my_packagecloud_token script/release 1.0.0`

The version will be bumped accordingly, a new git tag will be created and pushed to the `origin` remote and, finally, the gem will be packed and uploaded to [PackageCloud](https://packagecloud.io).
