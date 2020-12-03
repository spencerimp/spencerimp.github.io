Personal blog using template modified from

[https://github.com/mmistakes/minimal-mistakes](https://github.com/mmistakes/minimal-mistakes)

# Install development dependencies

```
sudo gem install jekyll bundler
bundle install
```

# Create a new post

```
rake post title="my post title"
# edit the yyyy-mm-dd-xxxx.md
# the url will be /root-url/yyyy/mm/dd/xxxx
```

# Create a pub page

```
rake page title="about"
# edit the xxxx.md
# the url will be /root-url/xxxx
```

# Local preview

```
rake preview
```

# Edit the navigation items (upper-right header)

```
#edit ./_data/navigation.yml
```
