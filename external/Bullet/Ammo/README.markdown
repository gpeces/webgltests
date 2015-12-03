



<!DOCTYPE html>
<html lang="en" class=" is-copy-enabled emoji-size-boost">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    <meta name="viewport" content="width=1020">
    
    
    <title>ammo.js/README.markdown at master · kripken/ammo.js · GitHub</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-144.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="kripken/ammo.js" name="twitter:title" /><meta content="ammo.js - Direct port of the Bullet physics engine to JavaScript using Emscripten" name="twitter:description" /><meta content="https://avatars3.githubusercontent.com/u/173661?v=3&amp;s=400" name="twitter:image:src" />
      <meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="https://avatars3.githubusercontent.com/u/173661?v=3&amp;s=400" property="og:image" /><meta content="kripken/ammo.js" property="og:title" /><meta content="https://github.com/kripken/ammo.js" property="og:url" /><meta content="ammo.js - Direct port of the Bullet physics engine to JavaScript using Emscripten" property="og:description" />
      <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">
    <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">
    <link rel="assets" href="https://assets-cdn.github.com/">
    
    <meta name="pjax-timeout" content="1000">
    

    <meta name="msapplication-TileImage" content="/windows-tile.png">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="selected-link" value="repo_source" data-pjax-transient>

    <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
    <meta name="google-analytics" content="UA-3769691-2">

<meta content="collector.githubapp.com" name="octolytics-host" /><meta content="github" name="octolytics-app-id" /><meta content="CA53F39D:4841:16053B:565FB32F" name="octolytics-dimension-request_id" />
<meta content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-pjax-transient="true" name="analytics-location" />
<meta content="Rails, view, blob#show" data-pjax-transient="true" name="analytics-event" />


  <meta class="js-ga-set" name="dimension1" content="Logged Out">
    <meta class="js-ga-set" name="dimension4" content="New repo nav">




    <meta name="is-dotcom" content="true">
        <meta name="hostname" content="github.com">
    <meta name="user-login" content="">

      <link rel="mask-icon" href="https://assets-cdn.github.com/pinned-octocat.svg" color="#4078c0">
      <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">

    <meta content="fe902029b1d6a42b7e0ac4ef85e4d29d9d7bfe9a" name="form-nonce" />

    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/github-d7e0b0c4fd7711345cdfc8fa9695541f6b64640cfc5897e9ea2337eba685ec9c.css" integrity="sha256-1+CwxP13ETRc38j6lpVUH2tkZAz8WJfp6iM366aF7Jw=" media="all" rel="stylesheet" />
    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/github2-a2501013b84e6062c9171a31d4fdb2225390126ddc5d8453188bc41b2a82ce18.css" integrity="sha256-olAQE7hOYGLJFxox1P2yIlOQEm3cXYRTGIvEGyqCzhg=" media="all" rel="stylesheet" />
    
    
    


    <meta http-equiv="x-pjax-version" content="a167fd1067b2539abfd52f8a30eb6b68">

      
  <meta name="description" content="ammo.js - Direct port of the Bullet physics engine to JavaScript using Emscripten">
  <meta name="go-import" content="github.com/kripken/ammo.js git https://github.com/kripken/ammo.js.git">

  <meta content="173661" name="octolytics-dimension-user_id" /><meta content="kripken" name="octolytics-dimension-user_login" /><meta content="1815807" name="octolytics-dimension-repository_id" /><meta content="kripken/ammo.js" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="1815807" name="octolytics-dimension-repository_network_root_id" /><meta content="kripken/ammo.js" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/kripken/ammo.js/commits/master.atom" rel="alternate" title="Recent Commits to ammo.js:master" type="application/atom+xml">

  </head>


  <body class="logged_out   env-production macintosh vis-public page-blob">
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>

    
    
    



      
      <div class="header header-logged-out" role="banner">
  <div class="container clearfix">

    <a class="header-logo-wordmark" href="https://github.com/" data-ga-click="(Logged out) Header, go to homepage, icon:logo-wordmark">
      <span class="mega-octicon octicon-logo-github"></span>
    </a>

    <div class="header-actions" role="navigation">
        <a class="btn btn-primary" href="/join" data-ga-click="(Logged out) Header, clicked Sign up, text:sign-up">Sign up</a>
      <a class="btn" href="/login?return_to=%2Fkripken%2Fammo.js%2Fblob%2Fmaster%2FREADME.markdown" data-ga-click="(Logged out) Header, clicked Sign in, text:sign-in">Sign in</a>
    </div>

    <div class="site-search repo-scope js-site-search" role="search">
      <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/kripken/ammo.js/search" class="js-site-search-form" data-global-search-url="/search" data-repo-search-url="/kripken/ammo.js/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
  <label class="js-chromeless-input-container form-control">
    <div class="scope-badge">This repository</div>
    <input type="text"
      class="js-site-search-focus js-site-search-field is-clearable chromeless-input"
      data-hotkey="s"
      name="q"
      placeholder="Search"
      aria-label="Search this repository"
      data-global-scope-placeholder="Search GitHub"
      data-repo-scope-placeholder="Search"
      tabindex="1"
      autocapitalize="off">
  </label>
