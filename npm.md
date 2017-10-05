# NPM Versioning standards

## Components

1. After making the component edits:
   ```
   bash
   git add .            # add all the modified files; adjust as appropriate!
   git commit           # follow git.md#format-of-the-commit-message standards
   npm run gulp -- bump # Sean: note the space between "-- bump"
   git push             # push to your forked repo
   ```
2. Record the component's package.json version number
3. Make the pull request
4. Update PD360-html  

---
  
**_EITHER_**  

In [pd360-html](https://github.com/sinet/pd360-html):
1. update the package.json dependency version to the component's version (from step 2 above)2. update npm-shrinkwrap.json (run `npm-shrinkwrap`)
3. find component name and change version number in the three different places (version, from, resolved)4. Commit the two files
5. Run `npm install` (may need to delete npm-shrinkwrap.json and node_modules/@sinet/{component} folder as well  
   
**_OR_**  

1. ensure your local "pd360-html" is fully up-to-date
   ```bash
   cd path/to/your/local/pd360-html/repo
   git pull
   npm install
   ```
2. in package.json, manually update the component's dependency version
3. update shrinkwrap, then prep and push the updates  
   ```bash
   npm-shrinkwrap
   git add .
   git commit -m "chore: bump _package_name_ to _version_number_"
   git push
   ```
---
