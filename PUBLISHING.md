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

Open **Actions → Publish reader → Run workflow**, select `main`, and run it.
Only `website/` is uploaded. Pushing commits alone never deploys the site.
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
then manually run **Publish reader**. Do not hand-edit compiled files.
The reader's explicit content importer supplies story updates before building;
this repository never reads private authoring files or editorial review state.

Console sync updates its own generated files and preserves the website and
workflow. Commit or preserve pending website edits before running console sync.
To roll back a website release, revert its website changes on `main` and manually
run the workflow again.