</form>
    </div>

      <ul class="header-nav left" role="navigation">
          <li class="header-nav-item">
            <a class="header-nav-link" href="/explore" data-ga-click="(Logged out) Header, go to explore, text:explore">Explore</a>
          </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="/features" data-ga-click="(Logged out) Header, go to features, text:features">Features</a>
          </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="https://enterprise.github.com/" data-ga-click="(Logged out) Header, go to enterprise, text:enterprise">Enterprise</a>
          </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="/pricing" data-ga-click="(Logged out) Header, go to pricing, text:pricing">Pricing</a>
          </li>
      </ul>

  </div>
</div>



    <div id="start-of-content" class="accessibility-aid"></div>

    <div id="js-flash-container">
</div>


    <div role="main" class="main-content">
        <div itemscope itemtype="http://schema.org/WebPage">
    <div id="js-repo-pjax-container" class="context-loader-container js-repo-nav-next" data-pjax-container>
      
<div class="pagehead repohead instapaper_ignore readability-menu experiment-repo-nav">
  <div class="container repohead-details-container">

    

<ul class="pagehead-actions">

  <li>
      <a href="/login?return_to=%2Fkripken%2Fammo.js"
    class="btn btn-sm btn-with-count tooltipped tooltipped-n"
    aria-label="You must be signed in to watch a repository" rel="nofollow">
    <span class="octicon octicon-eye"></span>
    Watch
  </a>
  <a class="social-count" href="/kripken/ammo.js/watchers">
    60
  </a>

  </li>

  <li>
      <a href="/login?return_to=%2Fkripken%2Fammo.js"
    class="btn btn-sm btn-with-count tooltipped tooltipped-n"
    aria-label="You must be signed in to star a repository" rel="nofollow">
    <span class="octicon octicon-star"></span>
    Star
  </a>

    <a class="social-count js-social-count" href="/kripken/ammo.js/stargazers">
      738
    </a>

  </li>

  <li>
      <a href="/login?return_to=%2Fkripken%2Fammo.js"
        class="btn btn-sm btn-with-count tooltipped tooltipped-n"
        aria-label="You must be signed in to fork a repository" rel="nofollow">
        <span class="octicon octicon-repo-forked"></span>
        Fork
      </a>

    <a href="/kripken/ammo.js/network" class="social-count">
      94
    </a>
  </li>
</ul>

    <h1 itemscope itemtype="http://data-vocabulary.org/Breadcrumb" class="entry-title public ">
  <span class="octicon octicon-repo"></span>
  <span class="author"><a href="/kripken" class="url fn" itemprop="url" rel="author"><span itemprop="title">kripken</span></a></span><!--
--><span class="path-divider">/</span><!--
--><strong><a href="/kripken/ammo.js" data-pjax="#js-repo-pjax-container">ammo.js</a></strong>

  <span class="page-context-loader">
    <img alt="" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
  </span>

</h1>

  </div>
  <div class="container">
    
<nav class="reponav js-repo-nav js-sidenav-container-pjax js-octicon-loaders"
     role="navigation"
     data-pjax="#js-repo-pjax-container"
     data-issue-count-url="/kripken/ammo.js/issues/counts">

  <a href="/kripken/ammo.js" aria-label="Code" aria-selected="true" class="js-selected-navigation-item selected reponav-item" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /kripken/ammo.js">
    <span class="octicon octicon-code"></span>
    Code
</a>
    <a href="/kripken/ammo.js/issues" class="js-selected-navigation-item reponav-item" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /kripken/ammo.js/issues">
      <span class="octicon octicon-issue-opened"></span>
      Issues
      <span class="counter">51</span>

