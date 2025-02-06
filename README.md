# quantum-collab.github.io

Website data for
[https://quantum-collab.github.io](https://quantum-collab.github.io).

## Local Rendering/Development

To render and view the website locally, you need to have Ruby and Jekyll
installed. The following steps show an example of creating a new Anaconda
environment specifically viewing the website locally:

1. Create a new Anaconda environment. Let's name it `ruby-jekyll` here. (
   `mamba` is a variant of `conda`. You can also use `conda` with the
   `conda-forge` channel to replace `mamba` here.)
   For Linux, do
   ```bash
   $ mamba create -n ruby-jekyll python=3 ruby gxx_linux-64
   ```
   For MacOS, replace `gxx_linux-64` with `clangxx_osx-64`.

2. Activate the Conda environment
   ```bash
   $ mamba activate ruby-jekyll
   ```

3. Get into the folder of this repository:
   ```bash
   $ cd quantom-collab.github.io
   ```

   And, optionally, switch to a specific branch if it's not the current one:
   ```bash
   $ git checkout <branch>
   ```

4. Install the Ruby dependencies required for this website
   ```bash
   $ bundle install
   ```

5. Render the website and start the web server
   ```bash
   $ bundle exec jekyll serve --livereload
   ```

6. Open the local website in a browser at
   `http://127.0.0.1:4000/quantom-collab.github.io/`

Next time you want to view the website locally, you only need to do steps 2, 3, 5,
and 6.


## Notes

These are notes about navigation of this site and where is what.

* The menu can be update in file `_data/navigation.yml`

* The pages being pointed to by the navigation are located in the folder
  `pages`. Each one corresponds to a file with `.md` extension.

* `assets/img/favicon.png`: the small icon displayed in the browser tab

* At the moment I have chosen to use the layout `page` but there are several
  other layouts that in the folder `_layout` that can be explored.

* In file `_config.yml`, you can see that posts form the feed. I have not yet
  experimented with it. This is also the file where logos are inserted. And the
  social media hooks etc. They are near the top of the file. You can also see
  that the cover image is defined in line
  `cover_image: "assets/img/bg/page-title.jpg"`.
  I have just inserted an image of sunset in there as place holder, one can
  either put in another image with the same path and filename, or change the
  line in `_config.yml` and use some other filename.

* In general images are movies live in assets folder.

* Slider images that show up on homepage and landing page are located in 
  `assets/img/slider`, and file where name of the files in that folder appear is
  `_includes/slider.html`.





