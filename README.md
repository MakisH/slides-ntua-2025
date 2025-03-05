# preCICE talk at the SIAM CSE25

- Title: Black-box coupling of simulation codes using preCICE
- Speaker: Gerasimos Chourdakis, University of Stuttgart
- Authors: Gerasimos Chourdakis + [more](https://www.precice.org/about/)
- Event: [SIAM CSE25](https://www.siam.org/conferences-events/siam-conferences/cse25/), Fort Worth, Texas, USA
- Date: March 5, 2025

[Start the presentation](https://makish.github.io/slides-cse25/) - [Get the PDF](https://github.com/MakisH/slides-cse25/blob/master/slides-archive.pdf)

This is an overview talk. Are you looking for training? Consider joining the [preCICE Workshops](https://precice.org/precice-workshop.html) or [supporting preCICE](https://precice.org/community-support-precice).

## Build

Follow the instructions on [reveal.js](https://revealjs.com/installation/), or just install Node.js 10.0.0 or later and do:

```bash
npm install
npm start
```

and go to [localhost:8000](http://localhost:8000/) to see the slides.

## Convert to PDF

See section "[Export to PDF](https://revealjs.com/pdf-export/)" in the reveal.js documentation.

[Decktape](https://github.com/astefanutti/decktape) does a marvelous job converting this presentation to PDF. Get the Docker image (see Decktape README) and run (for localhost):

```bash
docker run --rm -t --net=host -v "$(pwd)":/slides astefanutti/decktape generic --key=" " -p 2000 -s 1920x1440 http://localhost:8000 slides-archive.pdf
```

## License & more

- License: [CreativeCommons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/)
- Based on [reveal.js](https://github.com/hakimel/reveal.js). Template based on the "White" template by Hakim El Hattab.
- The University of Stuttgart logo is part of the corporate identity of the University of Stuttgart.