</a>
  <a href="/kripken/ammo.js/pulls" class="js-selected-navigation-item reponav-item" data-hotkey="g p" data-selected-links="repo_pulls /kripken/ammo.js/pulls">
    <span class="octicon octicon-git-pull-request"></span>
    Pull requests
    <span class="counter">1</span>

</a>

  <a href="/kripken/ammo.js/pulse" class="js-selected-navigation-item reponav-item" data-selected-links="pulse /kripken/ammo.js/pulse">
    <span class="octicon octicon-pulse"></span>
    Pulse
</a>
  <a href="/kripken/ammo.js/graphs" class="js-selected-navigation-item reponav-item" data-selected-links="repo_graphs repo_contributors /kripken/ammo.js/graphs">
    <span class="octicon octicon-graph"></span>
    Graphs
</a>

</nav>

  </div>
</div>

<div class="container repo-container new-discussion-timeline experiment-repo-nav">
  <div class="repository-content">

    

<a href="/kripken/ammo.js/blob/5ac1b031101112526656f0bd6a1a291c2ebad611/README.markdown" class="hidden js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:110f829da8db5b22703239d0b099533e -->

  <div class="file-navigation js-zeroclipboard-container">
    
<div class="select-menu js-menu-container js-select-menu left">
  <button class="btn btn-sm select-menu-button js-menu-target css-truncate" data-hotkey="w"
    title="master"
    type="button" aria-label="Switch branches or tags" tabindex="0" aria-haspopup="true">
    <i>Branch:</i>
    <span class="js-select-button css-truncate-target">master</span>
  </button>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax aria-hidden="true">

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <span class="octicon octicon-x js-menu-close" role="button" aria-label="Close"></span>
        <span class="select-menu-title">Switch branches/tags</span>
      </div>

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Filter branches/tags" id="context-commitish-filter-field" class="js-filterable-field js-navigation-enable" placeholder="Filter branches/tags">
        </div>
        <div class="select-menu-tabs">
          <ul>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="branches" data-filter-placeholder="Filter branches/tags" class="js-select-menu-tab" role="tab">Branches</a>
            </li>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="tags" data-filter-placeholder="Find a tag…" class="js-select-menu-tab" role="tab">Tags</a>
            </li>
          </ul>
        </div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches" role="menu">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <a class="select-menu-item js-navigation-item js-navigation-open "
               href="/kripken/ammo.js/blob/gh-pages/README.markdown"
               data-name="gh-pages"
               data-skip-pjax="true"
               rel="nofollow">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <span class="select-menu-item-text css-truncate-target" title="gh-pages">
                gh-pages
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open selected"
               href="/kripken/ammo.js/blob/master/README.markdown"
               data-name="master"
               data-skip-pjax="true"
               rel="nofollow">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <span class="select-menu-item-text css-truncate-target" title="master">
                master
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
               href="/kripken/ammo.js/blob/webidl/README.markdown"
               data-name="webidl"
               data-skip-pjax="true"
               rel="nofollow">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <span class="select-menu-item-text css-truncate-target" title="webidl">
                webidl
              </span>
            </a>
        </div>

          <div class="select-menu-no-results">Nothing to show</div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="tags">
        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <div class="select-menu-item js-navigation-item ">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <a href="/kripken/ammo.js/tree/0.0.3/README.markdown"
                 data-name="0.0.3"
                 data-skip-pjax="true"
                 rel="nofollow"
                 class="js-navigation-open select-menu-item-text css-truncate-target"
                 title="0.0.3">0.0.3</a>
            </div>
            <div class="select-menu-item js-navigation-item ">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <a href="/kripken/ammo.js/tree/0.0.2/README.markdown"
                 data-name="0.0.2"
                 data-skip-pjax="true"
                 rel="nofollow"
                 class="js-navigation-open select-menu-item-text css-truncate-target"
                 title="0.0.2">0.0.2</a>
            </div>
        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div>

    </div>
  </div>
</div>

    <div class="btn-group right">
      <a href="/kripken/ammo.js/find/master"
            class="js-show-file-finder btn btn-sm"
            data-pjax
            data-hotkey="t">
        Find file
      </a>
      <button aria-label="Copy file path to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button tooltipped tooltipped-s" data-copied-hint="Copied!" type="button">Copy path</button>
    </div>
    <div class="breadcrumb js-zeroclipboard-target">
      <span class="repo-root js-repo-root"><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/kripken/ammo.js" class="" data-branch="master" data-pjax="true" itemscope="url"><span itemprop="title">ammo.js</span></a></span></span><span class="separator">/</span><strong class="final-path">README.markdown</strong>
    </div>
  </div>

