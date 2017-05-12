# Colorname

[![Build Status](https://travis-ci.com/celilileri/colorname.svg?token=qSHr3MpL5P1vaDoy2yPE&branch=master)](https://travis-ci.com/celilileri/colorname)

Ruby Gem for decide name of a given color.

## Installation

### Easy Gem Installation

```shell
$ gem install colorname
```
### Gemfile  Integration

Add this line to your application's Gemfile:

```ruby
gem 'colorname'
```

And then execute:
```
$ bundle
```
## Usage

```ruby
Colorname.find 'f0f8ff'                    # [:aliceblue]

Colorname.find '#00ffff'                   # [:aqua, :cyan]

Colorname.find 143, 188, 143               # [:darkseagreen]

Colorname.find Color::RGB.new(255, 0, 255) # [:fuchsia, :magenta]
```

To find names of most dominant colors of and image

```ruby
Colorname.find_by_image (url_or_path)       # [:names_of_most_dominant_colors]
Colorname.findbyimage (url_or_path)         # [:names_of_most_dominant_colors]

```


To find dominant base color name

```ruby
Colorname.base '32cd32'                    # [:green]

Colorname.base '#FF00CC'                   # [:red]

Colorname.base 25, 150, 255                # [:blue]

Colorname.base Color::RGB.new(255, 0, 255) # [:red, :blue]

```

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/celilileri/colorname. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

