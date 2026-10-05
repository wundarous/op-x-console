# Reader website

The `website/` directory is the compiled reader and its supplied public Week 1
content. Existing console downloads remain at the repository root.

The live domain is configured in repository Settings → Pages → Custom domain.
This build serves from the domain root (`/`).

## Enable GitHub Pages once

Open this repository's **Settings → Pages**. Under **Build and deployment**,
choose **GitHub Actions** as the source. GitHub Actions must be enabled for this
repository. No personal token, AWS credentials, or additional repository is needed.

## Publish

Push changes to `website/` or `.github/workflows/pages.yml` to `main` to publish
automatically. Only `website/` is uploaded. Console-only updates do not redeploy.
For a manual deployment, open **Actions → Publish reader → Run workflow** and
select `main`.
Use the deployment link from the successful workflow to open the live site.

## Update the website

In the independent reader source project:

```sh
npm ci
npm test
npm run build -- --base=/
```

Replace this repository's `website/` directory with the resulting `dist/`
contents, removing obsolete build files. Review, commit, and push that change,
and the push to `main` publishes automatically. Do not hand-edit compiled files.
The reader's explicit content importer supplies story updates before building;
this repository never reads private authoring files or editorial review state.

Console sync updates its own generated files and preserves the website and
workflow. Commit or preserve pending website edits before running console sync.
To roll back a website release, revert its website changes on `main` and push
the revert; it will publish automatically.
