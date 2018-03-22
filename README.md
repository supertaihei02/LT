# LT




## Hugo Init

### 1. initialize
* For Mac `brew install hugo` and check install `hugo -v`


### 2. create topic

#### 1. Create
```
$ hugo new site [topic title(exp:yyyymm-times)]
Congratulations! Your new Hugo site is created in path/to/project/topic title.

Just a few more steps and you're ready to go:

1. Download a theme into the same-named folder.
   Choose a theme from https://themes.gohugo.io/, or
   create your own with the "hugo new theme <THEMENAME>" command.
2. Perhaps you want to add some content. You can add single files
   with "hugo new <SECTIONNAME>/<FILENAME>.<FORMAT>".
3. Start the built-in live server via "hugo server".

Visit https://gohugo.io/ for quickstart guide and full documentation.
```


Move to topic directory `cd [topic title direcotry]`

#### 2. Set theme
First, elect theme with website [https://themes.gohugo.io](https://themes.gohugo.io)
Clone theme repos to themes dir and remove .git.  
Write theme setting to project config.

```
$ git clone [git repo] themes/[theme name]
$ rm -r themes/[theme name]/.git
$ echo 'theme = "ananke"' >> [topic title]/config.toml
```

#### 3. Start local server
```
$ hugo new posts/post-sample.md
$ hugo server
```
Check your site [http://localhost:1313](http://localhost:1313/#1)


Some options `hugo help`
```
# contain draft
$ hugo server -D
# change theme
$ hugo server -t [theme name]
```






