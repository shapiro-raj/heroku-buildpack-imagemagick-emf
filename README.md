# heroku-buildpack-imagemagick-emf
Custom ImageMagick (with EMF) Buildpack

# Heroku Buildpack: ImageMagick with EMF support

This buildpack compiles libEMF and ImageMagick from source so that EMF/WMF formats
are supported inside a Heroku dyno.

## Usage

```bash
heroku buildpacks:clear -a <app>
heroku buildpacks:add --index 1 https://github.com/<youruser>/heroku-buildpack-imagemagick-emf.git -a <app>
heroku buildpacks:add --index 2 heroku/python -a <app>

