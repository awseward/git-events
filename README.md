# git-events

TODO: Consolidate what's currently spread out across these three locations:

```
  - https://github.com/awseward/dotfiles/tree/main/git-hooks

      Contains a set of hooks which all more or less delegate to `track` which
      writes TSV "events" to a central location that gets collected on a
      regular interval.

  - https://github.com/awseward/dw

      The following tables are concerned:

      - `public.dim_hook`
      - `public.dim_ref`
      - `public.dim_repo`
      - `public.events`
      - `public.fact_git_event`
      - `public.v_top_hooks`
      - `public.v_top_refs`
      - `public.v_top_repos`
      - `v2.v_repo`
      - `v2.v_top_repos`

      Some rework of the schemas would probably be good, too; I think it's
      grown a little funky over time.

  - https://github.com/awseward/git-events-collector

      Mostly just a small command line utility that packages TSV files up into
      SQLite files
```
