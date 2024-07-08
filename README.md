Process
===

To open an RFC, a Pull Request must be opened which creates a new Markdown file in `rfcs/` folder. The RFCs should follow the template `TEMPLATE.md`, and should have a file name that is a short human readable description of the feature (using lowercase alphanumeric characters and dashes only). Try using the general area of the RFC as a prefix, e.g. `encrypted-dms.md` or `profile-cosmetics.md`.

Every open RFC will be open for at least two calendar weeks. This is to make sure that there is sufficient time to review the proposal and raise concerns or suggest improvements. The discussion points should be reflected on the PR comments; when discussion happens outside of the comment stream, the points salient to the RFC should be summarized as a followup.

When the initial comment period expires, the RFC can be merged if there's consensus that the change is important and that the details of the features presented are workable. The decision to merge the RFC is made by the Campground team.

When revisions on the RFC text that affect features are suggested, they need to be incorporated before a RFC is merged; a merged RFC represents a maximally accurate version of the feature that is going to be implemented.

Each RFC will be assigned a shepherd.  This person will support you in getting feedback, request necessary changes, and ultimately either accept (and merge) the RFC or turn it away.

In general, RFCs can also be updated after merging to make the language of the RFC more clear, but should not change their meaning. When a new feature is built on top of an existing feature that has an RFC, a new RFC should be created instead of editing an existing RFC.

When there's no consensus that the feature is broadly beneficial and can be implemented, an RFC will be closed. The decision to close the RFC is made by the Campground team.

Note that in some cases an RFC may be closed because we don't have sufficient data or believe that at this point in time, the stars do not line up sufficiently for this change to be worthwhile, but this doesn't mean that it may never be considered again; an RFC PR may be reopened if new data is available since the original discussion, or if the PR has changed substantially to address the core problems raised in the prior round.

Implementation
===

When an RFC gets merged, the feature *can* be implemented; however, there's no set timeline for that implementation. In some cases implementation may land in a matter of days after an RFC is merged, in some it may take months.

To avoid having permanently stale RFCs, in rare cases Campground team can *remove* a previously merged RFC when the landscape is believed to change enough for a feature like this to warrant further discussion.

When an RFC is implemented and the implementation is enabled via feature flags, RFC should be updated to include "**Status**: Implemented" at the top level (before *Summary* section).