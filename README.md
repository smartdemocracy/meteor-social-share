# lukemadera:social-share

Cross platform (inc. Cordova) social sharing for facebook, twitter, pinterest


## Demo

[Demo](http://lukemadera-packages.meteor.com/social-share-basic)

[Source](https://github.com/lukemadera/meteor-packages/tree/master/social-share/basic)


## Dependencies

[none]


## Installation

In a Meteor app directory:
```bash
meteor add lukemadera:social-share
```


## Usage

### Blaze

```html
{{> lmSocialShare opts=opts}}
```

```js
if(Meteor.isClient) {
  Template.socialShareBasic.helpers({
    opts: function() {
      var opts ={
        facebook: true,
        twitter: true,
        pinterest: false,
        shareData: {
          url: 'http://google.com'
        }
      };
      return opts;
    }
  });
}
```
## React

```js

// in a react component:
  let opts = {
        facebook: true,
        twitter: true,
        pinterest: false,
        shareData: {
          url: 'http://google.com'
        }
    };
    
  <LmSocialShare {... opts} />
  

```
Then style as needed with the `lm-social-share-btn` and `lm-social-share-facebook`, `lm-social-share-twitter`, `lm-social-share-pinterest` classes.
