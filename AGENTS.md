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

- The admin UI is the original site's compiled bundle, served unchanged: `/` returns src/original-shell.html and the code lives in public/assets. Why: the user required a pixel-identical UI and no source code was available. The UI calls POST /api/cloud ({action,...}) and POST /api/upload; when those are missing it falls back to its built-in browser-only demo data.
