# domfunc
## A functional Library for the DOM

Functional libraries are never quite what I'm looking for, either they don't automatically curry or they don't resemble vanilla JS enough.

### TODO

1. Convert all JS's most useful higher order functions to functional ones
2. Make constructors for other containers, from Sanctuary and Folktale
3. Make a JSX-like component syntax that doesn't require compilers (like Babel...yuk)

## Ideas
It could be cool if you could **compose** components together and treat them like their own type of container.

```javascript
import Posts from './posts.js'
import LayoutWithMenu from './layout-with-menu.js'

const Heading = component('<h1>Welcome</h1>')

render(
  compose(LayoutWithMenu, compose(append(Heading), append(Posts))) (props)
)

```
