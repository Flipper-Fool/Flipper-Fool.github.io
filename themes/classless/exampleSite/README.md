# Demo for classless-blog

## How to run the demo yourself

Assuming you have

a) cloned the `classless-blog` theme _and_
b) `hugo` installed

you can easily run the demo follwing these steps:

1. Enter the exampleSite directory (where this Readme file is located):
   ```sh
   cd exampleSite
   ```
2. Run hugo (but tell it that the theme is in the parent directory of where you currently are )
   ```sh
   hugo server --themesDir="../.."
   ```

You can then visit the demo on http://localhost:1313/ (or similar, look at the output of the last command).

After that it is time to try out some stylesheet options in the `config.toml`.

## Sources

The images are all from Unsplash
and licensed under the [unsplash license](https://unsplash.com/license).

Here are the links to their sources and authors:

- [Drew_Beamer.jpg](https://unsplash.com/photos/vAij-E26haI)
  by [Drew Beamer](https://unsplash.com/@drew_beamer)
- [Gabriel_Izgi.jpg](https://unsplash.com/photos/cfQEO_1S0Rs)
  by [Gabriel Izgi](https://unsplash.com/@hirminhttps://unsplash.com/@gabrielizgi)
- [Max_Kleinen.jpg](https://unsplash.com/photos/L6sE85KbQrc)
  by [Max Kleinen](https://unsplash.com/@hirminhttps://unsplash.com/@hirmin)
- [Sandro_Katalina.jpg](https://unsplash.com/photos/k1bO_VTiZSs)
  by [Sandro Karalina](https://unsplash.com/@hirminhttps://unsplash.com/@sandrokatalina)
- [Tony_Reid.jpg](https://unsplash.com/photos/PGdMhonLLZk)
  by [Tony Reid](https://https://unsplash.com/@hirminunsplash.com/@togna_bologna)

Small resolution versions were used to not blow up the size of the theme and the repo.
The originals have much more detail.

The Markdownfiles in the content directory are
from the repository [hugoBasicExample](https://github.com/gohugoio/hugoBasicExample),
copyrighted by Steve Francia (2014)
and licensed under the [MIT license](https://mit-license.org/).
