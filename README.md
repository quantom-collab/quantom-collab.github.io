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
   `http://127.0.0.1:4000/`

Next time you want to view the website locally, you only need to do steps 2, 3, 5,
and 6.


## Notes

These are notes about navigation of this site and where is what.

* The menu in the header can be updated in file `_data/navigation.yml`

* The pages associated to each link in the header are located in the folder
  `_pages`.

* `assets/img/favicon.png`: the small icon displayed in the browser tab

* `assets/img/band_qcd_1.jpg`: the banner image on the landing page

* `assets/img/band_page_1.jpg`: the banner image on the other pages

* `assets/img/logo_quantom_collab.png`: the logo of QuantOm; currently unused

* Each news item is associated to a news article in the folder of `_news`.
