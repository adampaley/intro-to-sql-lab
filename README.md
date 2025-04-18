# Intro to SQL Lab
## Setup
Open your Terminal application and navigate to your `~/code/ga/labs` directory:

```
cd ~/code/ga/labs
```
Clone the [Intro to SQL Lab Starter Code](https://git.generalassemb.ly/modular-curriculum-all-courses/intro-to-sql-lab-starter-code) repository, and enter the new directory:

```
git clone https://git.generalassemb.ly/modular-curriculum-all-courses/intro-to-sql-lab-starter-code.git
cd intro-to-sql-lab-starter-code
```
Once cloned, you’ll need to remove the existing `.git` information.

This can be done with the following command:

```
rm -rf .git
```
    Removing the `.git` info is important as this is just a starter code provided by GA. You do not need the existing git history for this project.

With the old `.git` information removed, you can now reinitialize Git to start your own version control history.

Use these commands to initialize a new Git repository and make your first commit:

```
git init
git add .
git commit -m "initial commit"
```
Next, open the contents of your new project directory in VSCode:

`
code .
`
Create a new database called `world` and populate it with the SQL found in `world.sql`:

```
psql -f world.sql
```
Start `psql` and connect to the new database called `world`:

```
psql -d world
```
Use the `\d` command to see what tables are available. You should see:

| Schema | Name  | Type | Owner |
| ------ | ---- | ---- | ----- |
| public | cities |	table | your-username |
| public | countries | table | your-username |
| public | countrylanguages | table | your-username |

Now that you are connected to `psql` and see your tables, you’re ready to start.

## Exercises
### Instructions
Solve each clue in the `clues.sql` file in your starter code repo.

Run the SQL file in the terminal as you solve each clue:

```
psql -f clues.sql
```