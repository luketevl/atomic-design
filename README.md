# atomic-design

# Links http://atomicdesign.bradfrost.com/

![Chemical Equation - An example of a chemical equation showing hydrogen and oxygen atoms combining together to form a water molecule.](http://atomicdesign.bradfrost.com/images/content/chemical-equation.png)


# TL;DR
- **Atoms** are UI elements that can’t be broken down any further and serve as the elemental building blocks of an interface.
- **Molecules** are collections of atoms that form relatively simple UI components.
- **Organisms** are relatively complex components that form discrete sections of an interface.
- **Templates** place components within a layout and demonstrate the design’s underlying content structure.
- **Pages** apply real content to templates and articulate variations to demonstrate the final UI and test the resilience of the design system.

![Atomic design applied to the native mobile app Instagram.](http://atomicdesign.bradfrost.com/images/content/instagram-atomic.png)

# Atomic design guide

> Atomic design is a methodology composed of five distinct stages working together to create interface design systems in a more deliberate and hierarchical manner

![Atomic design is atoms, molecules, organisms, templates, and pages concurrently working together to create effective interface design systems.](http://atomicdesign.bradfrost.com/images/content/atomic-design-process.png)

# STAGES

## Atoms

![Atoms](http://atomicdesign.bradfrost.com/images/content/atomic-design-atoms.png)

- Are the basic building blocks of all matter. Each chemical element **has distinct properties**, and they **can’t be broken** down further without losing their meaning
- These ***atoms** include basic **HTML elements** like form _labels, inputs, buttons_, and others that can’t be broken down any further without ceasing to be _functional_.
- Are the smallest _functional unit_

![Atoms include basic HTML tags like inputs, labels, and buttons](http://atomicdesign.bradfrost.com/images/content/atoms-form-elements.png)

- Each interface **atom** has its own _unique properties_, such as the _dimensions_ of a hero image, or the _font size_ of a primary heading

## Molecules

![Molecules](http://atomicdesign.bradfrost.com/images/content/atomic-design-molecules.png)

- Are _groups of_ **two or more atoms** held together by chemical bonds. These combinations of **atoms** take on their own unique properties, and become more tangible and operational than **atoms**.
- Are groups of **atoms** bonded together that take on _distinct new properties_.
- For example, a form label, search input, and button can join together to create a search form **molecule**.
![A search form molecule is composed of a label atom, input atom, and button atom.](http://atomicdesign.bradfrost.com/images/content/molecule-search-form.png)

- Creating simple components helps UI designers and developers adhere to the **single responsibility principle**, an age-old computer science precept that encourages a **“do one thing and do it well”** mentality. Burdening a single pattern with too much complexity makes software unwieldy. Therefore, creating simple UI **molecules** makes _testing easier_, encourages **reusability**, and promotes **consistency** throughout the interface.

## Organisms

![Organisms](http://atomicdesign.bradfrost.com/images/content/atomic-design-organisms.png)

- Are assemblies of **molecules** functioning _together_ as a **unit**. 
- While some organisms might consist of different types of molecules, other organisms might consist of the same molecule repeated over and over again.

![This header organism is composed of a search form molecule, logo atom, and primary navigation molecule.](http://atomicdesign.bradfrost.com/images/content/organism-header.png)

## Templates

![Templates](http://atomicdesign.bradfrost.com/images/content/atomic-design-templates.png)

- Templates are page-level objects that place components into a layout and articulate the design’s underlying content structure.

![The homepage template consists of organisms and molecules applied to a layout.](http://atomicdesign.bradfrost.com/images/content/template.png)

- Important characteristic of **templates** is that they focus on the page’s underlying content structure rather than the page’s final content. Design systems must account for the dynamic nature of content, so it’s very helpful to articulate important properties of components like image sizes and character lengths for headings and text passages.

![Time Inc.'s homepage template demonstrates the content's underlying structure.](http://atomicdesign.bradfrost.com/images/content/template-timeinc-homepage.png)

## Pages

![Pages](http://atomicdesign.bradfrost.com/images/content/atomic-design-pages.png)

- **Pages** are specific instances of **templates** that show what a UI looks like with real representative content in place. Building on our previous example, we can take the homepage template and pour representative text, images, and media into the template to show real content in action.

![The page stage replaces placeholder content with real representative content to bring the design system to life.](http://atomicdesign.bradfrost.com/images/content/page.png)

- The **page** _stage_ is the most concrete stage of **atomic design**
- This is what users will see and interact with when they visit your experience.
- And this is where you see all those **components** coming together to form a beautiful and _functional user interface_.

> In addition to demonstrating the final interface as your users will see it, pages are essential for testing the effectiveness of the underlying design system. It is at the page stage that we’re able to take a look at how all those patterns hold up when real content is applied to the design system.

![At the page stage, we're able to see what Time Inc.'s homepage looks like with real representative content in place. With actual content in place, we're able to see if the UI components making up the page properly serve the content being poured into them.](http://atomicdesign.bradfrost.com/images/content/page-timeinc-homepage.png)


# ADVANTAGES OF ATOMIC DESIGN

## The part and the whole

> One of the biggest advantages atomic design provides is the ability to quickly shift between abstract and concrete. We can simultaneously see our interfaces broken down to their atomic elements and also see how those elements combine together to form our final experiences.

![Atomic design allows designers to traverse between abstract and concrete.](http://atomicdesign.bradfrost.com/images/content/atomic-design-abstract-concrete.png)

## Clean separation between structure and content
> A well-crafted design system caters to the content that lives inside it, and well-crafted content is aware of how it’s presented in the context of a UI. The interface patterns we establish must accurately reflect the nature of the text, images, and other content that live inside them. Similarly, our content should be aware of the manner in which it will be presented. The close relationship between content and design requires us to consider both as we construct our UIs.

> Atomic design gives us a language for discussing the structure of our UI patterns and also the content that goes inside those patterns. While there is a clean separation between the content structure skeleton (templates) and the final content (pages), atomic design recognizes the two very much influence each other. For instance, take the following example:

![Layout vs Page](http://atomicdesign.bradfrost.com/images/content/templates-pages-users-example.png)

> On the left we see the UI’s content skeleton, which consists of the same person block molecule repeated again and again. On the right we see what happens when we populate each instance of the person block molecule with representative content. Visualizing the content skeleton and the representative final content allows us to create patterns that accurately reflect the content that lives inside them. If a person’s name were to wrap onto five lines within the pattern, we would need to address that broken behavior at a more atomic level.

> The content we pour into our UIs at the page stage will influence the characteristics and parameters of the underlying design patterns.



# PATTERN LAB

![This is what Pattern Lab's patterns folder structure can look like. You can name and categorize these folders however you'd like, including changing the labels “atoms”, “molecules”, and “organisms”, “templates”, and ”pages”. The most important consideration is to establish naming and categorization that is most effective for your team.](http://atomicdesign.bradfrost.com/images/content/pattern-lab-file-structure.png)


# OBSERVATIONS
- Mustache
