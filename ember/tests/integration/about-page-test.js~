import startApp from 'sample/tests/helpers/start-app';

var App;

module('Integration - About Page', {
  setup: function() {
    App = startApp();
  }
});

test('Should navigate to the About page', function() {
  visit('/').then(function() {
    click("a:contains('About')").then(function() {
      equal(find('h3').text(), 'About');
    });
  });
});
