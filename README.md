# repo-contrib-graph

## Summary

As a developer, when I look around on GitHub, I can quickly see how active another user is by looking at their contribution graph.

![some sweet, tender loving](https://user-images.githubusercontent.com/519171/67789032-b18ee780-fa49-11e9-9d0b-4a9cf66a30f9.png)

However, it sometimes may just as important, if not *more* important to see how active a repository is. I want a quick, at-a-glance view of how often a repository is being contributed to. If I'm going to use a project as a dependency, I want to know that there's life in the community.

Enter repo-contrib-graph.

What does it do, you might ask?

Blammo:

![Theydies and Gentlethem, your repository contribution graph](https://user-images.githubusercontent.com/519171/67788391-9a9bc580-fa48-11e9-9370-c0696cb3b123.png)

It generates an ASCII contribution graph for an entire repository. Now you can see how active a repo is with just a few simple keystrokes!

## Installation & Usage

First, you might want to make sure you have [curl](http://curl.haxx.se/download.html) and [jq](http://stedolan.github.io/jq/download/) installed.

Then clone this repository!

```shell
git clone https://github.com/KyleMacey/repo-contrib-graph.git; cd repo-contrib-graph
```

Then simply pass in a repository.

```shell
./repo-contrib-graph rails/rails
```

Rather copy an entire URL?

```shell
./repo-contrib-graph https://github.com/rails/rails
```

Have a GitHub access token to alleviate the stress of API rate limits? Then `-t` is for you.

```shell
./repo-contrib-graph -t 123456789123456789 rails/rails
```

Your shell doesn't support color? `-p` that noise.

```shell
./repo-contrib-graph -p rails/rails
```

For more help, simply give it a `-h`

```shell
./repo-contrib-graph -h
```

## Credit

Inspired by [IonicaBizau/git-stats](https://github.com/IonicaBizau/git-stats)

## Coming (relatively) Soon

 - [x] **Colors!** A colorful representation of commit history for your viewing pleasure (#4)
 - [x] **Distributed Ranges!** To make the graphs more relevant (#5)
 - [x] **More stats!** Because who doesn't like data? (#6)
 - [ ] **???**
