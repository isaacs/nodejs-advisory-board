# Contribution Policy

Individuals making significant and valuable contributions are given
commit-access to the project. These individuals are identified by the
Technical Committee (TC) and discussed during the weekly TC meeting.

If you make a significant contribution and are not considered for
commit-access log an issue and it will be brought up in the next TC
meeting.

Internal pull-requests to solicit feedback are required for any other
non-trivial contribution but left to the discretion of the
contributor.

Pull requests may be approved by any committer with sufficient
expertise to take full responsibility for the change, according to the
"Landing Patches" protocol described below.

## Landing Patches

- All bugfixes require a test case which demonstrates the defect.  The
  test should *fail* before the change, and *pass* after the change.
- Trivial changes (ie, those which fix bugs or improve performance
  without affecting API or causing other wide-reaching impact) may be
  landed immediately after review by a committer who did not write the
  code, provided that no other committers object to the change.
- If you are unsure, or if you are the author, have someone else
  review the change.
- For significant changes wait a full 48 hours (72 hours if it spans a
  weekend) before merging so that active contributors who are
  distributed throughout the world have a chance to weigh in.
- Controversial changes and **very** significant changes should not be
  merged until they have been discussed by the TC which will make any
  final decisions.
- Always include the `Reviewed-by: Your Name <your-email>` in the
  commit message.
- In commit messages also include `Fixes:` that either includes the
  **full url** (e.g.  `https://github.com/joyent/node/issues/...`),
  and/or the hash and commit message if the commit fixes a bug in a
  previous commit.
- PR's should include their full `PR-URL:` so it's easy to trace a
  commit back to the conversation that lead up to that change.
- Double check PR's to make sure the persons **full name** and email
  address are correct before merging.
- Except when updating dependencies, all commits should be self
  contained.  Meaning, every commit should pass all tests. This makes
  it much easier when bisecting to find a breaking change.
