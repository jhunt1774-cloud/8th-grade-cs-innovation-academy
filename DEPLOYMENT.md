# Publish the student curriculum

The `student-site` folder is the complete buildless static website. Only its contents belong in the GitHub Pages repository. The teacher-private folder, complete-course archive, private assessment archive, and authoring source contain answer keys and must remain private. A private folder name is not an access control if it is uploaded into a public repository.

1. Create or select the intended GitHub repository. This package has not created or modified a repository.
2. Copy **only** the contents of `student-site` into the repository root. Include `.nojekyll`, `index.html`, all `.js` files, and `style.css`. No build command or package installation is needed.
3. Configure GitHub Pages to deploy from the intended branch and root folder. GitHub also supports a `/docs` source folder if you place the student files there instead. Do not select a folder containing teacher files.
4. Wait for GitHub's deployment to finish and open the exact URL GitHub reports. Test a deep lesson link such as `#w1d2`, all lab types, text zoom, keyboard use, response download/restore, and clipboard on an actual school Chromebook.
5. Use the published URL plus the lesson fragments in the Classroom assignment files. The repository URL and Pages URL are not necessarily identical.

All resource links are relative, and navigation uses URL fragments, so project subpaths are supported. Lessons load from a local script rather than a fetched JSON file; the site can also be opened from an extracted folder. Some browser features, especially clipboard and the isolated coding runner, may be restricted under file URLs or school policy. HTTPS GitHub Pages is the intended classroom deployment. No offline service worker or guaranteed offline Classroom/Pear access is claimed.

The site is intentionally small and uses no external libraries, media downloads, WebGL, camera, microphone, or student account system. It includes a protected short-lived JavaScript worker for the coding lab. Its timeout and limited output help with runaway code, but actual old-Chromebook performance and school browser policy require a device check. No device-specific performance certification is claimed.

To extend: use the included private authoring source, update lesson data and related question/solution records, then rebuild and check. Never copy the private source into the public repository. The stable lesson IDs connect the site, teacher guide, Classroom packages, and assessments.

Reference: [GitHub Pages publishing configuration](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).
