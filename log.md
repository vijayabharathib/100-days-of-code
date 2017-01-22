# 100 Days Of Code - Log

### Day 1: Jan 07, 2017

**Today's Progress**: Started styling components using SCSS

**Thoughts:** I had to go through customizing workflow to make sass work along with the project that I am working on. It was created using 'create-react-app', which doesn't support sass out of the box. CSS modules within the components broke some tests (as webpack didn't recognize css). ignore-styles came to rescue.

Cleaned up the travis.yml to work on it's own (without custom install and scripts sections).

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [Recipie App repository on GitHub]

### Day 2: Jan 08, 2017

**Today's Progress**: Completed styling the entire box using SCSS

**Thoughts:** Had to include few svgs as part of the styling process and a good learning trying to make svg work within react. Also configured workflow to accommodate modular scss. The box finally looks well and made it responsive to different viewports too. More than an hour today. Wanted to move on the ingredients coding, will have to wait until tomorrow.

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [Recipie App repository on GitHub]

### Day 3: Jan 14, 2017

**Today's Progress**: Started work on ingredients part of the recipie box

**Thoughts:** found it hard follow TDD, but had to keep that impulse to write app at check as I can already see TDD giving me good feedback on the existing code base.

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [Recipie App repository on GitHub]

### Day 4: Jan 15, 2017

**Today's Progress**: Continued work on ingredients part of the recipie box

**Thoughts:** coding this app with react and redux is overwhelming at times when things get messy with nested level of info. Had to go back to one step/one label/one button at time to stay motivated. finished the functional part of adding ingredients to recipies.

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [Recipie App repository on GitHub]


### Day 5: Jan 19, 2017

**Today's Progress**: Started designing ingredients with sass

**Thoughts:** messed up travis tests and automatic deployment to github pages as my commit didn't include the new style files. it was working locally as the file system had all necessary files. however, since the commit did not have few files, tests were failing only during travis CI build process. Apart from that, the styling comes out good and looks lively now.

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [Recipie App repository on GitHub]



### Day 6: Jan 21, 2017

**Today's Progress**: Continued designing ingredients with sass

**Thoughts:** picked up css triangle again to mark UX for collapsed/expanded modes. also sorted out design for the form to add ingredients. add recipie text box also got a placeholder.

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [Recipie App repository on GitHub]

### Day 7: Jan 22, 2017

**Today's Progress**: Started coding ingredient maintenance (delete)

**Thoughts:** easier to prepare the actions and reducers. with recipie id and ingredient id, the reducer is able to remove the ingredient from the store. I see paters of code duplication, potential refactoring opportunity. starting the DOM implementation through react components seems to be hard - this is because ingredient is now just a presentational component - with no onclick callback..etc. One for tomorrow.

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [manage-ingredient branch on github repository]


[Below are references to links used in the doc]: http://vijayabharathi.in
[Recipie App on GitHub Pages]: https://vijayabharathib.github.io/fcc-project-react-recipies
[Recipie App repository on GitHub]: https://github.com/vijayabharathib/fcc-project-react-recipies
