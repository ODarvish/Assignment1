Hi Omid! Nice work!

I found a few issues, the main ones are:

File paths - because of the file paths the links and the image are not being found. You should just need to remove a word and remember that ../ refers to the parent directory and ./ refers to the current directory

Using float: please remove all floats and use flex box instead.

Duplicate CSS - see the comments below.

Can you please make the changes, push to github and let me know when I can take another look?

*************************************

CRITERIA FOR GRADING

*************************************

GODKÄNT:
-------------------------------------

3 separate pages: ✅

A header with a page title on every page: ✅ ❌
Google's SEO algorithim expects one and only one unique h1 on each page. You have 2 h1s on each page - I suggest changing "My website" to an h2 or similar

A navigational menu every page with links to the other pages: ❌
The links are broken

Contact form:
    Email: ✅
    Message: ✅
    Required: ✅
    Mail to: ✅
    Nice!

RWD:
    Desktop: ✅
    Mobile: ❌
    Don't use float - it removes an element from the normal page flow and can break a page - look at the home page on mobile. There is a spelling mistake in the media query, so Main goes to 100% and is not floated, but the sidebar styling doesn't change so it still floats. 
    
     Use flex or grid instead, and for this flex should work well.

External CSS: ✅

-------------------------------------

VÄLGODKÄNT:
-------------------------------------

Current page indication in the menu: ✅
  Should be done with a class

Responsive Image: ❌
  Path to the image is broken, I can't see it

RWD:
  Media Query: ✅
  Flex/Grid: ❌

Separate CSS: ✅ ❌
  There is a lot of duplication of common styles such as the header. A better approach is to crate a gerneral styling file andd move all the common styling (header, nav etc) to this file.
  The #1 rule in coding is to write everytthing just once!
  Semantic: ✅

Semantic Element naming: ✅ ❌
  Don't use ids unless there is a specific reason i.e. JavaScript will target that element. Classes are reuseable.

Code Style:
  HTML: ✅
    Files and directoris should be written in lowercase
  CSS: ✅
  Avoid inline styling: 
    <li style="background-color: rgb(109, 109, 109);"
  This should be done with a specific class
  This doesn't have a selector, so is broken:
  {
    margin: 0;
    padding: 0;
  }