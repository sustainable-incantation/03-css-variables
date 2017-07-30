# CSS Variables

We all know about **Sass** and **variables** used in it.

**Q.** *So why are we discussing about CSS Variables if we already have a way to define them in Sass?*  
**A.** There is something that CSS Variables can do which Sass Variables can't.  
##### CSS Variables can be modified at run-time using JS, whereas Sass variables are set at compile-time and thus can't be modified later.  

***That is why we use CSS Variables.***


## Syntax

### How to define?
The CSS Variables are **always defined inside scope**.

For instance:

**Wrong**

    <style>
      --base-color: yellow;
    </style>

**Right**

    <style>
      element {
      --base-color: yellow;    
      }
    </style>

### How to use?

The variables are referenced (in CSS) using **var(--variablename)**.  

For instance:

    <style>
      element {
      --base-color: yellow;    
      }

      img {
        background: var(--base-color);
      }
    </style>
