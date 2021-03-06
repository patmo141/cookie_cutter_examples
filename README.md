# cookie_cutter_examples

This project is a collection of minimal examples of how to build rich interactive addon user interfaces using the CGCookie addon_common library.

# Tutorials

This project will follow along with some youtube videos


# How to Set Up

I have setup addon_common as a "subtree" of this repository, the main purpose of which is to allow github projects which leverage this to pull down the addon_common directory in the .zip.  Subtrees allow for relatively easy tracking and pushing of code to subtree repositories.   For projects that use addon_common as a subtree you can set it up like this

```
git remote add addon_common https://github.com/CGCookie/addon_common.git
git subtree add --prefix=subtrees/addon_common addon_common b280
```

this sets up the addon_common repository in a directory called "subtrees"  in your project.

# How to Keep Up to Date
to pull updates from addon_common

```
git subtree pull —prefix=subtrees/addon_common addon_common b280
```

If your project is using addon_common master branch, replace "b280" with "master"

# Contributing to addon_common
If you might contribute to addon_common, you should ford addon_common into your own repo and set up your subtree to track your fork.  You can then edit your forked addon_common directly in your project.  You can push your changes to your forked addon_common and later submit a pull request.

```
git subtree push —prefix=subtrees/addon_common addon_common b280
```


