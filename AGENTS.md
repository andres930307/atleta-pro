<!-- LOVABLE:BEGIN -->
> [!IMPORTANT]
> This project is connected to [Lovable](https://lovable.dev). Avoid rewriting
> published git history — force pushing, or rebasing/amending/squashing commits
> that are already pushed — as it rewrites history on Lovable's side and the
> user will likely lose their project history.
>
> Commits you push to the connected branch sync back to Lovable and show up in
> the editor, so keep the branch in a working state.
<!-- LOVABLE:END -->

## Architecture decisions
- Personal pages live under the client-gated authenticated route; account and onboarding stay public for session hydration.
- Athlete plans and logs are stored in the existing per-user Cloud row; private photos use the existing athlete-photos bucket.
- AI planning, coaching and peak-week generation use protected server functions so prompts and credentials stay private.
