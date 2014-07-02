import startApp from 'sample/tests/helpers/start-app';

var App;

module('Integration - Landing Page', {
  setup: function() {
    App = startApp();
  }
});

test('Should welcome me to Sample Ember', function() {
  visit('/').then(function() {
    equal(find('h2#title').text(), 'Welcome to Sample Ember');
  });
});
test('Should allow navigating back to root from another page', function() {
  visit('/about').then(function() {
    click('a:contains("Home")').then(function() {
      notEqual(find('h3').text(), 'About');
    });
  });
});
