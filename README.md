# repo-contrib-graph

## Summary

As a developer, when I look around on GitHub, I can quickly see how active another user is by looking at their contribution graph. 

![dhh is keeping it real](https://cloud.githubusercontent.com/assets/519171/7695690/5952f4be-fdc1-11e4-9c0f-3119f3b14675.png)

However, it sometimes may just as important, if not *more* important to see how active a repository is. I want a quick, at-a-glance view of how often a repository is being contributed to. If I'm going to use a project as a dependency, I want to know that there's life in the community.

Enter repo-contrib-graph.

What does it do, you might ask?

Blammo:

![Ladies and Gentlemen, your repository contribution graph](https://cloud.githubusercontent.com/assets/519171/7695724/e3ef72dc-fdc1-11e4-8251-4ace5642318e.png)

It generates an ASCII contribution graph for an entire repository. Now you can see how active a repo is with just a few simple keystrokes!

## Installation & Usage

First, you might want to make sure you have [curl](http://curl.haxx.se/download.html) and [jq](http://stedolan.github.io/jq/download/) installed.

Then clone this repository!

```shell
git clone https://github.com/KyleMacey/repo-contrib-graph.git; cd repo-contrib-graph`
```

Then simply pass in a repository with the `-r` flag.

```shell
./repo-contrib-graph -r rails/rails`
```

Rather copy an entire URL? 

```shell
./repo-contrib-graph -r https://github.com/rails/rails`
```

Have a GitHub access token to alleviate the stress of API rate limits? Then `-t` is for you.

```shell
./repo-contrib-graph -r rails/rails -t 123456789123456789`
```

For more help, simply give it a `-h`

```shell
./repo-contrib-graph -h`
```

## Credit

Inspired by [IonicaBizau/git-stats](https://github.com/IonicaBizau/git-stats)

## Coming Soon

 - [ ] **Colors!** A colorful representation of commit history for your viewing pleasure (#4)
 - [ ] **Distributed Ranges!** To make the graphs more relevant (#5)
 - [ ] **More stats!** Because who doesn't like data? (#6)
 - [ ] **???**
