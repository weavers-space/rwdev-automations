
# RapidWeaver Community Screenshot Submission tool

### Requirements

[Fake.app](https://itunes.apple.com/us/app/fake/id402356565?mt=12&at=11l8IQ) is what powers this entire thing! You will need to purchase it.


### How to Use

1. Create your `screenshots.txt` file with all your product info. More info below.
2. Make sure that you are logged into the RapidWeaver Community site.
3. Open the Fake workflow and press the play button.
4. Sit back and enjoy. There are some AppleScript keyboard hacks in here, so do not use other apps until this is complete.


### screenshots.txt

This file should be in the same folder as the Fake workflow file. I created this file via a ruby script that queried my database. You are on your own for creating this.

Here is the template for creating the file:

> id::image

#### Tips

* Each field needs to be separated by 2 colons `::`
* _image_ needs to be the full path to the screenshot on your local machine.