<include-fragment class="commit-tease" src="/kripken/ammo.js/contributors/master/README.markdown">
  <div>
    Fetching contributors&hellip;
  </div>

  <div class="commit-tease-contributors">
    <img alt="" class="loader-loading left" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32-EAF2F5.gif" width="16" />
    <span class="loader-error">Cannot retrieve contributors at this time</span>
  </div>
</include-fragment>
<div class="file">
  <div class="file-header">
  <div class="file-actions">

    <div class="btn-group">
      <a href="/kripken/ammo.js/raw/master/README.markdown" class="btn btn-sm " id="raw-url">Raw</a>
        <a href="/kripken/ammo.js/blame/master/README.markdown" class="btn btn-sm js-update-url-with-hash">Blame</a>
      <a href="/kripken/ammo.js/commits/master/README.markdown" class="btn btn-sm " rel="nofollow">History</a>
    </div>

        <a class="octicon-btn tooltipped tooltipped-nw"
           href="https://mac.github.com"
           aria-label="Open this file in GitHub Desktop"
           data-ga-click="Repository, open with desktop, type:mac">
            <span class="octicon octicon-device-desktop"></span>
        </a>

        <button type="button" class="octicon-btn disabled tooltipped tooltipped-nw"
          aria-label="You must be signed in to make or propose changes">
          <span class="octicon octicon-pencil"></span>
        </button>
        <button type="button" class="octicon-btn octicon-btn-danger disabled tooltipped tooltipped-nw"
          aria-label="You must be signed in to make or propose changes">
          <span class="octicon octicon-trashcan"></span>
        </button>
  </div>

  <div class="file-info">
      171 lines (106 sloc)
      <span class="file-info-divider"></span>
    5.24 KB
  </div>
</div>

  
  <div id="readme" class="blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="mainContentOfPage"><h1><a id="user-content-ammojs" class="anchor" href="#ammojs" aria-hidden="true"><span class="octicon octicon-link"></span></a>ammo.js</h1>

<h1><a id="user-content-demos" class="anchor" href="#demos" aria-hidden="true"><span class="octicon octicon-link"></span></a>Demos</h1>

<ul>
<li><a href="http://kripken.github.com/ammo.js/examples/webgl_demo/ammo.html">Cubes</a></li>
<li><a href="http://kripken.github.com/ammo.js/examples/webgl_demo_terrain/index.html">Heightmap</a></li>
</ul>

<h1><a id="user-content-overview" class="anchor" href="#overview" aria-hidden="true"><span class="octicon octicon-link"></span></a>Overview</h1>

<p><strong>Example code to give you an idea of the API: <a href="https://github.com/kripken/ammo.js/blob/master/examples/webgl_demo/ammo.html#L14">https://github.com/kripken/ammo.js/blob/master/examples/webgl_demo/ammo.html#L14</a></strong></p>

<p>ammo.js is a direct port of the <a href="http://bulletphysics.org/">Bullet physics engine</a> to JavaScript, using Emscripten. The source code is translated directly to JavaScript, without human rewriting, so functionality should be identical to the original Bullet.</p>

<p><strong>Note: ammo.js has just been updated to a new porting approach. If you find some part of the Bullet API that is not supported that you need, please see <a href="https://github.com/kripken/ammo.js/issues/60">https://github.com/kripken/ammo.js/issues/60</a></strong></p>

<p>'ammo' stands for "Avoided Making My Own js physics engine by compiling bullet from C++" ;)</p>

<p>ammo.js is zlib licensed, just like Bullet.</p>

<p>Discussion takes place on IRC at #emscripten on Mozilla's server (irc.mozilla.org)</p>

<h2><a id="user-content-instructions" class="anchor" href="#instructions" aria-hidden="true"><span class="octicon octicon-link"></span></a>Instructions</h2>

<p><code>builds/ammo.js</code> contains a prebuilt version of ammo.js. This is probably what you want.</p>

<p>You can also build ammo.js yourself, as follows:</p>

<ul>
<li><p>Get Emscripten</p>

<p><a href="http://emscripten.org">http://emscripten.org</a></p>

<p>and set it up. See</p>

<p><a href="https://github.com/kripken/emscripten/wiki/Getting-started">https://github.com/kripken/emscripten/wiki/Getting-started</a></p></li>
<li><p>Run the build script,</p>

<p><code>python make.py</code></p>

