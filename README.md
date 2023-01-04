# [ScottKirvan.github.io](https://github.com/ScottKirvan/ScottKirvan.github.io)

https://ScottKirvan.com / https://skvfx.com

## Running the Server
The instructions below for starting the server locally don't work in my case.  I use the following in the repository root:
```sh
bundle exec jekyll serve
```

After a recent windows update, I got a ```Can't find gem bundler (>=0a) with executable bundle``` error.  Fixed with:
```sh
sudo gem install bundler -v "$(grep -A 1 "BUNDLED WITH" Gemfile.lock | tail -n 1)"
```

## Branches

- **published**
    - this is the branch on the website

To work on this code, create a new branch, make the changes and test there, then merge that branch into published, and if no longer needed, delete the branch.

---
## [TODO](notes/TODO.md) ![TODO](notes/TODO.md)
---
## [CHANGELOG](notes/CHANGELOG.md) ![CHANGELOG](notes/CHANGELOG.md)

---
Forked from:  
https://ndrewtl.github.io/airspace-jekyll/

# [_Airspace_ for Jekyll](notes/ORIGINAL_README.md) (Original README.md)
