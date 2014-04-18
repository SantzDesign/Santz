# Santz Front-end Bolierplate

Santz front-end boilerplate. Responsive, HTML5, retina-ready, IE9+


### Setup folder structure

The bolierplate has 5 main folders:
 * CSS, which contains a DIST folder for compiled CSS and a SASS folder for development
 * Fonts
 * Images
 * Includes
 * JavaScript


### Make CSS consistent

Having consistent rules which each developer abodes by means that teams can quickly scale without introducing confusion about how a component works.

##### 1) Class names should contain hyphens

Just convention. Prettier.

##### 2) Use nesting sparingly

If using a pre-processor, don't nest more the 3 times if possible. This simplifies resulting CSS rules and makes specificity easier.

##### 3) Only use IDs when necessary  

IDs are fine in the following contexts.
 * Main logo
 * Forms
 * Anchors

IDs should not be used as a styling tool.

##### 4) General style guidelines

CSS should be beautifully designed, just as the site you are coding. Keep these in mind:

 * { on same line as selector
 * Space between rule and brace ( ".asd" { NOT ".asd{" )
 * Properties on new line, unless if it's a single property
 * Properties in somekind of logical order
 * space between property and value colon ( "display: none" NOT "display:none" )
 * 1 line between rules
 * 2 space tabs should be used in files

See example...

    .class {
      property: value;

      @include anymixin(value);

      &.class { property: value; }

      &.class {
        property: value;
        property: value;
      }
    }


### Workflow

This is particularly important for responsive.

In terms of workflow I consider that working on larger sizes first helps.

 1. Build desktop sizes.
 2. Test.
 3. Start building the responsive adaptations.
 4. Test.
 5. Deploy.


### Credits

 - Bootstrap, grid concepts // http://getbootstrap.com
 - Skeleton, grid concepts // http://www.getskeleton.com
 - HTML5 Doctor Reset, CSS reset // http://html5doctor.com/html-5-reset-stylesheet
 - Compass // http://compass-style.org
