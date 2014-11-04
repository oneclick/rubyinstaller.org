# rubyinstaller.org

## Important

This codebase host what we would like to call *upcoming* website for
RubyInstaller project, but is not live at this time.

If you want to report issues with current site, please use RubyInstaller's
[issue tracker](https://github.com/oneclick/rubyinstaller/issues) instead.

---

This repository holds the codebase, content and structure of
[rubyinstaller.org](http://rubyinstaller.org) website, built with
[Hugo](http://hugo.spf13.com) and (**TODO**)

## Get It!

For regular development, you only need [Ruby](http://rubyinstaller.org) to be
installed. This project will automatically fetch Hugo's dependency.

If you plan to introduce modifications to the theme used by the website, you
will require installation of A, B and C (**TODO**).

Then, clone this repository:

```console
git clone https://github.com/oneclick/rubyinstaller.org.git
cd rubyinstaller.org
```

You can now build your local copy and run the preview server:

```console
rake preview
```

Which will watch for changes and allow you see them locally at
[http://localhost:1313](http://localhost:1313/)

## Preview on Heroku

In case you cannot preview your changes locally or want other's to preview it
too, you can deploy your branch to Heroku.

- Signup to [Heroku](https://www.heroku.com/) if you don't have an account yet.
- Install [Heroku Toolbelt](https://toolbelt.heroku.com/)
- Clone this repository (see instructions above)
- Create a feature branch
- Make changes or add content
- Create preview application on Heroku using custom buildpack (**TODO**)

```console
heroku login
heroku create --buildpack https://github.com/oneclick/heroku-buildpack-hugo-something.git
```

- Push your code

```console
git push heroku feature_branch:master
heroku open
```
## TODOs

- [ ] Data structure
  - [x] Releases
  - [ ] DevKits
  - [x] News
- [ ] Theme and instructions
- [ ] Custom Buildpack for Heroku
- [ ] Contributing guidelines
  - [ ] Basic content structure
  - [ ] *How to* create releases
  - [ ] *How to* create news articles

## License

All the code contained in this repository, unless explicitly stated, is
licensed under MIT license.

A copy of the license can be found inside the [LICENSE](LICENSE) file.
