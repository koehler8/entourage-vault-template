# Templates

Scaffolds for notes **you** create by hand. Copy one, fill in the frontmatter,
drop it in the matching folder.

**Daily notes are deliberately not here.** The `morning` / `after-work` /
`before-bed` scaffolds live in the vault's configuration (control-plane side),
not in this folder, because that is what `vault_daily` renders from when it
creates today's note. A second copy here would look authoritative and drift
from the one actually in use — sections would stop matching, and the agents
that append to a named section would silently write nowhere.

To create today's note by hand, just ask an agent, or call `vault_daily`.