<p>which should generate builds/ammo.js.</p></li>
<li><p>Optionally, run the automatic tests,</p>

<p><code>python test.py</code></p></li>
</ul>

<h2><a id="user-content-usage" class="anchor" href="#usage" aria-hidden="true"><span class="octicon octicon-link"></span></a>Usage</h2>

<p>The most straightforward thing is if you want to write your code in C++, and
run that on the web. If so, then compile your code into LLVM, link it with
bullet, and compile that to JavaScript using emscripten. (The easiest way to
link it is to add your .bc file to the llvm-link command in make.py.)</p>

<p>If, on the other hand, you want to write code in JavaScript, you can use the
autogenerated binding code. A complete example appears in</p>

<p><code>examples/hello_world.js</code></p>

<p>That is HelloWorld.cpp from Bullet, translated to JavaScript. Other examples
in that directory might be useful as well. In particular see the WebGL
demo code in</p>

<p><code>examples/webgl_demo/ammo.html</code></p>

<h1><a id="user-content-bindings-api" class="anchor" href="#bindings-api" aria-hidden="true"><span class="octicon octicon-link"></span></a>Bindings API</h1>

<p>ammo.js autogenerates its API from the Bullet source code, so it should
be basically identical. There are however some differences and things
to be aware of:</p>

<ul>
<li><p>See <a href="https://github.com/kripken/emscripten/wiki/WebIDL-Binder">https://github.com/kripken/emscripten/wiki/WebIDL-Binder</a>
for a description of the bindings tool we use here, which includes
instructions for how to use the wrapped objects.</p></li>
<li><p>All ammo.js elements should be accessed through <code>Ammo.*</code>. For example,
<code>Ammo.btVector3</code>, etc., as you can see in the example code.</p></li>
<li><p>Member variables of structs and classes can be accessed through
setter and getter functions, that are prefixed with <code>|get_|</code> or <code>|set_|</code>.
For example,</p>

<p><code>rayCallback.get_m_rayToWorld()</code></p>

<p>will get <code>m_rayToWorld</code> from say a <code>ClosestRayResultCallback</code>. Native
JavaScript getters and setters could give a slightly nicer API here,
however their performance is potentially problematic.</p></li>
<li><p>Functions returning or getting <code>float&amp;</code> or <code>btScalar&amp;</code> are converted to
float. The reason is that <code>float&amp;</code> is basically <code>float*</code> with nicer syntax
in C++, but from JavaScript you would need to write to the heap every
time you call such a function, making usage very ugly. With this change,
you can do <code>|new btVector3(5, 6, 7)|</code> and it will work as expected. If
you find a case where you need the float&amp; method, please file an issue.</p></li>
<li><p>Not all classes are exposed, as only what is described in ammo.idl is
wrapped. Please submit pull requests with extra stuff that you need
and add.</p></li>
<li><p>There is experimental support for binding operator functions. The following
might work:</p>

<table><thead>
<tr>
<th>Operator</th>
<th>Name in JS</th>
</tr>
</thead><tbody>
<tr>
<td><code>=</code></td>
<td><code>op_set</code></td>
</tr>
<tr>
<td><code>+</code></td>
<td><code>op_add</code></td>
</tr>
<tr>
<td><code>-</code></td>
<td><code>op_sub</code></td>
</tr>
<tr>
<td><code>*</code></td>
<td><code>op_mul</code></td>
</tr>
<tr>
<td><code>/</code></td>
<td><code>op_div</code></td>
</tr>
<tr>
<td><code>[]</code></td>
<td><code>op_get</code></td>
</tr>
<tr>
<td><code>==</code></td>
<td><code>op_eq</code></td>
</tr>
</tbody></table></li>
</ul>

<h1><a id="user-content-troubleshooting" class="anchor" href="#troubleshooting" aria-hidden="true"><span class="octicon octicon-link"></span></a>Troubleshooting</h1>

<ul>
<li><p>It's easy to forget to write |new| when creating an object, for
example</p>

<p><code>var vec = Ammo.btVector3(1,2,3); // This is wrong! Need 'new'!</code></p>

<p>This can lead to error messages like the following:</p>

<p><code>Cannot read property 'a' of undefined</code>
  <code>Cannot read property 'ptr' of undefined</code></p>

<p>This is an annoying aspect of JavaScript, sadly.</p></li>
</ul>

<h1><a id="user-content-reporting-issues" class="anchor" href="#reporting-issues" aria-hidden="true"><span class="octicon octicon-link"></span></a>Reporting Issues</h1>

