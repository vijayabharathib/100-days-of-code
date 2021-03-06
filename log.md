# 100 Days Of Code - Log

### Day 1: Jan 07, 2017

**Today's Progress**: Started styling components using SCSS

**Thoughts:** I had to go through customizing workflow to make sass work along with the project that I am working on. It was created using 'create-react-app', which doesn't support sass out of the box. CSS modules within the components broke some tests (as webpack didn't recognize css). ignore-styles came to rescue.

Cleaned up the travis.yml to work on it's own (without custom install and scripts sections).

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [Recipie App repository on GitHub]
---

### Day 2: Jan 08, 2017

**Today's Progress**: Completed styling the entire box using SCSS

**Thoughts:** Had to include few svgs as part of the styling process and a good learning trying to make svg work within react. Also configured workflow to accommodate modular scss. The box finally looks well and made it responsive to different viewports too. More than an hour today. Wanted to move on the ingredients coding, will have to wait until tomorrow.

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [Recipie App repository on GitHub]
---

### Day 3: Jan 14, 2017

**Today's Progress**: Started work on ingredients part of the recipie box

**Thoughts:** found it hard follow TDD, but had to keep that impulse to write app at check as I can already see TDD giving me good feedback on the existing code base.

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [Recipie App repository on GitHub]
---

### Day 4: Jan 15, 2017

**Today's Progress**: Continued work on ingredients part of the recipie box

**Thoughts:** coding this app with react and redux is overwhelming at times when things get messy with nested level of info. Had to go back to one step/one label/one button at time to stay motivated. finished the functional part of adding ingredients to recipies.

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [Recipie App repository on GitHub]
---

### Day 5: Jan 19, 2017

**Today's Progress**: Started designing ingredients with sass

**Thoughts:** messed up travis tests and automatic deployment to github pages as my commit didn't include the new style files. it was working locally as the file system had all necessary files. however, since the commit did not have few files, tests were failing only during travis CI build process. Apart from that, the styling comes out good and looks lively now.

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [Recipie App repository on GitHub]
---

### Day 6: Jan 21, 2017

**Today's Progress**: Continued designing ingredients with sass

**Thoughts:** picked up css triangle again to mark UX for collapsed/expanded modes. also sorted out design for the form to add ingredients. add recipie text box also got a placeholder.

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [Recipie App repository on GitHub]
---

### Day 7: Jan 22, 2017

**Today's Progress**: Started coding ingredient maintenance (delete)

**Thoughts:** easier to prepare the actions and reducers. with recipie id and ingredient id, the reducer is able to remove the ingredient from the store. I see paters of code duplication, potential refactoring opportunity. starting the DOM implementation through react components seems to be hard - this is because ingredient is now just a presentational component - with no onclick callback..etc. One for tomorrow.

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [manage-ingredient branch on github repository]
---

### Day 8: Jan 23, 2017

**Today's Progress**: TDD integration test

**Thoughts:** wrote an integration test (TDD) for deleting an ingredient. the set up block (to set up few recipies and ingredients) spoiled all the other tests. the action creators had global id variable to create unique id each time. adding test changes the number and other tests were expecting different numbers. proper setup and tear down will solve it - started with a flush function to reset the globals. now there is only one (expected) failure. next step is to actually create the function and link it to the onclick of delete button to pass the failing test.

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [Recipie App repository on GitHub]
---

### Day 9: Jan 24, 2017

**Today's Progress**: delete ingredient TDD green

**Thoughts:** finally, simple use of dispatch (instead of trying to wrap around custom made transmit) worked. able to delete ingredients now. this was not like the recipie list & recipie component, as ingredient list also had a form to add new ingredients. i'll have to refactor either recipie/ingredient to match one another. for now, the last bit is to make the ingredients editable. another two/three days, and should be done with this project.

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [Recipie App repository on GitHub]
---

### Day 10: Jan 26, 2017

**Today's Progress**: edit ingredient TDD green

**Thoughts:** edit ingredient is now working. enabled cache for node_modules in travis. That shaved about a minute. Build time came down from 2 to 1 min. Styling for edit ingredient is also complete and looks good now.

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [Recipie App repository on GitHub]
---

### Day 11: Jan 27, 2017

**Today's Progress**: started refactoring the project

**Thoughts:** reducers first. It had a lot of duplication of loops to find the recipie by id. to follow DRY, extracted a few of them into separate functions of their own.

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [Recipie App repository on GitHub]
---

### Day 12: Jan 28, 2017

**Today's Progress**: a lot more refactoring

**Thoughts:** spent several hours refactoring reducers and components. started extracting container and presentational components.

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [Recipie App repository on GitHub]
---

### Day 13: Jan 28, 2017

**Today's Progress**: local storage

**Thoughts:** enabled local storage to rehydrate the app when it starts. had to refactor some of the reducers which wouldn't fit. Hence, uuid was used to generate unique ids.

**Link to work:**

1. [Recipie App on GitHub Pages]
2. [Recipie App repository on GitHub]
---
# REBOOT
## Completed React Recipie project and another project [Game of life], without any logs. Reboot to start logging again.

### Day 1: March 07, 2017

**Today's Progress**: Started with the dungeon crawler project

**Thoughts:** It was pretty hard to get through the dev environment set up though I just had to use the last project [game of life] as base. Finally, the maze was up and running

**Link to work:**

1. [Dungeon Crawler Game on GitHub Pages]
2. [Dungeon Crawler repository on GitHub]
---
### Day 2: March 08, 2017

**Today's Progress**: Created a player and moved him around

**Thoughts:** It is very tempting to jump right into solution. Had to keep myself from getting ahead of me and wrote some tests around player movement. The results are good. Game is kind of shaping up and pieces are falling into place. Handled arrow key press events to move player.

**Link to work:**

1. [Dungeon Crawler Game on GitHub Pages]
2. [Dungeon Crawler repository on GitHub]

---

[Below are references to links used in the doc]: http://vijayabharathi.in
[Recipie App on GitHub Pages]: https://vijayabharathib.github.io/fcc-project-react-recipies
[Recipie App repository on GitHub]: https://github.com/vijayabharathib/fcc-project-react-recipies
[Dungeon Crawler Game on GitHub Pages]:http://vijayabharathib.github.io/fcc-project-dungeon-crawler
[Dungeon Crawler repository on GitHub]:https://github.com/vijayabharathib/fcc-project-dungeon-crawler
