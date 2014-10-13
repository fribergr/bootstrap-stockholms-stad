Stockholms stad theme for Bootstrap
===================================

Prerequisite
------------
* Node.js (http://nodejs.org)
* Less (`npm install less`)

Compilation
-----------
* Copy `variables_sthlm.less` into less-folder of bootstrap source.
* Add `@import "variables_sthlm.less";` to `bootstrap.less` (directly after `@import "variables.less";` (should be line 3)
* Compile with: `lessc less/bootstrap.less > stockholm_stad_bs.css`


Usage
-----
For ordinary bootstrap functionality, just use the compiled CSS file instead of Bootstraps own CSS and you should be good to go.

---

The `stockholm_stad.css` file does contain some classes that may be used for footers, information boxes, Stockholms stad-flavoured panels, navbars and helpclasses for structuring the logo in the page header.

**The following classes has been added**

* sthlm-footer-primary
* sthlm-footer-primary-light
* sthlm-footer-success
* sthlm-footer-success-light
* sthlm-footer-info
* sthlm-footer-info-light
* sthlm-footer-warning
* sthlm-footer-warning-light
* sthlm-footer-danger
* sthlm-footer-danger-light
* sthlm-primary
* sthlm-success
* sthlm-info
* sthlm-warning
* sthlm-danger
* panel-sthlm

**Example code for full screen footers**

	<div class="sthlm-footer-danger">
	 <div class="container">
	  <div class="row">
	   <div class="col-md-4"><h2>Some stuff</h2><p>Some more stuffs</p></div>
	   <div class="col-md-4"><h2>Some stuff</h2><p>Some more stuffs</p></div>
	   <div class="col-md-4"><h2>Some stuff</h2><p>Some more stuffs</p></div>
	  </div>
	 </div>
	</div>
*Make sure the footers are outside any `<div class="container">` you may have (otherwise they would not be full width).*


**Example code for information boxes**

	<div class="sthlm-footer-danger">
	 <h4>sthlm-footer-danger</h4>
	 <p>Just a div containing some information that should most likely look good on any screen.</p>
	</div>

**Example code for restyling panels**

	<div class="panel panel-success panel-sthlm">
	 <div class="panel-heading">
	  <h3 class="panel-title">Panel success sthlm</h3>
	 </div>
	 <div class="panel-body">
	  Panel content
	 </div>
	</div>

**Example code for navbar following primary color scheme**

    <nav class="navbar navbar-default sthlm-primary" role="navigation">

**Example code for header with logo and text**

    <div class="sthlm-header">
      <a id="sthlm-logo" href="#">
        <img src="img/logo.png" alt="Home" />
        <div><h1>Page header</h1></div>
      </a>
    </div>
