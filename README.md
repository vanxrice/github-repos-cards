&lt;github-repos-cards&gt;
============

See the [component page](http://vanxrice.github.io/github-repos-cards/components/github-repos-cards) for more information.

## Live demo
See the [demo page](http://vanxrice.github.io/github-repos-cards/components/github-repos-cards/demo.html).

> A Polymer web component that displays git repository data from Github. This element was created to be used with Github's
API, and expects a response in the form of Github's API v3. A JSONP request is made for the provided request string. 

> The response object is exposed via data binding, and can be used to set the model or to use the request outside of this element, see the demo for an example.

> &lt;github-repo-card&gt; is the standalone card, it does not make any JSON request and may be used without &lt;github-repos-cards&gt;

## How To Use
Add to bower.json:
```json
{
  "dependencies": {
    "github-repos-cards": "~0.1.0"
  }
}
```
```html
<link rel="import" href="../github-repos-cards/github-repos-cards.html">
<!-- ... -->
<github-repos-cards maxRepoCount="5" response="{{ghResponse}}"
  request="https://api.github.com/users/vanxrice/repos?type=owner&sort=updated&direction=desc">
</github-repos-cards>
```

## Maintained by
- Vander Rice (Full-Stack Web Software Engineer)
- Twitter: [@van_rice](http://twitter.com/van_rice)
- Web: [http://vxrice.com](http://vxrice.com)

## License
Apache License Version 2.0, see LICENSE file
