# h2i
Pull data from homematic ccu via xmlapi and stores them inside a time series database like influxdb.

## Install
Easy and strait forward. Just 3 steps are neede:
1. Download and unpack the zip file or clone the git repository.
2. Edit the settings section of h2i file with you desired program editor.
3. Move the h2i file to /usr/local/bin.
Now h2i is ready to use.

## Use
<pre>
Usage:  
  h2i [command] [option]  

Available Commands:  
  version, -v, --version     - Print version information  
  help, -h, --help           - Print this help message  
  pull, -p, --pull           - Gets values from given device ids  

Available Options:  
  debug, -d, --debug         - Enables Debug informations  
</pre>

## ToDo
* Update README with install and use instructions. Write short info on how to use group by function in grafana for getting all values of one type.
* Add list command for getting and showing available device ids and types.
* Use GNU parallel to speed up the parsing process if avaiable.
* Outsource settings and list of id's into a separate file.
* Add install/update command.
* Add option for silent-run and dry-run.

## Changelog
1.2.2
* Add settings section.
* Update README with install an use info.

1.2.1
* Check if connection to ccu can be made and give error message if not.
* Clean up staelist on program finish.
* Silend run of curl und xmllint.

1.2.0
* Check enviroment for needed programs and give sugesstions on how to install them.

1.1.0
* Better code documentation.

1.0.0
* Initial Version with basic feature set.

## Authors
Torsten Scholz (exolon)

## Licence
GNU LGPLv3

## Disclaimer
You use this project at your own risk. This is not a solution that should be used in productive environments, but this code and guide could give you a quick start for your own experiments. Please keep also in mind that there are currently some security features missing.
