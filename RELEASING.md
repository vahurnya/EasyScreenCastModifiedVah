# Releasing

1.  Set the correct version in `package.json` and increase the extension
    version in `metadata.json`.
    
    Run `npm install`, commit `metadata.json`, `package.json` and `package-lock.json`.

2.  Rename current "next" milestone, create a new "next" one: <https://github.com/EasyScreenCast/EasyScreenCast/milestones>

3.  Update `CHANGELOG.md` with version and release date. Make sure all
    issues / PRs are listed.

4.  Create a tag and push: e.g. `git tag 1.4.0 && git push origin tag 1.4.0`

5.  Build locally `make zip-file`

6.  Create a new draft release on github: <https://github.com/EasyScreenCast/EasyScreenCast/releases/new>.
    Use the info from `CHANGELOG.md` to for the release notes. Upload the zipfile as a release artifact.

7.  Upload zip file on <https://extensions.gnome.org>.

8.  Once the extension is activated on <https://extensions.gnome.org/extension/690/easyscreencast/>
    publish the release on github: <https://github.com/EasyScreenCast/EasyScreenCast/releases>.

    If the extension is rejected, you can move the tag and start over.
