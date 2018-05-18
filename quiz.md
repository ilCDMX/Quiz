A top-level `App` component returns `<Button />` from its `render()` method.

1. What is the relationship between `<Button />` and `this` in that `Button`’s `render()`?
   <Button/> is an element from render(). 'this' refers to the element of render() once it has been instantiated.
   <Button/>is an element that will be render and instantiated, and 'this' will be a reference to the instance of that element

2. Does rendering `<Button><Icon /></Button>` guarantee that an `Icon` mounts?
   No. An independent element can be rendered if instructed to. The elements that derive from an element can only be 
   rendered if the father is being render. The children of the element may not be rendered even if the father is being
   rendered.

   Each element can be rendered, but will only render if the element they are children of is being rendered.
   The father may as well skip the children's render.

3. Can the `App` change anything in the `Button` output? What and how?
   It may change the button properties or his children. 
