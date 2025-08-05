# fiz GitHub Pages Template
fiz can import other fiz files via URL as long as the file can be fetched via HTTP GET. Publicly hosting fiz files enables people to import and build on each other's work. To facilitate serving fiz files, this guide shows how to publish static files to a project site on [GitHub Pages](https://pages.github.com).

## Instructions
1. Change the LICENSE. This template is released under the [`CC0-1.0` License](https://creativecommons.org/publicdomain/zero/1.0/). Unless you also intend to dedicate this repository to the public domain, update to [your intended license](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository). 
1. Configure GitHub Pages.
    1. In GitHub, open your repository's `Settings` > `Code and automation` > `Pages`.
    1. Under `Build and deployment`, set `Source` to `Deploy from a branch` and set `Branch` to `main` with folder `/docs`.
1. Replace the example assets in `/docs` with your assets. Create subdirectories as necessary.
1. Verify your fiz locally. You can serve the files locally using [`serve`](https://github.com/vercel/serve) or another similar tool. In your browser, check if the files import correctly. You will need to find and replace mentions of `https://<username>.github.io/<repo>/` with the local address (e.g. `http://localhost:3000/` by default for `serve`). Remember to revert these URLs back to the public GitHub Pages address before you publish.
1. Merge changes into main. This will publish to GitHub pages once merged.
1. Check that your fiz imports correctly from the public address.
1. Update this README to describe your repository.

### License Notes
- Image creators may want to consider licensing their images separately from their code or host them on a platform with more controls.
- External images linked within fiz files may have different licenses than the fiz repository itself. Users importing such files are responsible for ensuring they comply with the respective image copyrights.

### Stability Notes
- fiz doesn't have a centralized package manager (yet) so users are left to their own devices.
- There is currently no convention for how to organize fiz packages, but it may be helpful to create a showcase fiz to demonstrate what your package is about at a glance.
- For popular projects, it would be courteous to bake version numbers into your file names and never modify files once published. Only appending new files for new versions ensures you don't break importers.
- Keep in mind that repository owners can take down their repositories without notice. On the flip side, it is very easy for others to fork and host clones of repositories.
