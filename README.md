Bookmark.tmbundle
=================
Create bookmarks through comments which show in the symbol browser.
## Usage
Works with languages where single-line comments start with `//` or `#`
In single-line comments, add a `!` before any non-whitespace characters to create a bookmark. The text you enter after the `!` will be the label for the bookmark in the symbol browser.

## Example

`example.rb`
    
    ...
    # ! remember this place
    def output str
      puts str
    end
    ...
    #! this method is too long, come back and refactor
    def long_method
      ...
    end
    ...

`example.php`

    <?php
    ...
    // ! remember this place
    function output(str){
      echo str;
    }
    ...
    //! this method is too long, come back and refactor
    function long_method(){
      ...
    }
    ...

## Installation
First, ensure the TextMate bundle directory exists, and create it if it doesn't:

    mkdir -p ~/Library/Application Support/Avian/Bundles

Then, clone this repo to get the bundle:
    
    git clone https://github.com/bananastalktome/Bookmark.tmbundle.git ~/Library/Application Support/Avian/Bundles/Bookmark.tmbundle`
    
    
You could also manually download and copy the file in place, but then you won't be able to `git pull` for updates (which AFAIK TextMate doesn't automatically do for custom bundles).
