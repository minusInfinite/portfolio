# Person Portfolio

This is my Portfolio WIP for a Full-Stack Boot Camp I'm participating in.
You can find the delopment of this task at https://minusinfinite.github.io/portfolio/

## Task Requirements

For this task, we're given the following User Story

> AS AN employer
> I WANT to view a potential employee's deployed portfolio of work samples
> SO THAT I can review samples of their work and assess whether they're a good candidate for an open position

As well as the following Acceptance Criteria

> GIVEN I need to sample a potential employee's previous work
> WHEN I load their portfolio
> THEN I am presented with the developer's name, a recent photo or avatar, and links to sections about them, their work, and how to contact them
> WHEN I click one of the links in the navigation
> THEN the UI scrolls to the corresponding section
> WHEN I click on the link to the section about their work
> THEN the UI scrolls to a section with titled images of the developer's applications
> WHEN I am presented with the developer's first application
> THEN that application's image should be larger in size than the others
> WHEN I click on the images of the applications
> THEN I am taken to that deployed application
> WHEN I resize the page or view the site on various screens and devices
> THEN I am presented with a responsive layout that adapts to my viewport

## Process of development

I believe I have followed the above requirements with the following examples.
When you go to my [porfolio](https://minusinfinite.github.io/portfolio/)
You will see a Header and Navigation that is fixed to the Viewpoint. The links are booked marked via anchor tags and ID on page sections.

Below is an example from my index.html

```
<header>
    <h1>Porfolio - Ashley Mann</h1>
    <nav>
        <a href="#about-me">About Me</a>
            <a href="#projects">Projects</a>
            <a href="#contact">Contact</a>
            <a href="https://github.com/minusInfinite" target="_blank"
            >Github</a>
            </nav>
</header>
<main>
    <section id="about-me">
        <h2>About Me</h2>
```

The following CSS allows for the section links to scroll smoothly

```
html {
    scroll-behavior: smooth;
}
```

I have used the CSS option of Flex to allow my navigation and Project images to adjust to the browser viewpoint. Media Queries have also been added to change the navigation from an inline to a block list of links if given the viewpoints pixel width.

To demonstrate a link to a project, I've used the example of our first homework task as the first project. The image will link to the Github page deployment with the figure caption having a link to the Github repository
