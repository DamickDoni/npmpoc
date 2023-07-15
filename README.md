# ts func lib

## How to publish to npm

### Step 1

Rewrite the following items in package.json in each folder as appropriate.

* name
* description
* keywords
* repository
* author
* bugs
* homepage

### Step 2

Rewrite the [repo option](./.changeset/config.json) in Changeset.  

```
"changelog": [
  "@changesets/changelog-github",
  { "repo": "your_name/repository_name" }
],
```

Also, do not forget to rewrite the title of CHANGELOG.md.

### Step3

Implement a great library under the [packages](./packages) folder.  

build and test
```bash
$ yarn build
$ yarn test
```

### Step7
Create new version/changelos
```bash
$ yarn changeset
```
Apply Version
```bash
$ yarn version-apply
```
