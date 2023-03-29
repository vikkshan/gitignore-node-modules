I like to set up a `.gitignore` file at the very start (when I set up my repos and first clone it). So, most of the time, I get away with git caching the file problem.

NOTE: if you are using VS Code editor, your VS Code may prompt that you have too many actions in your repository. Mine does, but it can be because I use VS Code extensions for the git.

If not, you can follow these instructions;

The following steps are command line commands, so you will need your command prompt, terminal, or similar command line application. Here are the steps.

1. Navigate to the git repository folder.

2. Create a `.gitnore` file if it does not exist by the following command:

```
touch .gitignore
```
3. Add `node_modules` in `.gitignore` by opening and adding `"node_modules"` in the `.gitignore file.` Or you can run the following command.

```
echo node_modules >> .gitignore
```
4. Remove cached `node_modules` from the repo by running this command:

```
git rm -r --cached node_modules
```
5. run `git add` and `git commit` commands for the git to make notes of the `node_modules` folder removal.

```
git add . 
```
>This will add the `.gitignore` file and `node_module` removal (and any other change you made to the repo). 

```
git commit -m "Remove node_modules folder from the repo."
```
