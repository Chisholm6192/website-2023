## Setup

Fork this repo and then clone it onto your local machine.

```
git clone <your fork name>
cd website-2020
```

Set the original repo (ie non fork) as the "remote"

```
git remote add upstream https://github.com/thegoldenhack/website-2020.git
git fetch upstream
git checkout master
```

Set the environment variables and fill in the fields in the .env file with the appropriate values (if applicable).

```
cp .env.example .env
```

Check out a new branch and get started :)

```
git checkout -b <your branch name>
npm install
```

## Rebasing

Each time you open the codebase with the intention of doing some work on it, I recommend that you do a rebase. Trust me, it's MUCH better than merging, and as long as we work on distinct parts of the codebase, we shouldn't run into many issues.

Save your progress
`git stash save`

Get any changes that may have been made on master, and keep your forked branch in sync with the main repo

```
git checkout master
git pull upstream master
git push origin master
```

Go back to the branch you were on
`git checkout <your branch name>`

Rebase master -> you may have some conflicts to deal with at this point, but just follow the instructions in the console and everything should be ok
`git rebase master`

## PR Process

So let's say you wrote some code and you are ready to get it peer reviewed.

The first time you do this you may be prompted for your GitHub username and password!

_First make sure you've rebased!!_

Add the files you want to commit either individually
ie `git add src/views/HomePage/index.js`
or add all the files that have been modified
ie `git add .`

Commit the files you changed
`git commit -am 'Helpful commit message'`

Push to the remote
`git push origin <your branch name>`

Then hit the link in the console to open a pull request.

Pull requests must be reviewed and approved by 1 other team mate, at which point I (Dunja) will review it as well. If everything looks good, I'll merge your code to master!

Pull in your changes, and open a new branch

```
git checkout master
git pull upstream master
git checkout -b <your new branch name/>
```

## `yarn start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.


## Dad Joke Central
Kyle's favourite dad joke: 
    What time did Sean Connery get to Wimbledon? 
    Tennish.

Bonus dad joke!:
    Last Christmas my family bought a fake Christmas tree and the clerk said to my dad "Are you going to put it up yourself?". My dad replied "Don't be disgusting, I'm going to put it in the living room."

Tailai's Dad Joke that is a pun:
    ["hip", "hip"]

Dhruv's favourite dad joke:
    What do you call someone with no body and no nose? Nobody knows

Vipneet's dad joke:
    Today, my son asked "Can I have a book mark?" and I burst into tears. 11 years old and he still doesn't know my name is Brian.

Tailai's New Dad Joke:
    What's the difference between a bird and a fly?
    A bird can fly but a fly can't bird.
    
Wen's dad joke:
    Where are average things manufactured? The satisfactory 

Alice's Favorite Dad Joke:
    What's Forrest Gump's password?
    1Forrest1

Kyle's New Favourite Dad Joke:
	I recently bought a new thesaurus. Not only is it terrible, it's terrible.

Dennis's dad joke:
    (Read it aloud) What do you call a fish with no eyes? Fsh.
    
Vipneet's New Dad Joke:
    Why are elevator jokes so classic and good? They work on many levels.

Brayden's Dad Joke:
    There's a very fine line between numerators and denominators, and only a fraction of people understand that.

## Challenge Question
<details>
  <summary>What programming language does the James Webb Space Telescope use?</summary>

  ```
  JavaScript 🤣
  https://news.ycombinator.com/item?id=19737663
  ```
</details>