<p>If you find a bug in ammo.js and file an issue, please include a script
that reproduces the problem. That way it is easier to debug, and we can
then include that script in our automatic tests.</p>

<h1><a id="user-content-release-process" class="anchor" href="#release-process" aria-hidden="true"><span class="octicon octicon-link"></span></a>Release Process</h1>

<p>Pushing a new build in <code>builds/ammo.js</code> should be done only after the
following steps:</p>

<ul>
<li><p>Build a safe build and make sure it passes all automatic tests. Safe
builds contain a lot of runtime assertions that can catch potential
bugs (similar to the sort of things valgrind can catch).</p></li>
<li><p>Build a fast build and make sure it passes all automatic tests.</p></li>
<li><p>Run closure compiler on that fast build and make sure it passes
all automatic tests.</p></li>
<li><p>Make sure that the stress test benchmark did not regress
compared to the old build.</p></li>
<li><p>Run the WebGL demo in examples/webgl_demo and make sure it looks
ok.</p></li>
</ul>

<h1><a id="user-content-upstream-version" class="anchor" href="#upstream-version" aria-hidden="true"><span class="octicon octicon-link"></span></a>Upstream Version</h1>

<p>Bullet 2.82</p>
</article>
  </div>

</div>

<a href="#jump-to-line" rel="facebox[.linejump]" data-hotkey="l" style="display:none">Jump to Line</a>
<div id="jump-to-line" style="display:none">
  <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="" class="js-jump-to-line-form" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
    <input class="linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
    <button type="submit" class="btn">Go</button>
</form></div>

  </div>
  <div class="modal-backdrop"></div>
</div>

    </div>
  </div>

    </div>

      <div class="container">
  <div class="site-footer" role="contentinfo">
    <ul class="site-footer-links right">
        <li><a href="https://status.github.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
      <li><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
      <li><a href="https://shop.github.com" data-ga-click="Footer, go to shop, text:shop">Shop</a></li>
        <li><a href="https://github.com/blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a href="https://github.com/about" data-ga-click="Footer, go to about, text:about">About</a></li>
        <li><a href="https://github.com/pricing" data-ga-click="Footer, go to pricing, text:pricing">Pricing</a></li>

    </ul>

    <a href="https://github.com" aria-label="Homepage">
      <span class="mega-octicon octicon-mark-github" title="GitHub"></span>
</a>
    <ul class="site-footer-links">
      <li>&copy; 2015 <span title="0.08307s from github-fe130-cp1-prd.iad.github.net">GitHub</span>, Inc.</li>
        <li><a href="https://github.com/site/terms" data-ga-click="Footer, go to terms, text:terms">Terms</a></li>
        <li><a href="https://github.com/site/privacy" data-ga-click="Footer, go to privacy, text:privacy">Privacy</a></li>
        <li><a href="https://github.com/security" data-ga-click="Footer, go to security, text:security">Security</a></li>
        <li><a href="https://github.com/contact" data-ga-click="Footer, go to contact, text:contact">Contact</a></li>
        <li><a href="https://help.github.com" data-ga-click="Footer, go to help, text:help">Help</a></li>
    </ul>
  </div>
</div>



    
    
    

    <div id="ajax-error-message" class="flash flash-error">
      <span class="octicon octicon-alert"></span>
      <button type="button" class="flash-close js-flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
        <span class="octicon octicon-x"></span>
      </button>
      Something went wrong with that request. Please try again.
    </div>


      <script crossorigin="anonymous" integrity="sha256-l2+92s2tzzK6vbHiyKRvr+c1chcJSka10K/YmAXWu/c=" src="https://assets-cdn.github.com/assets/frameworks-976fbddacdadcf32babdb1e2c8a46fafe7357217094a46b5d0afd89805d6bbf7.js"></script>
      <script async="async" crossorigin="anonymous" integrity="sha256-N72+QTuNY+tARklDiRZxG/c1B+GXowOYCXvHFursd4Q=" src="https://assets-cdn.github.com/assets/github-37bdbe413b8d63eb404649438916711bf73507e197a30398097bc716eaec7784.js"></script>
      
      
      
    <div class="js-stale-session-flash stale-session-flash flash flash-warn flash-banner hidden">
      <span class="octicon octicon-alert"></span>
      <span class="signed-in-tab-flash">You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
      <span class="signed-out-tab-flash">You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
    </div>
  </body>
</html>

