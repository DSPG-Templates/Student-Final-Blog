# Final Reflection Blog

Write your answers to the questions here. Don’t forget to update the
metadata information above. Look through the [Markdown
Guide](https://quarto.org/docs/authoring/markdown-basics.html) to format
your text the way that you want it to be rendered.

![A picture you want to link here](imgs/The_Image.jpg)

## Assignment Objectives

For your two other submissions, you were asked to submit your answers
for areas of interest in your learning and other personal goals
throughout the DSPG program. This blog is meant to be a final reflection
of the progress you’ve made and the plans you have moving forward after
the program.

**Think of this blog as the blog that you would want potential employers
and others interested in your development to see.**

## What to Include in This Blog

As you prepare this blog, think about all the work and learning you’ve
put into your projects for DSPG. How do you want to demonstrate these
things to an external so that they can understand the the skills you’ve
been building.

Feel free to use the following as a guide to writing your blog.

- Can you elaborate on your learning throughout the program?
  - This encompasses both the technical and non technical knowledge
    you’ve gained.
  - What are skills you’ve picked up, observations you’ve made on data
    science work & the part of the projects which resonated most with
    you?
- Demonstrate some of your polished work from DSPG with an explanation
  of what it is and why you think it/they represent your work.
  - This could be an example of a data transformation code, a
    visualization, a map, etc.
- What new directions of learning are you now interested in pursuing
  after the end of the program.
- Do you think that you’ve met the goals you’ve outlined at the start of
  the program?

## Before Submitting Your Assignment

- Please update everything except the `categories: ["Final Reflection"]`
  in the YAML metadata section of your `NAME_Final_Blog.qmd` file.
- Replace the `NAME` section of the `NAME_Final_Blog.qmd` file with your
  first name.
- If you are including any images, place them in the `imgs\` folder and
  follow the guidelines discussed in the [Blog Writing Guidelines
  post](add%20link) for adding images.
  - The same practice holds for data to be in the `data` folder.
- Render the blog post locally on your device to make sure that it can
  render correctly. If you are in RStudio, you can use the Render icon
  or hit `Ctrl+Shift+K` on Windows and `Shift-Command-K` on Mac.

## Using Python Code Chunks

If you are using python in your code chunks you will need to run the
following at the top of your code, after the library imports. Set the
following chunks to `eval=TRUE`.

``` r
# Library for running python code in RStudio.
library(reticulate)
```

``` r
# Check for virtual environment, if it doesn't exist, create the venv, if it exists
# then use the venv called "r-python"

if (virtualenv_exists("r-python")) {
  use_virtualenv("r-python")
} else {
  virtualenv_create("r-python")
  use_virtualenv("r-python")
}
```

``` r
# Installing dependencies for the python virtualenv

virtualenv_install(envname = "r-python", packages = c("numpy", "pandas", "scikit-learn"), all = TRUE)
```
