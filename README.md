Pipal Academy Website
=====================

Official website of the Pipal Academy.
Initiated by Miranj on 29 Aug 2016.


Install
-------

1.  Ensure the following requirements are installed:
    - Ruby 2.3+
    - Jekyll 3.2+
    
2.  Build the site
        
        $ jekyll build
    
3.  Create an Apache config file and update the `RewriteBase`
    directive if required.
        
        $ cp templates/sample.htaccess templates/.htaccess
        $ vi templates/.htaccess
    
4.  Access the generated ./_site folder from your browser



Development
-----------

1.  Create an environment specific config file
    if required (eg. to override `baseurl`):
    
        $ cp sample_env_config.yml _env_config.yml
        $ vi _env_config.yml  

2.  Install dev tools:
    - Node.js http://nodejs.org
    - Gulp http://gulpjs.com/
    
        $ cd assets & npm install

3.  Enable continuous builds of the site
    
        $ jekyll build --watch --config _config.yml,_env_config.yml

4.  Enable continuous builds of the assets
    
        $ gulp

