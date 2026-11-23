# pick-our-door

A neighborhood poll to choose our front door color. Neighbors scan the QR code on the yard sign, try each color on an illustration of the house, and vote.

- `index.html`: the whole site (static, no build step)
- Votes are stored in the `front-door-vote` Supabase project through two public functions: `cast_door_vote` and `door_vote_results`. The tables are locked down by RLS.
- To change the deadline or announce a winner, edit the single row in `door_poll_settings`. No redeploy is needed.
