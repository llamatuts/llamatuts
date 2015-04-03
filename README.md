# [Llama tuts](http://llamatuts.github.io/)

Coding tutorials for absolute beginners. Even llamas need to learn how 
to code. This project is a collaboration between [Wendy Beth](https://twitter.com/wendybeth010), 
[Jimmy Lo](https://twitter.com/jimmylocoding) and [Jonathan Yeong](https://twitter.com/JonoYeong). 

> Estimated time to completion: 3 months (July 2015)

# Get started

Llama tuts uses [Jekyll](http://jekyllrb.com/) to generate the static site. Before you begin ensure
you have the jekyll gem installed on your machine. If not, run:

`gem install jekyll`

Then: 

1. Clone this repo.
2. `cd` into llamatuts folder.
3. Run `jekyll serve` and open `localhost:4000` to see the site.

# Deploy Llamatuts to Github Pages 
The steps below are in reference to the root directory of the project.

1. Clone https://github.com/llamatuts/llamatuts.github.io.
2. Rename the folder to _site.
  - `jekyll build` will generate static files and place them in _site directory.
3. To push to production make sure you are on branch `master` of `llamatuts` repo:
  - Then `cd _site` then `git commit -m "Your message" && git push"`

# Contributing
For things to do check out the issue list.

> If you're happy and you know it, clap your hand.
> If you think of something to write and you don't have time to write it yourself, make an issue!
> If you want design a new element or think something looks terrible, make an issue!
> If you want to help out in fixing these things, take an issue!

If we communicate the probability of disastrous merge conflicts is quite small. Especially
since this is only a 3 person project. Thus, the guidelines for merging and branching is quite
lax. There are some general best practices, described below.

#### Master branch
This branch is what the world will see. It is the code that will be pushed to our [Github Pages](https://github.com/llamatuts/llamatuts.github.io)
repo. The only branch that should merge into `master` is `develop`.

This is to safeguard against any merges that may break the llamatuts website.

#### Develop branch
This branch is what we'll merge most of our branches into. Once we are confident that our changes
haven't broken anything on the website we can merge `develop` into `master`. All of our feature branches
or branches dealing with issues should be branched from `develop` and not from `master`. This is because
`develop` will be ahead of `master` most of the time.

#### Feature/Issue branches
Create these branches off `develop` as you need. Or if you don't think it needs a branch you can work directly
on `develop`. Just be sure to communicate any merge conflicts you encounter.
