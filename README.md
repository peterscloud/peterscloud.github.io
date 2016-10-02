# peterscloud.github.io
Peter's Cloud Pages

To build the site use:

jekyll build --config _config.yml,_config_dev.yml

To test the site in the development enviroment use:

cd peterscloud.github.io/site && ruby -rwebrick -e 'WEBrick::HTTPServer.new(:Port=>8080,:DocumentRoot=>".").start'

The following serve command won't work, because it's going to rebuild the site without the--config option when a file is changed:

cd peterscloud.github.io && jekyll serve --port 8080 --host 0.0.0.0  --skip-initial-build