## Buildit Gems

This repo contains a file `build` that is a script for building gems using the [buildit-buildpack](https://github.com/schneems/buildit-buildpack).

## Run

Clone the repo.

```
$ git clone https://github.com/schneems/buildit-vim.git
$ cd buildit-vim
```

Create a heroku app

```
$ heroku create
```

Set your buildpack

```
$ heroku buildpacks:add https://github.com/schneems/buildit-buildpack
```


```
$ git push heroku master
```


Protip: If you need to re-deploy without changing your script you can force a commit by running `$ git commit --allow-empty -mempty`.

Now visit your site to download the results in a `builds.tar`

```
$ heroku open
```


