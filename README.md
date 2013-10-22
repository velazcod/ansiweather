## Description

AnsiWeather is a Shell script for displaying the current weather conditions in your
terminal, with support for ANSI colors and Unicode symbols.

![AnsiWeather Screenshot](http://www.cambus.net/content/2013/10/ansiweather-moscow.png)

Weather data comes from the `OpenWeatherMap` free weather API.

## Requirements

AnsiWeather requires the following dependencies : 

- A command to fetch HTTP data such as [cURL](http://curl.haxx.se) or [wget](https://www.gnu.org/software/wget/)
- jq (lightweight and flexible command-line JSON processor) : http://stedolan.github.io/jq/

## Usage

After cloning the repository, simply invoke the script by typing :

	./ansiweather

## Configuration

The following configuration options are available and should be set according
to your location and preferences.

Config options can also be set in ~/.ansiweatherrc

Example : `~/.ansiweatherrc`

	location:5391959
	fetch_cmd:ftp -V -o -
	units:metric
        

### Location

Example : `5391959`

	location:5391959
	
Find your city ID by making this call and replacing the 'q' param with your city name and state:
http://api.openweathermap.org/data/2.5/find?q=San%20Francisco%2CCA&mode=json

### System of Units

Both `metric` and `imperial` systems are supported.

	units:metric

### Display symbols

Toggle Unicode symbols display. Value can be either `true` or `false` (requires an Unicode capable display).

	symbols:true

## License

AnsiWeather is released under the BSD 3-Clause license. See `LICENSE` file
for details.

## Author

AnsiWeather is developed by Frederic Cambus

- Site : http://www.cambus.net
- Twitter: http://twitter.com/fcambus

## Resources

GitHub : https://github.com/fcambus/ansiweather
