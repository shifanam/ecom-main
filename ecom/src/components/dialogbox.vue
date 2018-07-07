<template>
  <div class="row">
    <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12">
      <div class="row">
        <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12">
          <div data-role="main" class="ui-content">
            <p>Welcome!</p>
            <a href="#pagetwo">Go to Dialog Page</a>
          </div>
          <div data-role="page" data-dialog="true" id="pagetwo">
            <div data-role="header">
              <h1>I'm A Dialog Box!</h1>
            </div>
            <div data-role="main" class="ui-content">
              <p>The dialog box is different from a normal page, it is displayed on top of the current page and it will not span the entire width of the page. The dialog has also an icon of "X" in the header to close the box.</p>
              <a href="#pageone">Go to Page One</a>
            </div>
            <div data-role="footer">
              <h1>Footer Text In Dialog</h1>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
