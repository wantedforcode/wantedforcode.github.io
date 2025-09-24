# Wanted For Code

Un sitio web para desarrolladores creado usando Jekyll con el tema Agency.

## Ejecutar en Local

### Requisitos previos

- Ruby (versión 2.6.0 o superior)
- Bundler

### Pasos para ejecutar el proyecto

1. **Clonar el repositorio**

```bash
git clone <URL_DEL_REPOSITORIO>
cd wantedforcode
```

2. **Instalar las dependencias**

```bash
bundle install
```

3. **Iniciar el servidor local**

```bash
bundle exec jekyll serve
```

4. **Acceder al sitio**

Abre tu navegador y visita: [http://localhost:4000](http://localhost:4000)

### Uso con diferentes versiones de Ruby (rbenv)

Si tienes múltiples versiones de Ruby instaladas con rbenv:

```bash
# Ver versiones disponibles
rbenv versions

# Usar una versión específica en el proyecto
rbenv local 3.2.2

# Verificar que estás usando la versión correcta
ruby -v

# Instalar dependencias y ejecutar
bundle install
bundle exec jekyll serve
```

---

## Información Original del Tema

# [Agency Jekyll Theme](https://github.com/raviriley/agency-jekyll-theme) Starter Template
[![RubyGems Downloads](https://img.shields.io/gem/dt/jekyll-agency.svg)](https://rubygems.org/gems/jekyll-agency)
[![LICENSE](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://github.com/raviriley/agency-jekyll-theme/blob/master/LICENSE.txt)
[![Tip Me via PayPal](https://img.shields.io/badge/PayPal-tip%20me-green.svg?logo=paypal)](https://www.paypal.me/raviriley)

This is the fastest and easiest way to get up and running on GitHub Pages.
Simply generate your own repository by clicking the 
[![template button](https://img.shields.io/badge/-Use%20this%20template-brightgreen)](https://github.com/raviriley/agency-jekyll-theme-starter/generate) button, 
then replace the sample content with your own and configure for your needs.

If you want your website to be at `YOUR-USERNAME.github.io`, that's what you must name your repo. If you want it to be like this: `https://raviriley.github.io/agency-jekyll-theme-starter/`, them make sure the `baseurl` in `_config.yml` matches the name of your repo. You can also use a `CNAME` file and your own custom domain!

**If you enjoy this theme, please consider [supporting me](https://www.paypal.me/raviriley) to continue developing and maintaining it.**

[![Support via PayPal](https://cdn.rawgit.com/twolfson/paypal-github-button/1.0.0/dist/button.svg)](https://www.paypal.me/raviriley)
