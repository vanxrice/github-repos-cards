# &lt;github-repos-cards&gt;
A Polymer web component that displays git repository data as a grid collection of cards. The &lt;github-repo-card&gt; displays basic repo information, including: stargazer/watcher count, repo description, a link to the README, default branch and last commit time, and includes a download link. &lt;github-repo-card&gt; is the standalone card, it does not make any request and may be used without &lt;github-repos-cards&gt;. This project intentionally does not define much styling (CSS or otherwise), you should style these elements in your application so they integrate well.

This element was intended to be used with Github's API, and expects a response in the form of Github's API v3. However requests are not restricted to Github, a JSONP request is made for the provided request string - this allows you to use a different REST API.

The response object is exposed as `response`, this can be used to manually set the model or to use the request outside of this element. See the demo for an example that sums stargazers.

See the [component page](http://vanxrice.github.io/github-repos-cards/components/github-repos-cards) for more information.

## Live demo
See the [demo page](http://vanxrice.github.io/github-repos-cards/components/github-repos-cards/demo.html).

## How To Use
### Installation
Available on [Bower](http://bower.io) as **github-repos-pages**.

Add to bower.json:
```json
{
  "dependencies": {
    "github-repos-cards": "~0.1.0"
  }
}
```

### Usage
This component is built using [Polymer](https://www.polymer-project.org/) and uses the [Web Component](http://webcomponents.org/) stack.

```html
<!-- … -->
<script src="../webcomponentsjs/webcomponents.js"></script>

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

Copyright © 2014 [@van_rice](http://twitter.com/van_rice)
