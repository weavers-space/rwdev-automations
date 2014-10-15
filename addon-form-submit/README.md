
# RapidWeaver Community Addon Automation Tool

I wrote a cool tool that will automate the creation of adding addons to the RapidWeaver Community Addons site. It loops through a text file and processes each line with the data defined for the product.

### Requirements

[Fake.app](https://itunes.apple.com/us/app/fake/id402356565?mt=12&at=11l8IQ) is what powers this entire thing! You will need to purchase it.


### How to Use

1. Create your `rwaddons.txt` file with all your product info. More info below.
2. Make sure that you are logged into the RapidWeaver Community site.
3. Open the Fake workflow and press the play button.
4. Sit back and enjoy. There are some AppleScript keyboard hacks in here, so do not use other apps until this is complete.


### rwaddons.txt

This file should be in the same folder as the Fake workflow file. I created this file via a ruby script that queried my database. You are on your own for creating this.

Here is the template for creating the file:

> type::title::description::keywords::price::icon::homepage::store::download::preview::video::date::version::build::bundleId::notes

#### Tips

* Each field needs to be separated by 2 colons `::`
* There must be no newline characters. However, `\n` will get interpreted as newlines when inserted into the form.
* The currency is hard coded into the workflow. Look at the JS code block in the workflow and you will see the varaible where to change it from USD. Other options are: GPB, EUR, CAD
* If any of the data elements need to be blank on the form (Ex: download url), simply put a space into the slot. (Having four colons in a row will break it)
* _type_ is either: theme, plugin, stack
* _keywords_ is a comma delimted list of keywords. No spaces.
* _icon_ needs to be the full path to the 512px icon on your local machine.


### TODO

* This tool does not upload any screenshots to the gallery yet.
* I will also be doing a version that will update exisitng addons. (Examples: add screenshots, change version, etc.)
