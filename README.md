Welcome to the official website of FRC team 3324, the Metrobots! This repository houses the complete codebase and asset library that powers our team’s online presence. This website serves as a comprehensive digital platform designed to connect and engage with our diverse audiences, including team members, mentors, sponsors, alumni, and our broader community.

This website was fully created with GitHub Pages, using Codepen.io for quicker prototyping. I enjoy putting all of the code within the HTML, because it makes my coding mentors upset. This means there are no `.js` (except for one list) or CSS styling files; everything is contained within `<script>` and `<style>` tags. If you find any inconsistencies or have a fun change to implement, feel free to contribute! Have a great time exploring!

All the best,  
Mateo Johnson (Metrobots 3324)


# Project File Structure

* **root** / (The home directory, everything is contained in here)
  * **about** / (The section for about our team)
    * **gallery** / (The section where photos from across the team's history are stored)
      * `index.html`
    * **leadership** / (The section where you can learn about our current leadership team)
      * `index.html`
    * `index.html`
  * **assets** / (Contains all the assets for the website, as well as connected sites)
    * **documents** / (Contains all of the pertinent documents for the current season)
      * `Calendar 24-25.ics`
      * `Season 24-25.md`
    * nothing else that's important (There are just a bunch of images, and I don't feel like listing them)
  * **docs** / (The documentation practices page)
    * `index.html`
  * **document** / (This is an unlinked page that is used for the [documentation form](https://metrobots.github.io/document))
    * `index.html`
  * **gallery** / (This is a second unlinked page that is used for the [documentation gallery](https://metrobots.github.io/gallery))
    * `index.html`
  * **matchsim** / (This is a third unlinked page that leads to the [match sim](https://metrobots.github.io/matchsim))
    * `index.html`
    * `teams.js` (THIS IS THE ONYL FULL JS FILE IN THE ENTIRE PROJECT, IT CONTAINS ALL TEAMS INFO, 1-10,000)
  * **mission** / (The page that talks about our community involvement)
    * `index.html`
  * **our-season** / (The page that gives our calendar for the current season, along with competition info)
    * **currentgame** / (The page that provides information about the current FRC game)
      * `index.html`
    * **robot-design** / (The page that provides information about robot design principles)
      * `index.html`
    * `index.html`
  * **resources** / (A folder that contains resources for the team: social media links, swervesim, scouting app, etc.)
    * **calendartool** / (This is a fourth unlinked page that leads to the [calendar tool](https://metrobots.github.io/resources/calendartool))
      * `index.html`
    * **scouting** / (The page that contains our match scouting form)
      * `index.html`
    * **swervesim** / (The page that contains our 2D swerve simulator (controller only))
      * `index.html`
    * `index.html`
  * `README.md` (**YOU ARE HERE**)
  * `index.html` (The homepage)
